# Boligmatch — OT Bolig- & Erhvervsudlejning

Matchmaker til boligsøgende og erhvervsdrivende i Trekantområdet.

**Live:** https://jimhoeeg.github.io/OTbolig/

| Fil | Indhold |
|---|---|
| [`index.html`](index.html) | Hele widgeten. Én selvstændig fil uden byggetrin eller afhængigheder ud over Google Fonts. |
| [`INTEGRATION.md`](INTEGRATION.md) | Sådan lægges den på otbolig.dk, konfigureres og sættes i drift. |
| [`KONCEPT-MATCHMAKER.md`](KONCEPT-MATCHMAKER.md) | Konceptoplægget bag: research, flow, tillidselementer og afgrænsning. |

Alt, der skal vedligeholdes — ledige lejemål, ventelistetal, kontaktpersoner og
modtager af henvendelser — ligger i `CONFIG`-objektet øverst i `index.html`.
Resten af filen behøver ikke at blive rørt.
