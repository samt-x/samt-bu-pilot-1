---
title: "Veikart"
linkTitle: "Veikart"
weight: 70

---

{{< i-arbeid >}}

Veien videre er fase 2: en videreføring på 12 uker. Planen er et utkast (versjon 0.3, 29. september 2026) og ikke godkjent. Foreslått prosjekteier er KS Digital. Arbeidspakker, milepæler og tidsplan står under [Oppgaver og framdrift](/pilotering/pilot-1/oppgaver-og-framdrift/#plan-for-fase-2).

## Kjerneidé

Drømmereise → arbeidsprosess → ansvar → informasjon og regler → nasjonal arkitektur og målarkitektur → prototype → videreføring.

Fase 2 bygger på POC-en fra fase 1, men POC-en er ikke en besluttet målarkitektur. Den bredere drømmereisen styrer retningen, mens prototypen tester et smalt, målbart utsnitt. Piloten skal verken reduseres til filkonvertering eller love en komplett omlegging av sektoren på tre måneder.

## Nasjonal arkitektur som premiss

Nasjonal arkitektur for digital samhandling skal være et styrende vurderingsgrunnlag. Piloten skal:

- beskrive juridisk, organisatorisk, semantisk og teknisk nivå i målarkitekturen
- vurdere autoritative kilder, datastyring, tilgang, sikkerhet, logging og forvaltningsansvar
- vurdere delingsmønstre som API og hendelser, dataprodukt, filutveksling i en overgang og datarom, uten å velge teknologi på forhånd
- vurdere relevante fellesressurser og standarder, blant annet Maskinporten, Altinn Autorisasjon, Felles datakatalog, begrepskatalogen, API-katalogen og Referansekatalogen
- dokumentere hvilke deler av POC-en som kan standardiseres og gjenbrukes på tvers av kommuner, fylkeskommuner og leverandører

Piloten skal også se på European Learning Model og eventuelle utvidelser av OneRoster eller FINT for overføring av karakterer, og se hen til andre piloter med tilsvarende behov, særlig [Pilot 4](/pilotering/pilot-4/). Rollen til data.norge.no og leverandørene skal avklares.

## Leveranser

| Id | Leveranse | Minimum for godkjenning |
|---|---|---|
| L1 | Brukerreise (AS-IS) | Dagens brukerreise er beskrevet |
| L2 | Ønsket brukerreise | Ønsket situasjon, aktørperspektiver og kritiske øyeblikk, godkjent av kommune og fylkeskommune |
| L3 | Arbeidsprosess og ansvar | Aktiviteter, beslutningspunkter, dataansvar, retting og avvik er beskrevet og avklart med leverandørene |
| L4 | Informasjonsmodell v1 | Avtalte dataelementer, begreper, relasjoner, kodeverk, kilder og kvalitetskrav |
| L5 | Regelsett v1 | Prioriterte regler er entydige, sporbare til kilde og kan testes maskinelt |
| L6 | Nasjonal arkitektur og målarkitektur | Arkitekturvurdering, kapabilitetskart, prinsipper, delingsmønster, tillit og tilgang, dataflyt og ansvar |
| L7 | Løsningsdesign | Første steg og langsiktig retning: grensesnitt, hendelser, feilflyt og avhengigheter |
| L8 | Prototype eller demonstrator | Et godkjent scenario kjøres ende til ende med testdata og dokumentert resultat |
| L9 | Videreføringsplan | Systemendringer, leverandørbehov, kostnadsdrivere, ansvar, veikart og beslutninger |
| L10 | Erfarings- og gevinstnotat | Baseline, testresultater, læring, gjenbruk og anbefaling for neste fase |

## Avgrensning

Innenfor de 12 ukene:

- overgangen fra ungdomsskole til videregående opplæring
- relevante data i VIGO 1, 2 og 3, med endelig feltavgrensning i uke 2–3
- drømmereise, arbeidsprosess, ansvar, informasjonsmodell, kodeverk og valideringsregler
- nasjonal arkitektur, målarkitektur, løsningsdesign og et avgrenset delingsmønster
- prototype med syntetiske eller dokumentert lovlige testdata, etter beslutning ved P2
- avhengigheter til skoleadministrative systemer, VIGO, Feide og relevante nasjonale registre og tjenester

Utenfor:

- full produksjonssetting i alle kommuner, fylkeskommuner og leverandørsystemer
- fullstendig digitalisering av alle føringsregler, klager og unntak
- endelig valg av dataromsteknologi før behov og delingsmønster er validert
- endelig forvaltningsorganisasjon og finansieringsmodell, utover et beslutningsklart forslag
- andre overganger, utover en dokumentert gjenbruksanalyse

## Mål og måling

| Mål | Nøkkelresultater |
|---|---|
| O1 En sammenhengende og trygg overgang | Drømmereisen godkjennes av kommune, fylkeskommune og berørte fagmiljøer. Framtidig prosess og RACI dekker registrering, validering, retting, deling, mottak og bruk. Baseline for manuelle trinn, feil og ledetid er dokumentert og sammenlignet med testresultatet. |
| O2 Felles informasjon og maskinlesbare regler | Informasjonsmodell v1 dekker de avtalte VIGO 1-, 2- og 3-opplysningene. Et prioritert regelsett er sporbart til kilde og kan testes maskinelt. Demonstratoren viser både godkjent og avvist datasett, med forståelige avvik og ansvar for retting. |
| O3 Nasjonal arkitektur gir gjenbrukbar retning | Relevante prinsipper, kapabiliteter, fellesressurser og standarder er vurdert. En målarkitekturbeslutning beskriver de fire nivåene, autoritative kilder, delingsmønster og plattformrolle. Gjenbruk er vurdert mot minst to andre kommuner, leverandørvarianter eller SAMT-BU-caser. |
| O4 Beslutningsklart grunnlag for videreføring | Prototype eller dokumentert alternativ er gjennomført etter P2. Systemendringer, leverandørbehov, kostnadsdrivere, ansvar og forvaltning er beskrevet. P3 gir en tydelig anbefaling om produktisering, skalering, ny utprøving eller stopp. |

Piloten skal ikke påstå realiserte gevinster uten baseline. Gevinsthypotesene er:

| Hypotese | Tidlig indikator | Målemetode |
|---|---|---|
| Færre datafeil | Andel poster som feiler validering | Baseline fra dagens overføringer sammenlignes med testresultatet |
| Mindre manuelt arbeid | Antall manuelle trinn og rettinger | Prosesskart og tidsmåling eller stikkprøver |
| Raskere og tryggere flyt | Ledetid og antall usikre overleveringer | Tidsstempler og hendelseslogg i demonstratoren |
| Bedre gjenbruk | Andel modell-, regel- og arkitekturkomponenter som kan brukes videre | Faglig gjenbruksanalyse mot minst to nye sammenhenger |

## Risiko

| Risiko | Vurdering | Tiltak |
|---|---|---|
| Endringer rekker ikke inn i de skoleadministrative systemene | Høy sannsynlighet, middels konsekvens | Testadapter eller demonstrator, og konkret leverandørplan |
| Uklart eierskap og beslutningsmyndighet | Middels, høy | Avklar prosjekteier, prosesseier og beslutningsforum ved P0 |
| For bredt omfang | Høy, høy | Lås scenario og datafelt ved P1 og P2 |
| Uenighet om begreper, kodeverk eller regler | Middels, høy | Kildesporing, versjonering og faglig beslutningsforum |
| Juridiske eller sikkerhetsmessige forhold er ikke avklart | Middels, høy | Dokumentert gjennomgang før P2, og testdata |
| POC-arkitekturen blir ukritisk gjort til målarkitektur | Middels, høy | AP3 vurderer alternative delingsmønstre og skiller samhandlingskontrakt fra implementasjon |
| Teknologivalg styrer behovet | Middels, middels | Beslutningskriterier før EDC, Simpl eller andre komponenter vurderes |
| Manglende kapasitet hos nøkkelpersoner | Middels, høy | Navngitt bemanning og minimumsallokering før P0 |
| Prototypen blir ikke gjenbrukbar | Middels, middels | Leverandøruavhengig modell, dokumentert arkitekturbeslutning og gjenbruksanalyse |
| Gevinster kan ikke dokumenteres | Middels, middels | Baseline og måleplan i uke 1 |

## Åpne spørsmål ved oppstart

- Hvem er formell prosjekteier, prosesseier og framtidig forvalter?
- Hvilke dataelementer i VIGO 1, 2 og 3 inngår i første fase?
- Hvilke deler av føringsskrivet kan og bør uttrykkes maskinelt?
- Hvilket delingsmønster løser behovet best, og hvilken rolle skal KS Digitals dataplattform ha i målarkitekturen?
- Hvilke nasjonale fellesressurser og standarder skal brukes, og hvilke må videreutvikles?
- Hvordan håndteres klager, avvik og unntak i første fase?
- Hvem finansierer og forvalter endringer i leverandørsystemene og VIGO etter piloten?

Leverandørene bør kobles på tidlig for å avklare validering, grensesnitt, endringsløp og prototype. Sektoren må samtidig eie behov, informasjonsmodell, regler og målarkitektur.
