---
# id: auto-generert – kopierte verdier overskrives automatisk ved push
id: d6ff5943-b53d-4da7-8396-c038517ff6ee
title: Juridiske forhold
linkTitle: Juridiske forhold
weight: 60
aliases:
 - /pilotering/pilot-1/juss/
lastmod: 2026-11-22T04:06:29+01:00
last_editor: Erik Hagen

---
En innledende juridisk vurdering av personvernet i fase 1, en vurdering av behovet for en full personvernkonsekvensvurdering (DPIA), og risikoene som ble identifisert i ROS-arbeidet. Piloten gjelder overføringen av elevlisten fra grunnskolen til Vigo i november hvert år.

Vurderingen bygger på en tverrfaglig workshop og flere arbeidsmøter med pilotteamet, der behov, datakilder og overordnede funksjonelle krav ble kartlagt. Den har to formål: å vise hvordan piloten kan gjennomføres lovlig innenfor dagens regelverk, og å peke på tiltak som kan gi større handlingsrom på sikt. Bare personvern er vurdert, ikke andre rettsområder. Dokumentet er dynamisk og skal oppdateres i takt med piloten.

## Ansvar og avtaler

Den behandlingsansvarlige har hovedansvaret for å følge personvernforordningen (GDPR art. 4 nr. 7). Den som behandler opplysninger på vegne av den behandlingsansvarlige, er databehandler (art. 4 nr. 8).

**Kommunen** samler inn personopplysninger om elever for å oppfylle sine lovpålagte oppgaver i grunnskolen, og strukturerer og lagrer dem i egne systemer, som Vigilo og kommunens dataplattform. Kommunen er behandlingsansvarlig for dette.

**Fylkeskommunen** trenger opplysninger om elevene for å behandle søknader om skoleplass og følge opp elevene som tas inn. Det skjer for fylkeskommunens egne formål og i egne systemer, blant annet Vigo.

Kommunen har ingen avtale med Vigo, og fylkeskommunen har ingen avtale med kommunens systemer. Partene har ikke felles kontroll over formål eller midler, og behandler ikke på vegne av hverandre. **Kommunen og fylkeskommunen er derfor behandlingsansvarlige hver for seg.**

**Databehandlere:** leverandøren av kommunens skoleadministrative system (for eksempel Vigilo) og KS Digital behandler opplysninger på vegne av kommunen. Novari IKT behandler opplysninger på vegne av fylkeskommunen i forbindelse med Vigo. Databehandlerne handler etter instruks (art. 28).

## Hjemmel

Det rettslige grunnlaget for å utveksle elevinformasjon mellom grunnskole og videregående følger av kapittel 9 og 25 i opplæringslova og kapittel 20 i opplæringsforskrifta.

- **Opplæringslova § 9-5:** fylkeskommunen skal sørge for en trygg og god overgang fra grunnskolen til videregående opplæring, og kommunen skal samarbeide med fylkeskommunen om overgangen. Det legges til grunn at samarbeidet også omfatter overføring av opplysninger om elever.
- **Opplæringslova § 25-1:** kommuner og fylkeskommuner kan behandle personopplysninger når det er nødvendig for å utføre oppgaver etter loven, og fylkeskommunen kan hente inn nødvendige opplysninger fra grunnskolene for å gjennomføre inntak.
- **Opplæringsforskrifta § 20-4** snevrer inn hva fylkeskommunen kan hente inn ved inntaket: om grunnskolen er fullført, halvårsvurdering med karakterer fra 10. trinn, og karakterer og fravær som føres på vitnemålet.

Overføringen i november gjelder bare navn, fødselsnummer, skole og klasse, som § 20-4 ikke nevner. Den kan likevel hjemles i § 9-5, fordi den bidrar til en lovpålagt oppgave: en god overgang, som også legger til rette for den senere overføringen etter § 20-4.

Behandlingsgrunnlaget etter personvernforordningen er **art. 6 nr. 1 e**: behandlingen er nødvendig for å utøve offentlig myndighet. Supplerende hjemmel er opplæringslova § 9-5, jf. § 25-1. Overføringen omfatter ikke særlige kategorier av personopplysninger, så art. 9 er ikke vurdert.

## Samtykke er ikke riktig grunnlag

Enkelte kommuner baserer i dag overføringen på samtykke. Det er etter vurderingen verken nødvendig eller egnet:

- **Ikke frivillig.** Det er en klar ubalanse mellom elev eller foresatte og skolen, og overføringen henger tett sammen med elevens mulighet til å få behandlet søknaden om skoleplass (art. 4 nr. 11, art. 7 og fortalepunkt 43).
- **Kan ikke trekkes tilbake på en meningsfull måte.** Når dataene er overført og brukt i inntaket, er tilbaketrekking vanskelig å forene med mottakerens plikter til dokumentasjon og saksbehandling.
- **Ikke nødvendig.** Overføringen er en del av lovpålagte oppgaver og offentlig myndighetsutøvelse.

I stedet bør det legges vekt på klart formål, dataminimering, tilgangsstyring, logging, tydelig ansvarsdeling og god informasjon til elever og foresatte.

## Sikkerhet og de registrertes rettigheter

| Tema | Risiko | Tiltak i piloten |
| --- | --- | --- |
| Åpenhet og informasjon | Manglende eller utydelig informasjon | Informasjonstekst til elever og foresatte om overføringen: formål, mottaker, datatyper og lagringstid |
| Formålsbegrensning | Data brukes utover pilotens formål | Formålet (overføring for inntak) dokumenteres, og dataplattformen brukes bare til strukturering og kontrollert videreformidling. Ingen analyse eller sekundærbruk |
| Dataminimering | For mange eller for detaljerte opplysninger | Et konkret og begrenset sett felter. Overskytende felter filtreres bort før overføring |
| Lagringstid og sletting | Data blir liggende etter piloten | Opplysningene lagres bare midlertidig i dataplattformen og slettes etter overføringen |
| Tilgangsstyring | For bred intern tilgang | Tilgang for et fåtall navngitte roller med tjenstlig behov, med tydelig skille mellom test, drift og utvikling |
| Innsyn | Vanskelig å få innsyn | Ordinære innsynsrutiner i kommunen og fylkeskommunen, tydeliggjort i informasjonen |
| Retting og sletting | Manglende rutiner | Eksisterende rutiner i Vigilo og Vigo. Dataplattformen har ikke masterdata |
| Samtykke | Uklarhet om samtykke | Samtykke brukes ikke. Behandlingen forankres i offentlig myndighetsutøvelse |
| Konfidensialitet | Uautorisert tilgang eller lekkasje | Etablerte, sikre integrasjoner og minst mulig manuell håndtering |
| Testing | Reelle personopplysninger i test | Syntetiske eller anonymiserte data der det er mulig |
| Dokumentasjon | Vanskelig å vise etterlevelse | Vurderinger av roller, formål, datatyper og tiltak samles i pilotdokumentasjonen |

## Avgrensning av piloten

Prinsippene om formålsbegrensning, dataminimering og lagringsbegrensning kan gjøre gjenbruk og analyse av data krevende. For å følge regelverket og samtidig bygge kompetanse, anbefales en stegvis tilnærming. Fase 1 ble avgrenset slik:

- Kommunen henter de nødvendige elevopplysningene fra Vigilo og legger dem i dataplattformen.
- Bare grunnleggende funksjoner i plattformen testes: innlasting, strukturering og bearbeiding, kvalitetssikring og standardisering, og kontrollert og sporbar deling til mottaker.
- Plattformen brukes ikke til analyse, sammenstilling med andre kilder eller gjenbruk.
- Alle personopplysninger slettes fra plattformen etter overføringen.
- Fylkeskommunen får bare opplysningene som trengs for å behandle søknader om skoleplass.

Før skarpe data brukes, bør kommunen og fylkeskommunen inngå (eller kontrollere at de har) avtaler om databehandling og datautlevering, dokumentere behandlingen og hjemlene i behandlingsprotokollen, og følge opp tiltakene i tabellen over.

## Personvernkonsekvenser (DPIA)

En innledende DPIA ble gjennomført for å identifisere risikoer og avklare om en full DPIA trengs. Ett av ti kriterier slo ut: behandlingen gjelder barn og unge, en sårbar gruppe. «Stor skala» ble satt til nei under tvil, fordi antallet elever kan øke raskt, og begrepet ikke er tallfestet.

Konklusjonen er at **full DPIA ikke er nødvendig nå**, fordi piloten er sterkt avgrenset, dataene bare behandles kortvarig og slettes, og det ikke brukes ny teknologi, profilering eller automatiserte beslutninger. Behovet skal vurderes på nytt når dataflyt, tekniske mekanismer og tilgangsstyring er fastlagt, når gjenbruk, analyse eller nye funksjoner vurderes, når flere datakilder kobles til, eller når antallet registrerte øker mye.

## Risikoer (ROS)

ROS-arbeidet identifiserte risikoer for selve POC-en og for en framtidig digital prosess. Risikoene er ikke scoret.

**POC-en:**

- Reelle personopplysninger brukt i POC-en eksponeres utilsiktet. Tiltak: syntetiske data eller et svært begrenset antall.
- Oppsettet skaper svakheter i tilgangsstyringen som kan gi sårbarheter i produksjonssystemer.
- API-et i POC-en samsvarer ikke med produksjonsmiljøene (for eksempel VIGO).
- Leverandørene har ikke kapasitet til de endringene POC-en krever. Tiltak: bruke OneRoster.

**Den digitale prosessen:**

- Datautvekslingen inneholder skadevare eller kode som stopper dataflyten.
- Dataformat og struktur i ungdomsskolenes kilder passer ikke med VIGO, slik at data må rettes manuelt.
- Prosessen fra POC-en lar seg ikke gjenbruke med større datasett.
- Rutinene blir for omfattende for brukerne, som går tilbake til gamle metoder.
- Data blir liggende hos KS Digital lenger enn nødvendig.
- Overføring av karakterer og mer utfyllende informasjon gir lekkasjer. Jo mer informasjon per elev, desto høyere konsekvens.
- Duplikate elever når identifikasjonen ikke er unik, for eksempel ved flytting til en kommune med et annet system.
- Informasjonen fra enkeltskoler er ikke godt nok skilt fra hverandre.
- «Spøkelsesposter» når elever bytter skole eller kommune.
- Nye krav til datakvalitet i OAS som krever større tilpasninger.
- Planleggingsfunksjonalitet i OAS synkroniseres for tidlig.
- IST eller VIGO har ikke kapasitet til å endre løsningen før og under drift.
- Elever mister tilganger i fagsystemet før tiden ved hyppige overføringer.
- Skoler som ikke skal være med, blir likevel overført.
- Feil i unntakslister gjør at elever faller ut og først oppdages når de skal søke.
- Høy aktivitet ved skolestart er ikke godt nok utredet.
- Inntakskontoret mister oversikten i den nye prosessen.

## Hva piloten lærte

**Om prosessen.** Det lønner seg å arbeide systematisk med personvern helt fra starten. Da blir det tydelig hva som ikke er forstått eller avklart, og juristene får et bedre bilde av hvilke spørsmål som er relevante. Juridiske vurderinger avhenger av detaljer i dataflyt, brukerreise og teknisk design, som først blir synlige i et konkret case, og de tekniske løsningene påvirker igjen hvilke juridiske spørsmål som oppstår. Det krever kontinuerlig dialog og en iterativ arbeidsform. Juridiske spørsmål bør avklares konkret i hver pilot før kunnskapen utvikles til generelle veiledere.

**Om datadeling og gjenbruk.** GDPR krever konkrete vurderinger fra case til case, men maler og strukturer kan gjøre vurderingene enklere. Arbeidet bør ses i sammenheng med prosjektet Allmenningen i KS Digital, som arbeider med felles komponenter og rammer i kommunesektoren. To områder bør prioriteres: en veileder om formålsbegrensning, behandlingsgrunnlag og personvernprinsippene, og avklaringer om dataplattformen som KS Digital må følge opp.

**Om samarbeid rundt barn og unge.** Oslo kommunes innsiktsarbeid har kartlagt smertepunkter som bør tas opp i senere piloter: delefrykt, analog deling og manuelt arbeid, ulik opplæring, system- og regelverksutfordringer, uklare roller, svekket brukermedvirkning og tillit, manglende standardisering, fragmenterte systemer, høy personavhengighet og uklarhet om hva som faktisk kan deles. Prosjektgruppen foreslår også en oversikt over relevant særlovgivning, og å følge opp om nye forskriftshjemler kan gjøre datahåndteringen mer forutsigbar. Udir bør være med på det.

**Maler.** Piloten har laget en generell mal for rammedokumentet og en mal for dataflyt og datapunkter (formål, hjemmel, datatyper, roller, nødvendighet og referanser). Det anbefales å lage delvis forhåndsutfylte maler for ROS og DPIA, standardiserte avtaler (databehandleravtaler og avtaler om datautlevering) med veiledning for valg av avtaletype, og en veileder for gjenbruk til forenlige formål.
