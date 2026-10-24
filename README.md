# Klassie Studiero – testpaket

Det här repot innehåller bara packade tillägg och deras `update.xml`, så att en Intune-hanterad testdator kan tvinga ut dem. Källkoden och testplanerna ligger i Klassies huvudrepo.

## Provtillägget för förstudien (Paket 7)

- Id: `phcopgoofchobdaeoibcnlegaglpoekh`
- Uppdateringsadress: `https://mattiasandrsson-prog.github.io/klassie-studiero-poc/update.xml`
- Policyvärde för `ExtensionInstallForcelist`: `phcopgoofchobdaeoibcnlegaglpoekh;https://mattiasandrsson-prog.github.io/klassie-studiero-poc/update.xml`
- Källa: `experiments/studiero-extension-poc`, testplan i `docs/skarmhantering-forstudie.md`.

## Tillägget, byggt för staging (Paket 8)

- Id: `kokkfabbjpdjkllofhmcbkjgpeojgaaj`
- Uppdateringsadress: `https://mattiasandrsson-prog.github.io/klassie-studiero-poc/studiero/update.xml`
- Policyvärde för `ExtensionInstallForcelist`: `kokkfabbjpdjkllofhmcbkjgpeojgaaj;https://mattiasandrsson-prog.github.io/klassie-studiero-poc/studiero/update.xml`
- Källa: `extension/`, byggt med `npm run build:extension -- --env staging --pack`. Det går mot stagings Supabase och innehåller bara den publika nyckeln.

Repot tas bort när testerna på testdatorn är klara eller när tillägget har en egen distribution.
