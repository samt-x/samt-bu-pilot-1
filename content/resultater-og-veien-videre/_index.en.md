---
title: "Results and the way forward"
linkTitle: "Results and the way forward"
weight: 90

---
Phase 1 was carried out from February to April 2026 and concluded with a demo on 30 April. The sources are the closing presentation and the lessons-learned report (version 1.0, 24 April 2026).

## Main results

- **A running POC** transfers the pupil list from Vigilo via KS Digital's data platform, transformed to FINT v4, to a simulated receiver for Vigo Skole. See [Chosen solution now](/en/pilotering/pilot-1/loesningsvalg/valgt-loesning-naa/).
- **The solution delivers benefits** in the form of greater efficiency and better control of information security and privacy. The findings from Bergen have been quality-assured in Arendal, Bykle and Vestland county authority.
- **Legal clarification:** the November transfer has a legal basis in the Education Act (opplæringslova) section 9-5, the municipality and the county authority are separate controllers, and consent is not the right basis. See [Legal matters](/en/pilotering/pilot-1/juridiske-forhold/).
- **Information models:** a Norwegian profile of OneRoster, a conceptual model for the transfer and a start on a person model in SHACL. See [Information architecture](/en/pilotering/pilot-1/loesningsvalg/informasjonsarkitektur/).
- **An architecture council** with Novari, KS Digital, KS and Digdir was established. It has created overall frameworks for architecture, a template for architecture assessments with guidance, and started on a description of what the intermediate layer is.

## Positive lessons learned

- Having the end users involved from the start made it easier to keep the focus on benefits.
- Many involved partners meant that the problems were seen in new ways.
- Having lawyers in the pilot group from the start was a great advantage. Law, too, can take an agile approach.
- Starting with something concrete early on uncovered unforeseen interoperability challenges.
- The sector already has good standardised information models (FINT and OneRoster).

## What was challenging

- Too little planning in advance led to more discussions and more fumbling than necessary.
- Perceptions of reality and understanding of the problem diverged. What some saw as a major problem was a non-problem for others.
- There were differing views on how the problem should be solved, and a lot of time went into architecture choices.
- Access to data from the municipalities' line-of-business systems can become costly. The suppliers charge per municipality to unlock data, and the agreements do not take sharing into account. The total comes to many millions of kroner for the country as a whole.

## Experiences and measures

The lessons-learned report goes through each phase and proposes measures for the project's handbook for pilots (see [Working model](/en/styring/arbeidsmodell/)).

| Phase | Experience | Measures |
|---|---|---|
| Choosing a pilot | The basis for the choice was too thin, the pain points unclear and the objectives not sufficiently anchored. There was no clear case owner | Update the template for case descriptions with case owner and objectives. Send out case descriptions and invite to a workshop in good time. Appoint representatives for municipalities and county authorities |
| Start-up | Too little time between choice of pilot, planning workshop and start-up. The benefit potential was unclear, and there were differing opinions on whether the POC should provide learning or a runnable service | More time for planning. Define the objectives early, with a dedicated OKR session once the team is in place. Clear separation between the tasks of the pilot and those of the core team, and escalation routes |
| Dream journey | Dream journeys take longer to create. A shared dream journey can reveal differing understandings of the problem | Obtain resources for dream journeys or scale down. AS-IS and TO-BE as separate steps in the plan |
| Choosing POC or MVP | Unclear whether the pilot should create a POC or an MVP. The choice to run the POC at KS Digital was not sufficiently anchored | As for start-up |
| Building it | A high pace in two-week sprints worked. Someone is needed to hold the pilot together. The tasks were too large and lacked a clear «done». Too little collaboration across working groups. Engagement was hard to sustain towards the end. The alternatives were not evaluated, which created uncertainty | Three-week sprints with stand-ups every other day. A dedicated sub-project manager. Vulnerability analysis early on. A common place for documentation (docs.samt-bu.no). Template for architecture and solution descriptions as a basis for decisions. Forums that take discussions lifted out of the pilot (architecture forum). Benefit assessment as a step in the template |
| Evaluation | OKRs were not established, but a high-level benefit analysis was carried out | |
| Communication | The pilot was presented at eKommune, among other places | Write a story about the pilot |

Other experiences:

- It is difficult to get data out of the municipalities' line-of-business systems, even when it is stated in the tender documents. Bergen has experienced this.
- Communication tools and document management, such as Teams, are difficult to get working across organisations.
- The partners need to understand the importance of time recording and how the co-funding rules work.
- Those who worked on information models spent a lot of time familiarising themselves with the domain and existing standards. Someone with a good overview of the domain would have given better speed from the start.

## The way forward

The closing session pointed to three possible paths: develop the POC further into a runnable MVP, extend it to also transfer results from primary and lower secondary school (grades), or extend it to more municipalities. However, it takes time to specify requirements for and develop an API in Vigo Skole, and the other cases may provide important input.

Technical development was therefore paused until the end of August 2026. Starting then still makes it possible to run an MVP on the transfer before Christmas and a POC on the data transferred after New Year 2027. The plan for phase 2 is under [Roadmap](/en/pilotering/pilot-1/loesningsvalg/veikart/).
