---
id: 6813b5d8-5548-4f1a-99dc-d654b2389d12
title: "Resultater og veien videre"
linkTitle: "Resultater og veien videre"
weight: 90
lastmod: 2026-11-22T04:06:29+01:00
last_editor: Erik Hagen

---
Fase 1 ble gjennomført februar–april 2026 og avsluttet med en demo 30. april. Kildene er avslutningspresentasjonen og erfaringsrapporten (versjon 1.0, 24. april 2026).

## Hovedresultater

- **En kjørende POC** overfører elevlisten fra Vigilo via KS Digitals dataplattform, transformert til FINT v4, til et simulert mottak for Vigo Skole. Se [Valgt løsning nå](/pilotering/pilot-1/loesningsvalg/valgt-loesning-naa/).
- **Løsningen gir gevinster** i form av effektivisering og bedre kontroll på informasjonssikkerhet og personvern. Funnene fra Bergen er kvalitetssikret i Arendal, Bykle og Vestland fylkeskommune.
- **Juridisk avklaring:** overføringen i november har hjemmel i opplæringslova § 9-5, kommunen og fylkeskommunen er behandlingsansvarlige hver for seg, og samtykke er ikke riktig grunnlag. Se [Juridiske forhold](/pilotering/pilot-1/juridiske-forhold/).
- **Informasjonsmodeller:** en norsk profil av OneRoster, en konseptuell modell for overføringen og en start på en personmodell i SHACL. Se [Informasjonsarkitektur](/pilotering/pilot-1/loesningsvalg/informasjonsarkitektur/).
- **Et arkitekturråd** med Novari, KS Digital, KS og Digdir ble etablert. Det har laget overordnede rammer for arkitektur, en mal for arkitekturvurderinger med veiledning, og startet på en beskrivelse av hva mellomlaget er.

## Positive læringspunkter

- At sluttbrukerne var med fra start, gjorde det enklere å holde fokus på gevinster.
- Mange involverte samarbeidspartnere gjorde at problemene ble sett på nye måter.
- Å ha jurister i pilotgruppa fra start var en stor fordel. Også jussen kan ha en smidig tilnærming.
- Ved å begynne med noe konkret tidlig ble uforutsette samhandlingsutfordringer avdekket.
- Sektoren har allerede gode standardiserte informasjonsmodeller (FINT og OneRoster).

## Hva som var utfordrende

- For lite planlegging i forkant ga flere diskusjoner og mer famling enn nødvendig.
- Virkelighetsoppfatningen og problemforståelsen spriket. Det noen så som et stort problem, var et ikke-problem for andre.
- Det var ulike syn på hvordan problemet burde løses, og det gikk mye tid til arkitekturvalg.
- Tilgang til data fra kommunenes fagsystemer kan bli kostbart. Leverandørene tar betalt per kommune for å låse opp data, og avtalene tar ikke høyde for deling. Summen blir mange millioner kroner for landet sett under ett.

## Erfaringer og tiltak

Erfaringsrapporten går gjennom hver fase og foreslår tiltak til prosjektets håndbok for piloter (se [Arbeidsmodell](/styring/arbeidsmodell/)).

| Fase | Erfaring | Tiltak |
|---|---|---|
| Velge pilot | Grunnlaget for valget var for tynt, smertepunktene uklare og målene ikke godt nok forankret. Det manglet en tydelig case-eier | Oppdatere malen for casebeskrivelser med case-eier og mål. Sende ut casebeskrivelser og innkalle til workshop i god tid. Peke ut representanter for kommuner og fylkeskommuner |
| Oppstart | For kort tid mellom valg av pilot, planleggingsworkshop og oppstart. Gevinstpotensialet var uklart, og det var ulike meninger om POC-en skulle gi læring eller en kjørbar tjeneste | Bedre tid til planlegging. Definere målene tidlig, med en egen OKR-økt når teamet er satt. Tydelig skille mellom pilotens og kjerneteamets oppgaver, og eskaleringsveier |
| Drømmereise | Drømmereiser tar lengre tid å lage. En felles drømmereise kan avdekke ulik problemforståelse | Skaffe ressurser til drømmereiser eller skalere ned. AS-IS og TO-BE som egne steg i planen |
| Velge POC eller MVP | Uklart om piloten skulle lage POC eller MVP. Valget om å kjøre POC-en hos KS Digital var for dårlig forankret | Som for oppstart |
| Lage det | Høyt tempo i sprinter på to uker fungerte. Det trengs en som holder i piloten. Oppgavene var for store og manglet tydelig «ferdig». For lite samarbeid på tvers av arbeidsgrupper. Engasjementet var vanskelig å holde oppe mot slutten. Alternativene ble ikke evaluert, noe som skapte uklarheter | Sprinter på tre uker med standup annenhver dag. Egen delprosjektleder. Sårbarhetsanalyse tidlig. Felles sted for dokumentasjon (docs.samt-bu.no). Mal for arkitektur- og løsningsbeskrivelser som grunnlag for beslutninger. Fora som tar diskusjoner som løftes ut av piloten (arkitekturforum). Gevinstvurdering som steg i malen |
| Evaluering | OKR ble ikke etablert, men det ble gjort en overordnet gevinstanalyse | |
| Formidling | Piloten ble blant annet presentert på eKommune | Lage en sak om piloten |

Andre erfaringer:

- Det er vanskelig å få data ut av kommunenes fagsystemer, selv når det står i konkurransegrunnlaget. Bergen har erfart dette.
- Kommunikasjonsverktøy og dokumenthåndtering, som Teams, er vanskelig å få til å fungere på tvers av organisasjoner.
- Samarbeidspartnerne må forstå hvor viktig timeføring er, og hvordan reglene for medfinansiering virker.
- De som arbeidet med informasjonsmodeller, brukte mye tid på å sette seg inn i domenet og eksisterende standarder. Noen med god oversikt over domenet ville gitt bedre fart fra start.

## Veien videre

Avslutningen pekte på tre mulige veier: utvikle POC-en videre til en kjørbar MVP, utvide den til også å overføre resultater fra grunnskolen (karakterer), eller utvide den til flere kommuner. Det tar imidlertid tid å kravsette og utvikle et API i Vigo Skole, og de andre casene kan gi viktige innspill.

Den tekniske utviklingen ble derfor satt på pause til slutten av august 2026. Oppstart da gjør det fortsatt mulig å kjøre en MVP på overføringen før jul og en POC på dataene som overføres etter nyttår 2027. Planen for fase 2 står under [Veikart](/pilotering/pilot-1/loesningsvalg/veikart/).
