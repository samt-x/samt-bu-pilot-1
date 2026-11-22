---
title: "Alternative løsninger"
linkTitle: "Alternative løsninger"
weight: 10

---
Arbeidsgruppen for arkitektur diskuterte tidlig om piloten skulle lage en MVP eller en POC. Den anbefalte en POC for å komme raskt i gang, vise hvordan det faktiske problemet kan løses, og samtidig illustrere mulighetsrommet for videre bruk av data. Målet var funksjonalitet og læring, ikke en ferdig løsning. Forslaget fra sprint 1 står i [Arbeidsnotat sprint 1](arbeidsnotat-sprint-1/).

Tre alternativer ble vurdert. Erfaringsrapporten peker på at alternativene ikke ble evaluert systematisk, og at det skapte unødige uklarheter (se [Resultater og veien videre](/pilotering/pilot-1/resultater-og-veien-videre/)).

## Alternativ 1: Felles dataforvaltning på KS Digitals tjenesteplattform

Data hentes fra kommunens skoleadministrative system og legges i KS Digitals dataplattform, som et mellomlag mellom kommune og fylkeskommune. Der struktureres dataene etter FINT-modellen, kvalitetssikres og deles videre til Vigo.

- Infrastrukturen finnes allerede, så piloten kunne komme raskt i gang.
- Gir automatisert dataflyt og grunnlag for en mer datadrevet hverdag.
- Legger til rette for standardisering, deling og gjenbruk av data for kommuner og fylkeskommuner, også på andre fagområder som helse og omsorg, plan og bygg og velferd.

Dette alternativet ble prøvd ut i POC-en, se [Valgt løsning nå](/pilotering/pilot-1/loesningsvalg/valgt-loesning-naa/).

## Alternativ 2: Direkte integrasjon mellom kommunens systemer og FINT

Kommunens skoleadministrative systemer (SAS) kommuniserer direkte med FINT og Vigo Skole, uten et felles mellomlag. Alternativet bygger på eksisterende rammeverk og integrasjonsmønstre i sektoren. Det ble beskrevet som et parallelt løp med testdata, men ikke utviklet videre i fase 1.

## Alternativ 3: Føderert datadeling med vekt på personvern

Dette forslaget bygger på prinsippene i NOU 2024: 14 «Med lov skal data deles», om å gjøre offentlige data tilgjengelige for videre bruk. Det krever at:

- tjenester, datasett og informasjonsmodeller kan oppdages og brukes maskinelt
- data bare utveksles der det finnes mandat
- datasuverenitet overholdes: dataene eies av kildesystemene, som også styrer tilgangen
- det spores hva som er utvekslet mellom hvem og når
- et tillitsrammeverk verifiserer at aktørene er dem de utgir seg for å være

Forslaget gjenbruker eksisterende standarder og åpen kildekode for sikker, standardisert og føderert datautveksling. Fordi EU har arbeidet med dette lenge og laget regelverk som før eller siden vil gjelde i Norge gjennom EØS-avtalen, anbefaler forslaget et norsk opplæringsdatarom (education data space) basert på [Simpl-Open](/innsikt/eu-relatert/data-spaces/loesninger/simpl/). Data hentes fra Vigilo og sendes via Vigo Skole til Vigo, med Vigos kodeverk, Felles datakatalog (data.norge.no) og Folkeregisteret som felles ressurser.

I planen for fase 2 er teknologivalget holdt åpent: EDC eller Simpl kan vurderes dersom de svarer på behovet, men er ikke mål i seg selv (se [Veikart](/pilotering/pilot-1/loesningsvalg/veikart/)).
