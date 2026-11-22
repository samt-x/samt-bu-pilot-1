---
id: 8dcb24a7-2c3a-4bb5-a111-e362bc93ad23
title: "Oppgaver og framdrift"
linkTitle: "Oppgaver og framdrift"
weight: 15
lastmod: 2026-11-20T01:51:08+01:00
last_editor: Erik Hagen

---

Oppgavene i pilot 1 ligger som issues i [samt-bu-pilot-1](https://github.com/samt-x/samt-bu-pilot-1/issues) og på brettet [SAMT-BU Pilot 1 – Overgang ungdomsskole videregående](https://github.com/orgs/samt-x/projects/1) (Project 1). Denne siden viser hvor arbeidet står.

| Visning | Viser |
|---|---|
| [Board](https://github.com/orgs/samt-x/projects/1/views/1) | Alle oppgaver etter status |
| [By responsible](https://github.com/orgs/samt-x/projects/1/views/2) | Oppgavene gruppert etter hvem som har ansvaret |
| [Open tasks](https://github.com/orgs/samt-x/projects/1/views/3) | Åpne oppgaver i en tabell |
| [My tasks](https://github.com/orgs/samt-x/projects/1/views/5) | Dine oppgaver (krever innlogging) |
| [Timeline](https://github.com/orgs/samt-x/projects/1/views/4) | GitHubs egen tidslinje, uten avhengigheter |

## Status

Fase 1 ble avsluttet med en demo 30. april 2026. Den tekniske utviklingen ble satt på pause til slutten av august. Fase 2 er planlagt som en videreføring på 12 uker, men planen er ikke godkjent og oppstartsdatoen er ikke satt.

## Opprinnelig plan for fase 1

Fase 1 gikk fra februar til april 2026, i sprinter på to uker. Hver sprint startet med et planleggingsmøte og sluttet med en demo. Arbeidet var delt i sju arbeidspakker:

1. Drømmereise (kjerneteamet)
2. Kjørende POC eller MVP
3. Informasjonsmodell
4. Arkitektur
5. Oversikt over juridisk mulighetsrom
6. Juridisk rammeverk
7. Erfaringsrapport (kjerneteamet)

Tre milepæler styrte arbeidet: når det var avklart hvilke informasjonselementer piloten skulle inneholde, når ROS-analysen var gjennomført, og når det var besluttet hvordan piloten skulle gå videre.

![Overordnet plan for fase 1, uke 6–17 i 2026: drømmereise i uke 6–7, kjørende POC, arkitektur og informasjonsmodell gjennom hele perioden, juridiske begrensninger og juridisk ramme, og løsningsmønstre og erfaringsrapport mot slutten. Fem sprinter med planlegging og demo, ROS i uke 9 og beslutning om veien videre i uke 15](overordnet-plan-fase-1.png)

## Plan for fase 2

{{< i-arbeid >}}

Planen for fase 2 er et utkast (versjon 0.3, 29. september 2026) og ikke godkjent. Den bygger på et arbeidsdokument fra samlingen på Gardermoen 30. august 2026.

Arbeidet er delt i to spor som utvikles i sammenheng. Spor A (AP1–AP2) gjelder tjeneste, informasjon og regler. Spor B (AP3–AP4) gjelder arkitektur og utprøving. AP0, AP5, juss, personvern, sikkerhet, leverandørdialog og erfaringsdeling går på tvers.

| Arbeidspakke | Innhold | Leveranser |
|---|---|---|
| AP0 Mobilisering og styring | Mandat, omfang, aktørkart, kilder, baseline, beslutnings- og risikologg | Oppstartsnotat, måleplan og P0 |
| AP1 Drømmereise, prosess og ansvar | Ønsket brukeropplevelse, framtidig prosess, roller, RACI, avvik og unntak | L1, L2 og L3 |
| AP2 Informasjon, kodeverk og regler | Dataelementer, begreper, kilder, kvalitetskrav og maskinlesbar validering | L4 og L5 |
| AP3 Nasjonal arkitektur og målarkitektur | Prinsipper, kapabiliteter, fellesressurser, de fire samhandlingsnivåene, delingsmønster og arkitekturbeslutninger | L6, kapabilitetskart og beslutningsgrunnlag til P2 |
| AP4 Løsningsdesign og prototype | Grensesnitt, sikkerhet, testdata, validering, feilflyt, logging og demonstrasjon | L7 og L8 |
| AP5 Gevinst, læring og videreføring | Måling, gjenbruk, leverandørplan, kostnadsdrivere, forvaltning og veikart | L9, L10 og P3 |

Leveransene L1–L10 er beskrevet under [Veikart](/pilotering/pilot-1/loesningsvalg/veikart/).

### Milepæler og beslutningsporter

| Tidspunkt | Milepæl eller port | Beslutning eller resultat |
|---|---|---|
| Uke 1 | P0 Oppstart | Eier, prosjektleder, mandat, ressurser, omfang og kilder er bekreftet |
| Uke 7 | M1 Drømmereise | Drømmereisen er godkjent av kommune, fylkeskommune og berørte fagmiljøer |
| Uke 7 | P1 Modellgrunnlag | Prosess, ansvar, data, kodeverk og prioriterte regler er omforent |
| Uke 10 | P2 Arkitektur og prototype | Vurderingen mot nasjonal arkitektur, målarkitektur, delingsmønster, sikkerhet, scenario, testdata og kapasitet er godkjent |
| Uke 12 | M2 Demonstrasjon | Et avgrenset scenario er demonstrert ende til ende med testdata og dokumentert måling |
| Uke 12 | P3 Videreføring | Resultater, gevinster, kostnadsdrivere, avhengigheter og forvaltning er belyst, og neste fase besluttes |

Prototypen bygges bare dersom P2 godkjenner scenario, testdata, sikkerhet, løsningsdesign, kapasitet og læringsmål. Detaljert utvikling starter først etter P2.

### Overordnet plan

| Arbeidspakke | Uke 1 | Uke 2 | Uke 3–5 | Uke 4–7 | Uke 7–10 | Uke 11–12 | Port |
|---|---|---|---|---|---|---|---|
| AP0 Mobilisering og styring | Aktiv | | | | | | P0 |
| AP1 Drømmereise, prosess og ansvar | Start | AS-IS-brukerreise | AS-IS-brukerreise | Drømmereise | | | M1, P1 |
| AP2 Informasjon, kodeverk og regler | | Start | | Modell og regelsett | | | P1 |
| AP3 Nasjonal arkitektur og målarkitektur | | | | Analyse | Målarkitektur og delingsmønster | | P2 |
| AP4 Løsningsdesign og prototype | | | | | Design | Bygg, test og demo | M2 |
| AP5 Gevinst, læring og videreføring | Baseline | | | | Måling | Sammenstilling | P3 |
| Juss, sikkerhet, leverandørdialog og erfaringsdeling | Start | Løpende | Løpende | Kontroll | Løpende | Avslutning | P0–P3 |

Arbeidet koordineres ukentlig i kjernegruppen, med fag- og arkitekturverksteder ved behov.

## Tidslinje

Alle oppgavene på brettet, med pilene for hvilke oppgaver som venter på hverandre. Det som har skjedd, er mørkt. Datoer som mangler, er beregnet og stiplet. Figuren lages fra brettet hver time. Slik leser du den, og slik får en oppgave med: se [Tidslinje](/prosjektleveranser/loesninger/samhandlingsplattform/oppgavestyring/tidslinje/) i oppgavestyringen.

{{< inline-svg "project-1-nb.svg" "/prosjektleveranser/loesninger/samhandlingsplattform/oppgavestyring/tidslinje" >}}
