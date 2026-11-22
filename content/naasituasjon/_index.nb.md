---
# id: auto-generert – kopierte verdier overskrives automatisk ved push
id: c3642c32-45ac-4d09-9640-e4f8cb6971ae
title: "Nåsituasjon"
linkTitle: "Nåsituasjon"
weight: 30
aliases:
 - /pilotering/pilot-1/brukerreiser/
lastmod: 2026-11-22T04:06:29+01:00
last_editor: Erik Hagen

---
Hvordan elevlisten overføres fra grunnskole til videregående i dag, og hvilke krav Novari stiller til en digital overføring til VIGO Skole.

## Overføring av elevlisten i dag

Prosessen gjelder overføring av elevdata fra grunnskole til videregående skole før overgangen mellom skolene. Formålet er å klargjøre elevene i fylkeskommunene, slik at de kan søke videregående opplæring i starten av januar.

Hovedutfordringen er at prosessen i stor grad er manuell på kommunenes side. Skoleadministrasjonen i grunnskolen laster ned filer fra fagsystemet (for eksempel Vigilo), mellomlagrer og redigerer dem lokalt på PC, og laster dem så opp i fylkeskommunens fagsystem (Vigo). Prosessen er relativt enkel, men oppleves som unødvendig, siden den burde vært automatisert. Mellomlagring av filer lokalt er også en sikkerhetsrisiko, fordi data kan komme på avveie fra filer som er lagret og ikke slettet.

![AS-IS-brukerreise for overføring av elevliste mellom grunnskole og videregående: skoleadministrasjonen laster ned fil med elevdata fra Vigilo, mellomlagrer og redigerer den lokalt og laster den opp i Vigo Skole, og inntakskontoret flytter filene videre til Vigo. Til høyre: omfang, hvordan prosessen oppleves, varianter og hva som er viktig](as-is-overforing-elevliste.png)

## Krav til en digital overføring

Novari har, etter samtaler med fagpersonene sine, beskrevet krav til de tre overføringene av data om avgangselever fra ungdomsskolenes skoleadministrative systemer (SAS) til VIGO Skole. Novari mener overføringen helst bør håndteres i ungdomsskolenes SAS. Kravene er:

- **Komplette datasett.** En overføring skal alltid gjelde alle avgangselevene (liste eller karakterdata), ikke enkeltelever. Ellers vet ikke fylkeskommunen når overføringen er komplett, og ungdomsskolen vet ikke om den er akseptert.
- **Rett feil i kilden.** Feil og advarsler skal rettes i ungdomsskolens SAS, slik at man unngår følgefeil. Dette følger av prinsippet om riktighet (GDPR art. 5 nr. 1 d), innebygd personvern (art. 25) og retten til retting (art. 16).
- **Maskinporten.** Et nytt API mot VIGO Skole bør bruke Maskinporten for maskin-til-maskin-autentisering. Bare kommunene i den aktuelle fylkeskommunen får tilgang, styrt med organisasjonsnummer. Kommunene kan delegere tilgangen til tredjeparter, for eksempel KS Digital eller en leverandør som Altinn-systembruker. I dag styres tilgangen med VIGO-skolenummer.
- **Rollestyrt tilgang.** I dag oppnevner fylkeskommunen superbrukere på ungdomsskolene som laster opp filene. Med API bør dette erstattes av rollestyrt tilgang i SAS.
- **Bare feilfrie datasett godtas.** Advarsler (for eksempel manglende fag eller for mange valgfag) kan godtas, men bør rettes. Feil kan gi feil poenggrunnlag, slik at elever feilaktig ikke kommer inn eller får tilbud.
- **Løpende validering.** SAS bør validere løpende mot reglene i Utdanningsdirektoratets føringsskriv og reglene for fødselsnummer i registreringshåndboken, eller i det minste ved innsending.
- **Tydelig tilbakemelding.** Feil og advarsler skal meldes samlet og tydelig til den som sendte inn, med status akseptert, feil eller advarsler. Svaret fra API-et beskriver feil per elev, men ikke den maskinlesbare regelen som feilet.
- **Rask retting.** Fristene er ofte korte (3–7 dager), særlig for sluttkarakterer om sommeren. Det må være mulig å rette og sende inn på nytt med en gang.
- **Ingen innsending etter fristen.** Endringer som kommer etter poengberegning eller innleveringsfrist, skal ikke sendes via API. SAS bør sperre innsending etter fristen, eller varsle tydelig. Fylkeskommunen behandler sene endringer, som klager, manuelt og med logging direkte i VIGO.

Skriftlige eksamenskarakterer henter ungdomsskolen fra Udirs prøveadministrasjonssystem (PAS), og de skal være registrert i skolesystemet før den endelige datapakken leveres til VIGO.
