# PRISMA 2020 counts - title/abstract stage

```mermaid
flowchart TD
  I["Records identified from databases (n = 1001)<br/>Europe PMC n = 466; PEDro n = 4; PubMed/MEDLINE n = 531"]
  R["Records removed before screening:<br/>duplicate records (n = 439)"]
  S["Records screened (n = 562)"]
  X["Records excluded (n = 487)<br/>E1 Publication type (review of any kind, editorial, letter, comment, reply, erratum, conference abstract, protocol, trial registration, book chapter, surgical technique note without patient outcomes, case report of 1-4 patients, survey of clinicians): 233<br/>E2 Not a clinical patient study (cadaver, biomechanical, animal, in vitro, computational or finite-element, imaging of healthy wrists): 86<br/>E3 Population: not scapholunate ligament injury or instability in adults (other carpal or wrist conditions, salvage-stage SLAC, perilunate dislocation, scaphoid fracture or nonunion, children only): 156<br/>E4 Intervention: scapholunate injury not treated by surgical repair or reconstruction (conservative care only, diagnosis or imaging only, debridement or thermal shrinkage alone, salvage procedures): 11<br/>E9 Other (explained): 1"]
  F["Reports sought for retrieval (n = 75)"]
  I --> R
  I --> S
  S --> X
  S --> F
```

```json
{
 "stage": "ta",
 "tool": "sr-screener 1.0.0",
 "complete": true,
 "pending_records": 0,
 "state_problems": [],
 "identified_by_database": {
  "Europe PMC": 466,
  "PEDro": 4,
  "PubMed/MEDLINE": 531
 },
 "identified_total": 1001,
 "duplicates_removed": 439,
 "records_screened": 562,
 "records_to_screen": 562,
 "records_excluded": 487,
 "excluded_by_code": {
  "E1": 233,
  "E2": 86,
  "E3": 156,
  "E4": 11,
  "E9": 1
 },
 "reports_sought_for_retrieval": 75,
 "advanced_include": 55,
 "advanced_unclear": 20,
 "advanced_outside_allowed_languages": 5,
 "agreement": {
  "n": 562,
  "both_advance": 70,
  "both_exclude": 487,
  "a_only_advance": 3,
  "b_only_advance": 2,
  "observed_agreement": 0.9911,
  "kappa": 0.96,
  "pabak": 0.982,
  "conflicts": 5,
  "resolved_by": {
   "A+B": 556,
   "ADJ": 5,
   "QC": 1
  }
 },
 "decided_by": {
  "A+B": 556,
  "ADJ": 5,
  "QC": 1
 }
}
```
