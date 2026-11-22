---
id: 8dcb24a7-2c3a-4bb5-a111-e362bc93ad23
title: "Tasks and progress"
linkTitle: "Tasks and progress"
weight: 15
lastmod: 2026-11-20T01:51:08+01:00
last_editor: Erik Hagen

---

The tasks of pilot 1 are issues in [samt-bu-pilot-1](https://github.com/samt-x/samt-bu-pilot-1/issues) and on the board [SAMT-BU Pilot 1 – Overgang ungdomsskole videregående](https://github.com/orgs/samt-x/projects/1) (Project 1). This page shows where the work stands.

| View | Shows |
|---|---|
| [Board](https://github.com/orgs/samt-x/projects/1/views/1) | All tasks by status |
| [By responsible](https://github.com/orgs/samt-x/projects/1/views/2) | The tasks grouped by who is responsible |
| [Open tasks](https://github.com/orgs/samt-x/projects/1/views/3) | Open tasks in a table |
| [My tasks](https://github.com/orgs/samt-x/projects/1/views/5) | Your tasks (requires login) |
| [Timeline](https://github.com/orgs/samt-x/projects/1/views/4) | GitHub's own timeline, without dependencies |

## Status

Phase 1 was concluded with a demo on 30 April 2026. Technical development was paused until the end of August. Phase 2 is planned as a 12-week continuation, but the plan has not been approved and the start date has not been set.

## Original plan for phase 1

Phase 1 ran from February to April 2026, in two-week sprints. Each sprint started with a planning meeting and ended with a demo. The work was divided into seven work packages:

1. Dream journey (core team)
2. Running POC or MVP
3. Information model
4. Architecture
5. Overview of the legal room for manoeuvre
6. Legal framework
7. Lessons-learned report (core team)

Three milestones governed the work: when it had been clarified which information elements the pilot should include, when the risk and vulnerability analysis (ROS) had been carried out, and when it had been decided how the pilot should proceed.

![Overall plan for phase 1, weeks 6–17 of 2026: dream journey in weeks 6–7, running POC, architecture and information model throughout the period, legal constraints and legal framework, and solution patterns and lessons-learned report towards the end. Five sprints with planning and demo, ROS in week 9 and decision on the way forward in week 15](overordnet-plan-fase-1.png)

## Plan for phase 2

{{< i-arbeid >}}

The plan for phase 2 is a draft (version 0.3, 29 September 2026) and has not been approved. It builds on a working document from the gathering at Gardermoen on 30 August 2026.

The work is divided into two tracks that are developed together. Track A (AP1–AP2) covers service, information and rules. Track B (AP3–AP4) covers architecture and testing. AP0, AP5, law, privacy, security, supplier dialogue and sharing of experience are cross-cutting.

| Work package | Content | Deliverables |
|---|---|---|
| AP0 Mobilisation and governance | Mandate, scope, actor map, sources, baseline, decision and risk log | Start-up note, measurement plan and P0 |
| AP1 Dream journey, process and responsibility | Desired user experience, future process, roles, RACI, deviations and exceptions | L1, L2 and L3 |
| AP2 Information, code lists and rules | Data elements, concepts, sources, quality requirements and machine-readable validation | L4 and L5 |
| AP3 National architecture and target architecture | Principles, capabilities, shared resources, the four interoperability levels, sharing pattern and architecture decisions | L6, capability map and decision basis for P2 |
| AP4 Solution design and prototype | Interfaces, security, test data, validation, error flow, logging and demonstration | L7 and L8 |
| AP5 Benefits, learning and continuation | Measurement, reuse, supplier plan, cost drivers, management and roadmap | L9, L10 and P3 |

The deliverables L1–L10 are described under [Roadmap](/en/pilotering/pilot-1/loesningsvalg/veikart/).

### Milestones and decision gates

| Time | Milestone or gate | Decision or result |
|---|---|---|
| Week 1 | P0 Start-up | Owner, project manager, mandate, resources, scope and sources are confirmed |
| Week 7 | M1 Dream journey | The dream journey is approved by the municipality, the county authority and the professional communities concerned |
| Week 7 | P1 Model basis | Process, responsibility, data, code lists and prioritised rules are agreed |
| Week 10 | P2 Architecture and prototype | The assessment against national architecture, target architecture, sharing pattern, security, scenario, test data and capacity is approved |
| Week 12 | M2 Demonstration | A bounded scenario has been demonstrated end to end with test data and documented measurement |
| Week 12 | P3 Continuation | Results, benefits, cost drivers, dependencies and management have been examined, and the next phase is decided |

The prototype will only be built if P2 approves the scenario, test data, security, solution design, capacity and learning objectives. Detailed development does not start until after P2.

### Overall plan

| Work package | Week 1 | Week 2 | Weeks 3–5 | Weeks 4–7 | Weeks 7–10 | Weeks 11–12 | Gate |
|---|---|---|---|---|---|---|---|
| AP0 Mobilisation and governance | Active | | | | | | P0 |
| AP1 Dream journey, process and responsibility | Start | AS-IS user journey | AS-IS user journey | Dream journey | | | M1, P1 |
| AP2 Information, code lists and rules | | Start | | Model and rule set | | | P1 |
| AP3 National architecture and target architecture | | | | Analysis | Target architecture and sharing pattern | | P2 |
| AP4 Solution design and prototype | | | | | Design | Build, test and demo | M2 |
| AP5 Benefits, learning and continuation | Baseline | | | | Measurement | Consolidation | P3 |
| Law, security, supplier dialogue and sharing of experience | Start | Ongoing | Ongoing | Review | Ongoing | Close-out | P0–P3 |

The work is coordinated weekly in the core group, with professional and architecture workshops as needed.

## Timeline

All tasks on the board, with arrows showing which tasks wait for each other. What has happened is dark. Missing dates are calculated and dashed. The chart is generated from the board every hour. How to read it, and how a task gets into it: see [Timeline](/en/prosjektleveranser/loesninger/samhandlingsplattform/oppgavestyring/tidslinje/) in task management.

{{< inline-svg "project-1-en.svg" "/en/prosjektleveranser/loesninger/samhandlingsplattform/oppgavestyring/tidslinje" >}}
