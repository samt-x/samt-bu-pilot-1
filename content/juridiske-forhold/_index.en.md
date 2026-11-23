---
# id: auto-generated – copied values are overwritten automatically on push
id: d6ff5943-b53d-4da7-8396-c038517ff6ee
title: "Legal matters"
linkTitle: "Legal matters"
weight: 60
aliases:
 - /pilotering/pilot-1/juss/
lastmod: 2026-11-22T04:06:29+01:00
last_editor: Erik Hagen

---
An initial legal assessment of privacy in phase 1, an assessment of the need for a full data protection impact assessment (DPIA), and the risks identified in the risk and vulnerability (ROS) work. The pilot concerns the transfer of the pupil list from the primary and lower secondary school to Vigo in November every year.

The assessment builds on a cross-disciplinary workshop and several working meetings with the pilot team, where needs, data sources and high-level functional requirements were mapped. It has two purposes: to show how the pilot can be carried out lawfully within existing regulations, and to point to measures that can provide greater room for manoeuvre in the longer term. Only privacy has been assessed, not other areas of law. The document is dynamic and will be updated as the pilot progresses.

## Responsibility and agreements

The controller has the main responsibility for complying with the General Data Protection Regulation (GDPR Article 4(7)). Anyone who processes data on behalf of the controller is a processor (Article 4(8)).

**The municipality** collects personal data about pupils in order to fulfil its statutory duties in primary and lower secondary school, and structures and stores it in its own systems, such as Vigilo and the municipality's data platform. The municipality is the controller for this.

**The county authority** needs information about the pupils in order to process applications for a school place and to follow up the pupils who are admitted. This is done for the county authority's own purposes and in its own systems, including Vigo.

The municipality has no agreement with Vigo, and the county authority has no agreement with the municipality's systems. The parties do not jointly determine the purposes or means, and do not process data on behalf of each other. **The municipality and the county authority are therefore separate controllers.**

**Processors:** the supplier of the municipality's school administration system (for example Vigilo) and KS Digital process data on behalf of the municipality. Novari IKT processes data on behalf of the county authority in connection with Vigo. The processors act on instructions (Article 28).

## Legal basis

The legal basis for exchanging pupil information between primary and lower secondary school and upper secondary follows from chapters 9 and 25 of the Education Act (opplæringslova) and chapter 20 of the Education Regulations (opplæringsforskrifta).

- **The Education Act section 9-5:** the county authority shall ensure a safe and good transition from primary and lower secondary school to upper secondary education, and the municipality shall cooperate with the county authority on the transition. It is assumed that this cooperation also includes the transfer of information about pupils.
- **The Education Act section 25-1:** municipalities and county authorities may process personal data when necessary to perform duties under the Act, and the county authority may obtain necessary information from the primary and lower secondary schools in order to carry out admission.
- **The Education Regulations section 20-4** narrows down what the county authority may obtain for admission: whether primary and lower secondary school has been completed, the half-year assessment with grades from Year 10, and the grades and absence recorded on the leaving certificate.

The November transfer only covers name, national identity number, school and class, which section 20-4 does not mention. It can nevertheless be based on section 9-5, because it contributes to a statutory duty: a good transition, which also prepares for the later transfer under section 20-4.

The lawful basis for processing under the GDPR is **Article 6(1)(e)**: the processing is necessary for the exercise of official authority. The supplementary legal basis is the Education Act section 9-5, cf. section 25-1. The transfer does not include special categories of personal data, so Article 9 has not been assessed.

## Consent is not the right basis

Some municipalities currently base the transfer on consent. According to the assessment, this is neither necessary nor appropriate:

- **Not freely given.** There is a clear imbalance between the pupil or parents and the school, and the transfer is closely linked to the pupil's ability to have their application for a school place processed (Article 4(11), Article 7 and Recital 43).
- **Cannot be withdrawn in a meaningful way.** Once the data has been transferred and used in admission, withdrawal is difficult to reconcile with the recipient's obligations regarding documentation and case processing.
- **Not necessary.** The transfer is part of statutory duties and the exercise of official authority.

Instead, emphasis should be placed on a clear purpose, data minimisation, access control, logging, a clear division of responsibility and good information to pupils and parents.

## Security and the rights of data subjects

| Topic | Risk | Measures in the pilot |
|---|---|---|
| Transparency and information | Missing or unclear information | Information text to pupils and parents about the transfer: purpose, recipient, data types and retention period |
| Purpose limitation | Data is used beyond the pilot's purpose | The purpose (transfer for admission) is documented, and the data platform is used only for structuring and controlled onward transmission. No analysis or secondary use |
| Data minimisation | Too much or too detailed information | A specific and limited set of fields. Surplus fields are filtered out before transfer |
| Retention and deletion | Data remains after the pilot | The information is stored only temporarily in the data platform and deleted after the transfer |
| Access control | Too broad internal access | Access for a small number of named roles with a business need, with a clear separation between test, operations and development |
| Right of access | Difficult to gain access | Ordinary access procedures in the municipality and the county authority, made clear in the information |
| Rectification and erasure | Missing procedures | Existing procedures in Vigilo and Vigo. The data platform holds no master data |
| Consent | Uncertainty about consent | Consent is not used. The processing is based on the exercise of official authority |
| Confidentiality | Unauthorised access or leakage | Established, secure integrations and as little manual handling as possible |
| Testing | Real personal data in testing | Synthetic or anonymised data where possible |
| Documentation | Difficult to demonstrate compliance | Assessments of roles, purposes, data types and measures are collected in the pilot documentation |

## Delimitation of the pilot

The principles of purpose limitation, data minimisation and storage limitation can make reuse and analysis of data demanding. In order to comply with the regulations while building competence, a stepwise approach is recommended. Phase 1 was delimited as follows:

- The municipality retrieves the necessary pupil information from Vigilo and places it in the data platform.
- Only basic functions of the platform are tested: loading, structuring and processing, quality assurance and standardisation, and controlled and traceable sharing with the recipient.
- The platform is not used for analysis, combination with other sources or reuse.
- All personal data is deleted from the platform after the transfer.
- The county authority receives only the information needed to process applications for a school place.

Before live data is used, the municipality and the county authority should enter into (or check that they have) data processing agreements and data disclosure agreements, document the processing and legal bases in the record of processing activities, and follow up the measures in the table above.

## Data protection impact assessment (DPIA)

An initial DPIA was carried out to identify risks and clarify whether a full DPIA is needed. One of ten criteria applied: the processing concerns children and young people, a vulnerable group. «Large scale» was set to no, with some doubt, because the number of pupils can increase rapidly and the term is not quantified.

The conclusion is that **a full DPIA is not necessary at present**, because the pilot is tightly delimited, the data is processed only briefly and then deleted, and no new technology, profiling or automated decision-making is used. The need shall be reassessed when the data flow, technical mechanisms and access control have been determined, when reuse, analysis or new functions are considered, when more data sources are connected, or when the number of data subjects increases significantly.

## Risks (ROS)

The ROS work identified risks for the POC itself and for a future digital process. The risks have not been scored.

**The POC:**

- Real personal data used in the POC is unintentionally exposed. Measure: synthetic data or a very limited number.
- The set-up creates weaknesses in access control that can lead to vulnerabilities in production systems.
- The API in the POC does not match the production environments (for example VIGO).
- The suppliers do not have capacity for the changes the POC requires. Measure: use OneRoster.

**The digital process:**

- The data exchange contains malware or code that stops the data flow.
- Data format and structure in the lower secondary schools' sources do not match VIGO, so data must be corrected manually.
- The process from the POC cannot be reused with larger data sets.
- The procedures become too extensive for the users, who revert to old methods.
- Data remains with KS Digital longer than necessary.
- Transfer of grades and more detailed information leads to leaks. The more information per pupil, the higher the consequence.
- Duplicate pupils when identification is not unique, for example when moving to a municipality with a different system.
- The information from individual schools is not sufficiently separated.
- «Ghost records» when pupils change school or municipality.
- New data quality requirements in the school administration system (OAS) that require major adaptations.
- Planning functionality in the OAS is synchronised too early.
- IST or VIGO do not have capacity to change the solution before and during operation.
- Pupils lose access to the line-of-business system prematurely with frequent transfers.
- Schools that are not supposed to be included are transferred anyway.
- Errors in exception lists cause pupils to drop out and only be discovered when they are about to apply.
- High activity at the start of the school year has not been sufficiently investigated.
- The admission office loses its overview in the new process.

## What the pilot learned

**About the process.** It pays to work systematically with privacy right from the start. This makes it clear what has not been understood or clarified, and gives the lawyers a better picture of which questions are relevant. Legal assessments depend on details of the data flow, user journey and technical design, which only become visible in a concrete case, and the technical solutions in turn affect which legal questions arise. This requires continuous dialogue and an iterative way of working. Legal questions should be clarified concretely in each pilot before the knowledge is developed into general guidance.

**About data sharing and reuse.** The GDPR requires concrete assessments from case to case, but templates and structures can make the assessments easier. The work should be seen in connection with the Allmenningen project at KS Digital, which works on common components and frameworks in the municipal sector. Two areas should be prioritised: guidance on purpose limitation, lawful basis and the data protection principles, and clarifications regarding the data platform that KS Digital must follow up.

**About collaboration around children and young people.** Oslo kommune's insight work has mapped pain points that should be addressed in later pilots: fear of sharing, analogue sharing and manual work, differing training, system and regulatory challenges, unclear roles, weakened user participation and trust, lack of standardisation, fragmented systems, high dependency on individuals and uncertainty about what can actually be shared. The project group also proposes an overview of relevant special legislation, and following up whether new regulatory provisions could make data handling more predictable. Udir should be involved in this.

**Templates.** The pilot has created a general template for the framework document and a template for data flow and data points (purpose, legal basis, data types, roles, necessity and references). It is recommended to create partly pre-filled templates for ROS and DPIA, standardised agreements (data processing agreements and data disclosure agreements) with guidance on choosing the type of agreement, and guidance on reuse for compatible purposes.
