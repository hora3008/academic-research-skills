# PRISMA 2020 counts - full-text stage

```mermaid
flowchart TD
  F["Reports sought for retrieval (n = 75)"]
  N["Reports not retrieved (n = 42)"]
  E["Reports assessed for eligibility (n = 33)"]
  X["Reports excluded (n = 14)<br/>E1 Publication type (review, editorial, letter, comment, erratum, conference abstract, protocol, trial registration, book chapter, technique note without patient outcomes, case report of 1-4 patients, survey of clinicians): 2<br/>E3 Population: not SL injury in adults, SLAC stage II or higher, or SL repair during distal radius fracture fixation without separate SL data: 2<br/>E4 Intervention: no SL ligament repair, reconstruction or capsulodesis (conservative care, debridement or thermal shrinkage alone, RASL or screw or K-wire fixation alone, salvage surgery): 4<br/>E5 Postoperative protocol not described to the minimum level (immobilisation type or duration, or start of motion, plus one more element): 6"]
  C["Reports of included studies (n = 18)"]
  U["Reports awaiting classification (n = 1)"]
  F --> N
  F --> E
  E --> X
  E --> C
  E --> U
```

```json
{
 "stage": "ft",
 "tool": "sr-screener 1.0.0",
 "complete": true,
 "pending_records": 0,
 "pending_ta_records": 0,
 "pending_ta_qc_records": 0,
 "fulltext_set_out_of_date": false,
 "state_problems": [],
 "reports_sought_for_retrieval": 75,
 "reports_not_retrieved": 42,
 "reports_assessed": 33,
 "reports_to_assess": 33,
 "reports_excluded": 14,
 "excluded_by_reason": {
  "E1 Publication type (review, editorial, letter, comment, erratum, conference abstract, protocol, trial registration, book chapter, technique note without patient outcomes, case report of 1-4 patients, survey of clinicians)": 2,
  "E3 Population: not SL injury in adults, SLAC stage II or higher, or SL repair during distal radius fracture fixation without separate SL data": 2,
  "E4 Intervention: no SL ligament repair, reconstruction or capsulodesis (conservative care, debridement or thermal shrinkage alone, RASL or screw or K-wire fixation alone, salvage surgery)": 4,
  "E5 Postoperative protocol not described to the minimum level (immobilisation type or duration, or start of motion, plus one more element)": 6
 },
 "reports_unclear_awaiting_classification": 1,
 "studies_included_reports": 18,
 "agreement": {
  "n": 33,
  "both_advance": 16,
  "both_exclude": 15,
  "a_only_advance": 1,
  "b_only_advance": 1,
  "observed_agreement": 0.9394,
  "kappa": 0.879,
  "pabak": 0.879
 },
 "decided_by": {
  "A+B": 31,
  "ADJ": 1,
  "Maes (author)": 1
 }
}
```
