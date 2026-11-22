---
# id: auto-generated – copied values are overwritten automatically on push
id: c3642c32-45ac-4d09-9640-e4f8cb6971ae
title: "Current situation"
linkTitle: "Current situation"
weight: 30
aliases:
 - /pilotering/pilot-1/brukerreiser/
lastmod: 2026-11-22T04:06:29+01:00
last_editor: Erik Hagen

---
How the pupil list is transferred from primary and lower secondary school to upper secondary today, and which requirements Novari sets for a digital transfer to VIGO Skole.

## Transfer of the pupil list today

The process concerns the transfer of pupil data from primary and lower secondary school to upper secondary school ahead of the transition between the schools. The purpose is to prepare the pupils in the county authorities so that they can apply for upper secondary education at the beginning of January.

The main challenge is that the process is largely manual on the municipalities' side. School administration staff in primary and lower secondary schools download files from the line-of-business system (for example Vigilo), store and edit them locally on a PC, and then upload them to the county authority's line-of-business system (Vigo). The process is relatively simple, but is perceived as unnecessary, since it ought to have been automated. Storing files locally is also a security risk, because data can go astray from files that are stored and not deleted.

![AS-IS user journey for the transfer of the pupil list between primary and lower secondary school and upper secondary: the school administration downloads a file with pupil data from Vigilo, stores and edits it locally and uploads it to Vigo Skole, and the admission office moves the files on to Vigo. On the right: scope, how the process is experienced, variants and what matters](as-is-overforing-elevliste.png)

## Requirements for a digital transfer

After discussions with its subject-matter experts, Novari has described requirements for the three transfers of data on school leavers from the lower secondary schools' school administration systems (SAS) to VIGO Skole. Novari believes the transfer should preferably be handled in the lower secondary schools' SAS. The requirements are:

- **Complete data sets.** A transfer shall always cover all school leavers (list or grade data), not individual pupils. Otherwise the county authority does not know when the transfer is complete, and the lower secondary school does not know whether it has been accepted.
- **Correct errors at source.** Errors and warnings shall be corrected in the lower secondary school's SAS, so that knock-on errors are avoided. This follows from the principle of accuracy (GDPR Article 5(1)(d)), data protection by design (Article 25) and the right to rectification (Article 16).
- **Maskinporten.** A new API for VIGO Skole should use Maskinporten for machine-to-machine authentication. Only the municipalities in the county authority concerned are given access, controlled by organisation number. The municipalities can delegate access to third parties, for example KS Digital or a supplier as an Altinn system user. Today access is controlled by VIGO school number.
- **Role-based access.** Today the county authority appoints super users at the lower secondary schools who upload the files. With an API, this should be replaced by role-based access in the SAS.
- **Only error-free data sets are accepted.** Warnings (for example missing subjects or too many optional subjects) can be accepted, but should be corrected. Errors can result in an incorrect points basis, so that pupils wrongly fail to get in or receive an offer.
- **Continuous validation.** The SAS should validate continuously against the rules in Udir's grading guidelines (føringsskriv) and the rules for national identity numbers in the registration handbook, or at least on submission.
- **Clear feedback.** Errors and warnings shall be reported together and clearly to the submitter, with the status accepted, errors or warnings. The response from the API describes errors per pupil, but not the machine-readable rule that failed.
- **Quick correction.** Deadlines are often short (3–7 days), especially for final grades in the summer. It must be possible to correct and resubmit straight away.
- **No submission after the deadline.** Changes that arrive after the points calculation or submission deadline shall not be sent via the API. The SAS should block submission after the deadline, or give a clear warning. The county authority handles late changes, such as appeals, manually and with logging directly in VIGO.

The lower secondary school retrieves written examination grades from Udir's test administration system (PAS), and they shall be registered in the school system before the final data package is delivered to VIGO.
