# Boligmatch — sådan lægges den på otbolig.dk

Én fil: `boligmatch.html`. Ingen build, intet framework, ingen afhængigheder ud over
Google Fonts. Virker i alle nyere browsere, på mobil og i både lys og mørk visning.

---

## 1. Vælg indlejringsmetode

### A. Iframe — anbefalet

Virker på Squarespace, WordPress, Wix og alt andet. Widgetens CSS kan ikke kollidere
med sidens egen. Læg `boligmatch.html` op på serveren, og indsæt:

```html
<iframe src="/boligmatch.html" title="Boligmatch — find din bolig"
        style="width:100%;border:0;display:block" height="900"
        id="boligmatch-frame" loading="lazy"></iframe>

<script>
/* Lader iframen vokse og skrumpe i takt med indholdet */
window.addEventListener("message", function (e) {
  if (e.data && e.data.type === "boligmatch:hoejde") {
    document.getElementById("boligmatch-frame").style.height = e.data.hoejde + "px";
  }
});
</script>
```

Widgeten sender selv sin højde til den omkringliggende side, så der aldrig opstår
en scrollbar inde i iframen.

### B. Direkte på siden

Kopiér hele indholdet af `boligmatch.html` ind i en HTML-blok på siden. Den arver
så sidens baggrundsfarve. Brug kun denne metode, hvis temaet ikke har aggressiv CSS
på `button`, `input` og `fieldset`.

---

## 2. Tilpas indholdet

Alt, der skal vedligeholdes, ligger i det første `<script>`-tag i filen, under
overskriften `KONFIGURATION`. Resten af filen behøver ikke at blive rørt.

| Hvad | Hvor | Bemærk |
|---|---|---|
| Demobjælken | `CONFIG.demo` | Sæt til `false`, når rigtige data er lagt ind |
| Antal lejemål i alt | `CONFIG.totalLejemaal` | Bruges til "X ledige ud af Y lige nu" |
| Modtager af henvendelser | `CONFIG.endpoint` | Se afsnit 3 |
| Lovet svartid | `CONFIG.svartid` | **Skal kunne holdes** — det er et driftsløfte |
| Ole og Rickie | `CONFIG.kontakt` | Tilføj `foto: "/billeder/ole.jpg"` for rigtige portrætter |
| Ventelistetal | `CONFIG.venteliste` | Se advarslen nedenfor |
| Årlig omsætning pr. by | `CONFIG.omsaetning` | Bruges til ærlig forventningsstyring |
| Ledige boliger | `BOLIGER` | Tilføj `billede: "..."` — ellers tegnes en neutral facade |
| Ledige erhvervslejemål | `ERHVERV` | Samme opbygning |

### Ventelistetallene skal være ægte

`CONFIG.venteliste` har formen `"By|antal værelser": antal på listen`:

```js
venteliste: { "Kolding|3": 4, "Vejle|3": 2 }
```

Er der ikke et tal for en given kombination, vises **ingen køplads** — kun løftet om
at blive kontaktet først. Det er med vilje. Et opdigtet kønummer ødelægger præcis den
tillid, resten af widgeten er bygget op om.

---

## 3. Modtag henvendelserne

`CONFIG.endpoint` skal pege på noget, der tager imod `POST` med JSON. Tre muligheder:

1. **Formspree** (hurtigst i gang) — opret en formular, og indsæt dens URL.
2. **Make eller Zapier** — opret et webhook-scenarie, der lægger henvendelsen i
   Boligmanager og sender en mail til Rickie.
3. **Eget endpoint** på serveren bag otbolig.dk.

Sendt JSON ser sådan ud:

```json
{
  "spor": "privat",
  "oensker": { "by": ["Kolding"], "vaerelser": 3, "budget": 7500,
               "tid": "straks", "vigtigt": ["altan","p-plads"],
               "husstand": "par", "indkomst": "ja", "husdyr": "nej", "ryger": "nej" },
  "valgtLejemaal": "kol-99",
  "kontakt": { "navn": "...", "mail": "...", "tlf": "...", "besked": "..." },
  "tidspunkt": "2026-09-17T09:12:44.000Z",
  "kilde": "Boligmatch"
}
```

Er `endpoint` tom, vises kvitteringen alligevel, men **intet sendes**. Brug kun tom
værdi til test. Fejler kaldet, får brugeren en fejlbesked med Oles telefonnummer i
stedet for en blind ende.

---

## 4. Design

Widgeten følger otbolig.dk's egen linje:

| Element | Værdi | Variabel |
|---|---|---|
| Accentfarve | `#1BA1DC` (logoets cyanblå) | `--primary` |
| Struktur og bånd | `#000000` | `--black` |
| Overskrifter | Playfair Display, bold | `--serif` |
| Brødtekst | Lato Light, gråtonet | `--sans`, `--muted` |

Alle farver er variabler øverst i `<style>` under `:root`. Rammer den blå ikke præcist
logoets nuance, rettes `--primary` ét sted — så følger knapper, chips, ikoner, badges
og fremhævninger med. Husk den lysere variant i de to mørke blokke længere nede, så
widgeten også holder i mørk visning.

Brødteksten er venstrestillet i selve flowet, selvom sitet centrerer sin brødtekst.
Det er et bevidst valg: centreret tekst i en formular gør den markant sværere at
udfylde. Overskrifter, resultatbeskeder og introen er centreret som på sitet.

---

## 5. CVR-opslag på erhvervssporet

Feltet findes allerede. Skal det slå firmanavnet op automatisk, tilføjes et kald til
et CVR-API fra jeres egen server (et opslag direkte fra browseren blokeres af de
fleste udbydere). Det er bevidst ikke bygget ind, fordi det kræver en nøgle og et
serverkald, I selv skal stå for.

---

## 6. Inden lancering

- [ ] Rigtige boliger og erhvervslejemål lagt ind i `BOLIGER` og `ERHVERV`
- [ ] Rigtige ventelistetal i `CONFIG.venteliste` — eller felterne fjernet
- [ ] `CONFIG.endpoint` sat op og testet
- [ ] `CONFIG.demo` sat til `false`
- [ ] Portrætter af Ole og Rickie lagt ind
- [ ] Svartiden i `CONFIG.svartid` aftalt med Rickie, så den kan holdes
- [ ] Teksten om databehandling holdt op mod jeres privatlivspolitik
- [ ] Prøvet igennem på en telefon
