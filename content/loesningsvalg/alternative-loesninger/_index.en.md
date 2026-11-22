---
id: c4e98cfc-efc5-441d-9c63-c88cd22a6324
title: "Alternative solutions"
linkTitle: "Alternative solutions"
weight: 10

---
The architecture working group discussed early on whether the pilot should build an MVP or a POC. It recommended a POC in order to get started quickly, show how the actual problem can be solved, and at the same time illustrate the room for further use of data. The aim was functionality and learning, not a finished solution. The proposal from sprint 1 is in [Working note sprint 1](arbeidsnotat-sprint-1/).

Three alternatives were considered. The lessons-learned report points out that the alternatives were not evaluated systematically, and that this created unnecessary uncertainty (see [Results and the way forward](/en/pilotering/pilot-1/resultater-og-veien-videre/)).

## Alternative 1: Common data management on KS Digital's service platform

Data is retrieved from the municipality's school administration system and placed in KS Digital's data platform, as an intermediate layer between the municipality and the county authority. There the data is structured according to the FINT model, quality-assured and shared on to Vigo.

- The infrastructure already exists, so the pilot could get started quickly.
- Provides automated data flow and a basis for a more data-driven everyday life.
- Facilitates standardisation, sharing and reuse of data for municipalities and county authorities, also in other areas such as health and care, planning and building, and welfare.

This alternative was tested in the POC, see [Chosen solution now](/en/pilotering/pilot-1/loesningsvalg/valgt-loesning-naa/).

## Alternative 2: Direct integration between the municipality's systems and FINT

The municipality's school administration systems (SAS) communicate directly with FINT and Vigo Skole, without a common intermediate layer. The alternative builds on existing frameworks and integration patterns in the sector. It was described as a parallel track with test data, but was not developed further in phase 1.

## Alternative 3: Federated data sharing with an emphasis on privacy

This proposal builds on the principles in NOU 2024: 14 «Med lov skal data deles» (By law, data shall be shared), on making public data available for reuse. It requires that:

- services, data sets and information models can be discovered and used by machines
- data is only exchanged where there is a mandate
- data sovereignty is respected: the data is owned by the source systems, which also control access
- what has been exchanged between whom and when is tracked
- a trust framework verifies that the actors are who they claim to be

The proposal reuses existing standards and open source software for secure, standardised and federated data exchange. Because the EU has worked on this for a long time and created regulations that will sooner or later apply in Norway through the EEA Agreement, the proposal recommends a Norwegian education data space based on [Simpl-Open](/en/innsikt/eu-relatert/data-spaces/loesninger/simpl/). Data is retrieved from Vigilo and sent via Vigo Skole to Vigo, with Vigo's code lists, the National Data Catalogue (data.norge.no) and the National Population Register as shared resources.

In the plan for phase 2, the choice of technology is left open: EDC or Simpl can be considered if they meet the need, but are not goals in themselves (see [Roadmap](/en/pilotering/pilot-1/loesningsvalg/veikart/)).
