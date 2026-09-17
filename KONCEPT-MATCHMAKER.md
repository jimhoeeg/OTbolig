# Boligmatch — matchmaker til OT Bolig- & Erhvervsudlejning

Konceptoplæg. Version 1, september 2026.

---

## 1. Hvem er OT Bolig?

**OT Bolig- & Erhvervsudlejning ApS** (CVR 27282792), House of Innovation, Jernbanegade 27, 6000 Kolding.

| Forhold | Fakta |
|---|---|
| Stiftet | 1. august 2003 af Ole Lind Terkelsen — som stadig ejer og driver selskabet |
| Størrelse | Ca. 30 ejendomme, ca. 200 lejemål (100+ lejligheder) |
| Typer | Lejligheder 1–5 værelser + erhverv: butik, kontor, lager, værksted |
| Geografi | Kolding, Vejle, Haderslev, Lunderskov, Vamdrup, Christiansfeld, Grindsted, Sdr. Omme, Gesten, Billund — samt Vejers og Bork Havn |
| Koncern | Moderselskab Terkelsen Invest ApS. Medejer af Grindsted Ejendomsselskab |
| Administration | 100 % egen administration — bevidst strategi om at komme "tættere på lejerne" |
| Nøglepersoner | Ole Terkelsen (ejer), 20 85 33 95 · Rickie Bjørn Wilken (ejendomsadministrator), 40 18 79 30 |
| Systemer | Boligmanager som administrationssystem + egen lejerportal |
| Drift | Egen ansat vicevært + faste lokale håndværkere i hver by |
| Service i dag | Guide til bedre indeklima, tjekliste ved skader, fraflytningstjekliste |

### Det der betyder noget strategisk

1. **De er udlejer — ikke portal.** De ejer selv murstenene. Det er den absolut stærkeste tillidsposition på et marked, hvor boligsøgende er trætte af betalingsportaler og bange for svindelannoncer.
2. **Lukket, begrænset beholdning.** ~200 lejemål med lav udskiftning betyder, at der sjældent er mange ledige på én gang. En matchmaker kan derfor ikke kun være en søgemaskine — den skal først og fremmest være en **efterspørgselsmotor**, der fanger behovet, *før* boligen bliver ledig.
3. **Tomgang er den reelle økonomi.** Hver måneds tomgang på et lejemål er direkte tabt indtjening. En matchmaker, der på opsigelsesdagen kan udpege de 5 rigtige kandidater, betaler sig selv hjem.
4. **To vidt forskellige kunder.** Privat er selvbetjening og følelser. Erhverv er rådgivning, m², og et opkald fra Ole. Samme indgang, to spor.
5. **Ejerhistorik som aktiv.** Samme ejer i 23 år, egen administration, eget navn og telefonnummer på hjemmesiden. Det skal frem i lyset, ikke gemmes i en "Om os"-fane.

> **Kildeforbehold:** otbolig.dk kunne ikke hentes direkte fra dette miljø (blokeret af netværkets egress-policy). Ovenstående bygger på søgeresultater med indhold fra otbolig.dk's egne sider (forside, Om os, Service, Ejendomme, Ny ejendomsadministrator) samt offentlige registre (CVR, Proff). Tal og formuleringer bør verificeres med Ole, før de bruges i markedsføring.

---

## 2. Grundidé

> **Boligmatch: 60 sekunder, 7 spørgsmål — og du ved, præcis hvor du står.**

Ikke et ansøgningsskema. En kort, guidet samtale, der ender med ét af tre ærlige svar:

- **"Vi har 2 boliger til dig lige nu."**
- **"Ikke lige nu — men du er nr. 4 i køen til 3-værelses i Kolding, og vi skriver til dig, før boligen kommer på nettet."**
- **"Vi har ikke noget, der passer. Her er, hvad vi faktisk har."**

Det tredje svar er det vigtigste. **Et ærligt nej er den billigste tillid, man kan købe.**

---

## 3. Flowet — privat

Ét spørgsmål pr. skærm. Mobil først. Ingen login. Ingen kontaktoplysninger, før der er leveret værdi.

| # | Skærm | Indhold | Hvorfor |
|---|---|---|---|
| 0 | Split | Privat / Erhverv | Deler i to spor med det samme |
| 1 | Hvor vil du bo? | By-chips (Kolding, Vejle, Grindsted, Billund, Christiansfeld, Lunderskov, Vamdrup, Sdr. Omme, Haderslev, Gesten) + "Jeg er fleksibel" | Flervalg udvider matchfladen markant |
| 2 | Hvor stor? | 1–2 / 2–3 / 3–4 / 4+ værelser | Nemt at svare på, præcist nok til at matche |
| 3 | Budget | Slider for husleje, med tydelig markering af inkl./ekskl. forbrug | Fjerner det største senere frafald |
| 4 | Hvornår? | Hurtigst muligt / inden for 3 mdr. / 3–6 mdr. / jeg orienterer mig | Segmenterer varme fra kolde leads |
| 5 | Hvad betyder mest? | Vælg op til 3: altan/have, husdyr tilladt, elevator, p-plads, plads til vaskemaskine, nyrenoveret, tæt på skole/station, lav varmeudgift | Skaber ejerskab og giver OT reel produktviden |
| 6 | Lidt om dig | Husstandstype, fast indkomst (ja/nej), husdyr, ryger | Rammesættes som *"så vi kan finde det rigtige — ikke for at sortere dig fra"* |
| 7 | **Resultatet** | Se nedenfor | Selve produktet |
| 8 | Kontakt | Navn, mail, mobil — og kun det | Bedes om *efter* værdien er leveret |

### Resultatskærmen — hele forretningen ligger her

**A · Direkte match**
Boligkort med billeder, husleje, **fuld månedlig ydelse** (husleje + aconto), depositum og forudbetalt leje udregnet i kroner, indflytningsdato, og én knap: *"Book fremvisning"*.

**B · Delvist match**
> *"Vi har ingen 3-værelses i Kolding under 8.000 kr. ledige lige nu. Der bliver typisk 3–4 ledige om året. Du står nu nr. 4 på listen — og vi skriver til dig, før boligen kommer på nettet."*
Plus 2–3 nærmeste alternativer (naboby, ét værelse mindre, 500 kr. mere).

**C · Intet match**
Sig det rent ud, og vis hvad der *faktisk* findes. Ingen pyntede resultater.

### Den økonomiske klarhedsboks

Vises på hvert boligkort og er et undervurderet konverteringsværktøj:

```
Husleje                  6.800 kr.
Aconto varme/vand          900 kr.
──────────────────────────────────
Pr. måned                7.700 kr.

Ved indflytning
Depositum (3 mdr.)      20.400 kr.
Forudbetalt leje (1 md.) 6.800 kr.
──────────────────────────────────
I alt                   27.200 kr.
```

Hovedparten af boligsøgende springer fra, fordi de ikke tør spørge om totalen. Vis den uopfordret.

---

## 4. Flowet — erhverv

Kortere, tungere, og ender altid i et menneske.

1. **Hvad skal I bruge?** Kontor / Butik / Lager / Værksted / Klinik / Showroom
2. **Hvor mange m²?** 20–50 / 50–150 / 150–500 / 500+
3. **Hvor?** By-chips
4. **Hvornår + hvor længe?** Indflytning + ønsket lejeperiode
5. **Praktiske krav:** Facade/kundeadgang, port eller rampe, loftshøjde, parkering, 3-faset strøm, antal kontorpladser
6. **Firma:** CVR-opslag der autoudfylder navn, adresse og branche (mindre friktion, mere seriøsitet, bedre kvalificering)
7. **Resultat:** Matchende lokaler + *"Ole ringer dig op inden for 1 arbejdsdag"*

**Erhvervstilliden ligger i personen, ikke i systemet:**
> *"Ole har udlejet erhverv i Trekantområdet siden 2003 og er medejer af Grindsted Ejendomsselskab. Han kender markedet — og kan ofte finde noget, der aldrig bliver annonceret."*

Det sidste er reelt sandt for en privat udlejer, og det er en meget stærk grund til at udfylde formularen frem for at gå på Lokaleportalen.

---

## 5. Sådan skaber vi tillid (det vigtigste afsnit)

Alle punkter herunder er ting, OT Bolig **faktisk kan indfri**. Intet af det er kulisse.

| # | Tillidselement | Konkret udførelse |
|---|---|---|
| 1 | **Ansigter frem for postkasser** | Billede, fulde navn og direkte nummer på Ole og Rickie — på resultatskærmen, ikke begravet i "Om os" |
| 2 | **"Vi er udlejer, ikke portal"** | Sættes øverst: *"Vi ejer selv de 200 lejemål, du søger i. Du taler med ejeren — ikke et mellemled."* |
| 3 | **Anti-svindel-løftet** | Eksplicit, i egen boks: *"Du betaler aldrig for at stå på listen. Vi beder aldrig om MitID, kontooplysninger eller betaling for at se en bolig. Depositum betales først, når kontrakten er underskrevet."* Dette er den største reelle frygt på lejemarkedet |
| 4 | **Ingen skjulte tal** | Total månedlig ydelse + indflytningsomkostninger vist op front på hver bolig |
| 5 | **23 års historik** | *"Samme ejer siden 2003. 30 ejendomme. 200 lejemål. CVR 27282792."* Tal og CVR gør det verificerbart |
| 6 | **Egen administration og egen vicevært** | *"Går vandvarmeren i stykker, ringer du til en, der bor i Trekantområdet — ikke til et callcenter."* |
| 7 | **Ærlig forventningsstyring** | Vis faktisk gennemsnitlig ventetid pr. by og boligtype. Lov mindre, end I leverer |
| 8 | **Svarløfte med tidsramme** | *"Rickie vender tilbage inden for 1 arbejdsdag."* Og så skal det holdes — det er et driftsløfte, ikke et designelement |
| 9 | **Hvad sker der nu?** | Tre trin efter afsendelse: match → fremvisning → kontrakt. Ingen skal være i tvivl |
| 10 | **Lejerudtalelser** | 3–4 korte citater med fornavn, by og boligtype. Gerne Google-anmeldelser med link |
| 11 | **Synlig databehandling** | *"Vi bruger kun dine oplysninger til at finde dig en bolig. Vi videresælger ingenting. Slet dig selv med ét klik."* Plus opbevaringsperiode |
| 12 | **Intet tvunget login** | Resultatet vises, før der spørges om kontaktoplysninger |

---

## 6. Sådan aktiverer vi behovet (uden at presse)

Alt herunder er ægte knaphed — ikke kunstige nedtællinger. Falsk knaphed ødelægger nøjagtig den tillid, vi bygger op i afsnit 5.

- **Reel status:** *"7 ledige lejemål ud af 200 lige nu."* Ærligt, og skaber naturligt tempo.
- **Køposition:** *"Du er nr. 4 til 3-værelses i Kolding."* Et konkret tal skaber ejerskab — folk forlader ikke en plads, de har fået tildelt.
- **Første-kig-løftet:** *"Vi skriver til dig, før boligen kommer på nettet."* Dette er den stærkeste mekanik i hele konceptet — en privat udlejer *kan* faktisk give forkøbsret, og det er en ægte grund til at tilmelde sig nu frem for senere.
- **Økonomisk klarhed:** Totalbeløbet gør drømmen konkret og dermed beslutningsklar.
- **Personlig opfølgning med navn og tidsramme.** Et menneske, der har lovet at ringe, er stærkere end enhver rabat.
- **Sæsonpåmindelse:** *"Flest lejligheder bliver ledige i Kolding omkring studiestart."* Rådgivning, ikke pres.

---

## 7. Hvad OT Bolig får på bagsiden

Matchmakeren er lige så meget et internt værktøj som et kundeprodukt.

- **Efterspørgselsdatabase:** Hvilke byer, størrelser og prisniveauer er der reelt efterspørgsel på? Direkte input til renoveringsplan, prissætning og fremtidige opkøb.
- **Tomgangsdræber:** Ved hver opsigelse trækkes top-5 kandidater frem med det samme. Færre tomme måneder er ren bundlinje.
- **Segmenteret udsendelse:** *"Ny 3-værelses i Vejle — du står nr. 2"* til præcis den rigtige lille gruppe. Ingen nyhedsbrevsstøj.
- **Kvalificering før fremvisning:** Færre spildte visninger, fordi budget, tidshorisont og husstand allerede er kendt.
- **Erhvervspipeline:** Ole ser, hvilke m²-behov der ligger i markedet — også når han ikke har lokalet endnu.

---

## 8. Teknik og integration

- **Boligliste:** Fase 1 kan køre på en simpel, redigerbar datakilde (JSON/CMS) med de ledige lejemål. Fase 2 trækker direkte fra **Boligmanager**, hvis systemet har API — det skal afklares med Ole.
- **Lejerportalen:** Matchmakeren er indgangen *før* lejemålet; lejerportalen er livet *efter*. De skal linke til hinanden, men ikke blandes sammen.
- **Notifikationer:** Mail + SMS ved match. SMS er markant stærkere på "første kig"-løftet.
- **GDPR:** Samtykke med formål og opbevaringsperiode, ét-kliks sletning, ingen videregivelse. Skal være synligt, ikke gemt i en fodnote — det er også et tillidselement.
- **Admin:** Enkel liste over emner med filtre (by, størrelse, budget, tidshorisont), eksport, og "marker som kontaktet".
- **Sprog og tone:** Dansk, du-form, korte sætninger. Samme rolige tone som resten af otbolig.dk.

---

## 9. Afgrænsning

**Fase 1 — MVP**
Privat- og erhvervsflow, matchlogik mod manuelt vedligeholdt boligliste, resultatskærm med økonomiboks, alle 12 tillidselementer, mailnotifikation, admin-liste, GDPR-samtykke.

**Fase 2**
Automatisk "første kig"-udsendelse ved opsigelse, live køposition, CVR-opslag på erhverv, Boligmanager-integration, fremvisningsbooking direkte i kalender, SSO mod lejerportalen.

**Bevidst udenfor**
Betalingsmur, konto-oprettelse for at se resultater, chatbot, scoring der afviser folk automatisk. Alle fire underminerer tilliden mere, end de gavner.

---

## 10. Sådan måler vi, om det virker

| Mål | Hvorfor |
|---|---|
| Gennemførselsrate i flowet | Er det reelt simpelt nok? Mål: over 60 % |
| Emner pr. uge pr. by | Hvor er efterspørgslen? |
| Andel udlejninger, der kom fra matchlisten | Den egentlige forretningsværdi |
| Tomgangsdage før/efter | Den hårde økonomiske effekt |
| Faktisk svartid vs. det lovede | Tillidsløftet er kun værd noget, hvis det holdes |

---

## 11. Spørgsmål til Ole, før vi bygger

1. Har Boligmanager et API — eller skal boliglisten vedligeholdes manuelt i fase 1?
2. Hvor mange lejemål er typisk ledige ad gangen, og hvor lang er den reelle gennemsnitlige tomgang?
3. Findes der allerede en venteliste, og hvordan håndteres den i dag?
4. Hvem svarer på henvendelserne — Rickie, Ole, eller efter type? Og hvilken svartid tør vi love?
5. Skal erhverv fortsat annonceres via Lokaleportalen sideløbende?
6. Må vi bruge konkrete tal (200 lejemål, 30 ejendomme, ventetider) i markedsføringen?
7. Skal Vejers og Bork Havn med som ferieudlejning — eller holdes helt udenfor?
