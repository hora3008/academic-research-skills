# Étape 1 · Phase 2 : journal de recherche (revue systématique)

> `deep-research` mode `systematic-review` (`bibliography_agent`) + `sr-screener` (phase 0 protocole, phase 1 notices).
> Protocole : `../02_Protocole_PRISMA-P.md` v1.0, confirmé par Maes le 2026-10-08.

## 1. Recherches exécutées le 2026-10-08

| Base | Équation | Notices | Fichier |
|---|---|---|---|
| PubMed/MEDLINE | équation du protocole, limite `"2020/01/01"[dp] : "2026/10/08"[dp]` (texte exact : `exports/pubmed_query.txt`) | **531** | `exports/pubmed_2026-10-08.nbib` |
| Europe PMC | adaptation de l'équation (champs TITLE_ABS, FIRST_PDATE 2020-01-01 → 2026-10-08, prépublications exclues : NOT SRC:PPR) (`exports/europepmc_query.txt`) | **466** | `exports/europepmc_2026-10-08.csv` |
| PEDro | champ « Abstract & Title », recherches séparées : `scapholunate`, `scapho-lunate`, `carpal instability`, `scaphol*` (0 résultat chacune), `wrist instability` (1), `wrist ligament*` (6), `scaphoid` (24) ; union = 31 notices, dont **4** publiées depuis 2020 (filtre d'année appliqué après extraction, PEDro n'en offrant pas pour cette recherche) | **4** | `exports/pedro_2026-10-08.csv` |
| ClinicalTrials.gov (registre) | `scapholunate OR "scapho-lunate" OR "carpal instability" OR "wrist instability" OR "scapholunate ligament"` | **48** enregistrements | `registres/clinicaltrials_2026-10-08.csv` (traités à part : études en cours) |
| Recommandations officielles | PubMed (filtres guideline/consensus/Delphi), recherche web sur les sites des sociétés savantes | voir `recommandations/` | |
| Non interrogées | Embase, Scopus, Web of Science, CINAHL, Cochrane CENTRAL : pas d'accès (limite déclarée) | — | — |

## 2. Identification (diagramme PRISMA 2020, partie « Identification »)

| Étape | Nombre |
|---|---|
| Notices identifiées dans les bases | 1 001 (PubMed 531 ; Europe PMC 466 ; PEDro 4) |
| Enregistrements identifiés dans les registres | 48 (ClinicalTrials.gov) |
| Doublons retirés (`sr-screener prepare_records.py`, DOI + titre) | 439 |
| **Notices uniques à trier (titre + résumé)** | **562** (dont 7 sans résumé), réparties en 13 lots |
| Études témoins retrouvées | 3/3 (Bakker 2022 → R00269 ; Kemler 2023 → R00156 ; Ying 2024 → R00090) |

Détail du dédoublonnage : `tri/sr_work/duplicates.csv` ; comptes : `tri/sr_work/identification.json`.

## 3. Étapes suivantes (rien n'est trié pour l'instant)

1. ⏸ **Confirmation du protocole de tri** par l'auteur (`tri/screening_protocol.md` ; explication : `tri/protocole_tri_explication_FR.md`). C'est une règle de fer de `sr-screener` : aucun tri avant cette confirmation.
2. ⏸ **Enregistrement OSF** par l'auteur (guide : `../OSF_enregistrement_guide.md`), idéalement avant le tri.
3. Pilote : l'auteur classe lui-même l'échantillon, puis comparaison avec les relecteurs IA.
4. Tri complet des titres et résumés (après accord de l'auteur sur le coût), arbitrage, contrôle qualité.
5. Récupération des textes intégraux (accès libre via Europe PMC/PMC ; les autres sont à obtenir par l'auteur).
6. Tri sur texte intégral, extraction des données, risque de biais (RoB 2 / ROBINS-I / JBI).
