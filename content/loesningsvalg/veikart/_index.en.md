---
title: "Roadmap"
linkTitle: "Roadmap"
weight: 70

---

{{< i-arbeid >}}

The way forward is phase 2: a 12-week continuation. The plan is a draft (version 0.3, 29 September 2026) and has not been approved. The proposed project owner is KS Digital. Work packages, milestones and schedule are under [Tasks and progress](/en/pilotering/pilot-1/oppgaver-og-framdrift/#plan-for-phase-2).

## Core idea

Dream journey → work process → responsibility → information and rules → national architecture and target architecture → prototype → continuation.

Phase 2 builds on the POC from phase 1, but the POC is not an agreed target architecture. The broader dream journey sets the direction, while the prototype tests a narrow, measurable slice. The pilot shall neither be reduced to file conversion nor promise a complete overhaul of the sector in three months.

## National architecture as a premise

The national architecture for digital interoperability shall be a governing basis for assessment. The pilot shall:

- describe the legal, organisational, semantic and technical levels of the target architecture
- assess authoritative sources, data governance, access, security, logging and management responsibility
- assess sharing patterns such as APIs and events, data products, file exchange during a transition period and data spaces, without choosing technology in advance
- assess relevant shared resources and standards, including Maskinporten, Altinn Authorisation, the National Data Catalogue, the concept catalogue, the API catalogue and the Reference Catalogue
- document which parts of the POC can be standardised and reused across municipalities, county authorities and suppliers

The pilot shall also look at the European Learning Model and any extensions of OneRoster or FINT for the transfer of grades, and take account of other pilots with similar needs, especially [Pilot 4](/en/pilotering/pilot-4/). The role of data.norge.no and the suppliers shall be clarified.

## Deliverables

| Id | Deliverable | Minimum for approval |
|---|---|---|
| L1 | User journey (AS-IS) | The current user journey is described |
| L2 | Desired user journey | Desired situation, actor perspectives and critical moments, approved by the municipality and the county authority |
| L3 | Work process and responsibility | Activities, decision points, data responsibility, correction and deviations are described and clarified with the suppliers |
| L4 | Information model v1 | Agreed data elements, concepts, relationships, code lists, sources and quality requirements |
| L5 | Rule set v1 | Prioritised rules are unambiguous, traceable to source and can be tested by machine |
| L6 | National architecture and target architecture | Architecture assessment, capability map, principles, sharing pattern, trust and access, data flow and responsibility |
| L7 | Solution design | First step and long-term direction: interfaces, events, error flow and dependencies |
| L8 | Prototype or demonstrator | An approved scenario is run end to end with test data and a documented result |
| L9 | Continuation plan | System changes, supplier needs, cost drivers, responsibility, roadmap and decisions |
| L10 | Lessons-learned and benefits note | Baseline, test results, learning, reuse and recommendation for the next phase |

## Delimitation

Within the 12 weeks:

- the transition from lower secondary school to upper secondary education
- relevant data in VIGO 1, 2 and 3, with final delimitation of fields in weeks 2–3
- dream journey, work process, responsibility, information model, code lists and validation rules
- national architecture, target architecture, solution design and a bounded sharing pattern
- prototype with synthetic or documented lawful test data, subject to a decision at P2
- dependencies on school administration systems, VIGO, Feide and relevant national registers and services

Outside:

- full deployment to production in all municipalities, county authorities and supplier systems
- complete digitalisation of all grading rules, appeals and exceptions
- final choice of data space technology before the need and sharing pattern have been validated
- final management organisation and funding model, beyond a proposal ready for decision
- other transitions, beyond a documented reuse analysis

## Objectives and measurement

| Objective | Key results |
|---|---|
| O1 A seamless and secure transition | The dream journey is approved by the municipality, the county authority and the professional communities concerned. The future process and RACI cover registration, validation, correction, sharing, receipt and use. A baseline for manual steps, errors and lead time is documented and compared with the test result. |
| O2 Common information and machine-readable rules | Information model v1 covers the agreed VIGO 1, 2 and 3 information. A prioritised rule set is traceable to source and can be tested by machine. The demonstrator shows both an approved and a rejected data set, with understandable deviations and responsibility for correction. |
| O3 National architecture provides reusable direction | Relevant principles, capabilities, shared resources and standards have been assessed. A target architecture decision describes the four levels, authoritative sources, sharing pattern and platform role. Reuse has been assessed against at least two other municipalities, supplier variants or SAMT-BU cases. |
| O4 A basis for continuation ready for decision | A prototype or documented alternative has been carried out after P2. System changes, supplier needs, cost drivers, responsibility and management are described. P3 gives a clear recommendation on productisation, scaling, new testing or stopping. |

The pilot shall not claim realised benefits without a baseline. The benefit hypotheses are:

| Hypothesis | Early indicator | Measurement method |
|---|---|---|
| Fewer data errors | Proportion of records that fail validation | Baseline from current transfers is compared with the test result |
| Less manual work | Number of manual steps and corrections | Process map and time measurement or spot checks |
| Faster and more secure flow | Lead time and number of insecure handovers | Timestamps and event log in the demonstrator |
| Better reuse | Proportion of model, rule and architecture components that can be reused | Professional reuse analysis against at least two new contexts |

## Risk

| Risk | Assessment | Measures |
|---|---|---|
| Changes cannot be made in the school administration systems in time | High probability, medium consequence | Test adapter or demonstrator, and a concrete supplier plan |
| Unclear ownership and decision-making authority | Medium, high | Clarify project owner, process owner and decision forum at P0 |
| Scope too broad | High, high | Lock scenario and data fields at P1 and P2 |
| Disagreement on concepts, code lists or rules | Medium, high | Source tracing, versioning and a professional decision forum |
| Legal or security matters have not been clarified | Medium, high | Documented review before P2, and test data |
| The POC architecture is uncritically turned into the target architecture | Medium, high | AP3 assesses alternative sharing patterns and separates the interoperability contract from the implementation |
| Choice of technology drives the need | Medium, medium | Decision criteria before EDC, Simpl or other components are considered |
| Lack of capacity among key people | Medium, high | Named staffing and minimum allocation before P0 |
| The prototype is not reusable | Medium, medium | Supplier-independent model, documented architecture decision and reuse analysis |
| Benefits cannot be documented | Medium, medium | Baseline and measurement plan in week 1 |

## Open questions at start-up

- Who is the formal project owner, process owner and future manager?
- Which data elements in VIGO 1, 2 and 3 are included in the first phase?
- Which parts of Udir's grading guidelines (føringsskriv) can and should be expressed in machine-readable form?
- Which sharing pattern best meets the need, and what role should KS Digital's data platform have in the target architecture?
- Which national shared resources and standards shall be used, and which need further development?
- How are appeals, deviations and exceptions handled in the first phase?
- Who funds and manages changes to the supplier systems and VIGO after the pilot?

The suppliers should be involved early to clarify validation, interfaces, change processes and the prototype. At the same time, the sector must own the need, information model, rules and target architecture.
