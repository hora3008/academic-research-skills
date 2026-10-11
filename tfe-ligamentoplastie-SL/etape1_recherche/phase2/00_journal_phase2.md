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

## 3. Tri sur titre et résumé (terminé le 2026-10-10)

| Étape | Nombre |
|---|---|
| Notices triées | 562 |
| **Exclues** | **487** : E1 type de publication 233 ; E2 pas une étude clinique 86 ; E3 population 156 ; E4 intervention 11 ; E9 autre 1 |
| **Retenues pour le texte intégral** | **75** (55 éligibles, 20 incertaines) ; dont 5 dans une langue hors liste, à vérifier au texte intégral |
| Accord entre les 2 relecteurs IA | 99,1 % ; kappa 0,96 ; PABAK 0,98 ; 5 désaccords arbitrés |
| Contrôle qualité (relecture de 376 exclusions) | 1 notice réintégrée |
| Études témoins | 3/3 retenues |
| Vérification humaine | **Aucune** (décision de l'auteur, dérogation enregistrée dans `tri/sr_work/pilot_override.json`) |

Fichiers : `tri/Screening_TA/` : nombres PRISMA (`TA_prisma_counts.md`), méthodes (`TA_methodes_selection_FR.md`), journal des décisions sans résumés (`TA_journal_decisions_sans_resumes.csv`), corpus (`TA_literature_corpus.yaml`).

## 4. Textes intégraux

- Récupérés automatiquement en accès libre : **16 sur 75** (14 via le texte libre d'Europe PMC, mis en PDF ; 2 via des dépôts universitaires). Chaque PDF a été contrôlé : le titre correspond à la notice.
- Manquants : **59** (éditeurs qui bloquent le téléchargement automatique, ou articles non libres). Liste : `tri/textes_integraux_manquants.md`.

## 5. Tri sur texte intégral (terminé le 2026-10-10)

| Étape | Nombre |
|---|---|
| Textes recherchés | 75 |
| **Non récupérés** | **59** (option (a) choisie par l'auteur : pas de recherche manuelle des PDF) |
| Textes évalués | 16 |
| Exclus | 7 : E1 note technique sans patients 1 ; E3 population (fractures du radius) 1 ; E4 pas de geste ligamentaire (RASL, transfert tendineux dynamique) 2 ; **E5 protocole post-opératoire insuffisamment décrit 3** |
| En attente de classement | 1 (R00092 : âge des patients non rapporté) |
| **Études incluses** | **8** |
| Accord entre relecteurs IA (inclure ou non) | 87,5 % ; kappa 0,75 ; 2 désaccords arbitrés |
| Vérification humaine | Aucune (décision de l'auteur) |

Fichiers : `tri/Screening_FT/` (`FT_prisma_counts.md`, `FT_methods_selection.md`, `FT_literature_corpus.yaml`).

⚠️ Deux des trois études témoins (Kemler 2023, Ying 2024) font partie des textes **non récupérés** : elles ne sont donc pas incluses. Kemler 2023 est pourtant gratuit sur PMC pour un lecteur humain.

## 6. Extraction des données et risque de biais (terminés le 2026-10-11)

- **Deux extractions IA indépendantes** des 8 études incluses : n° 1 dans la session principale, n° 2 par 8 agents séparés sans accès à la n° 1. Les désaccords ont été tranchés en relisant la source. Aucune vérification humaine.
- **Accord sur 96 données clés :** 81 concordantes (84 %), 13 complétées (omissions de l'extraction n° 1), 2 divergentes (interprétation de la non-infériorité de Bakker 2022 ; complications de Lee 2023).
- **Incident corrigé :** les PDF fabriqués à partir d'Europe PMC avaient perdu le contenu des tableaux. Les tableaux ont été récupérés dans le XML source. Ils ne changent aucune décision du tri sur texte intégral.
- **Question d'éligibilité pour l'auteur :** Nienstedt 2023 (ténodèse dynamique, incluse) et R00527 (stabilisation dynamique, exclue) relèvent de la même famille de techniques.
- Fichiers : `extraction/extraction_reconciliee_et_risque_biais.md` (version de référence) ; `extraction/grille_extraction_IA2_brute.csv` (grille de 60 colonnes de l'extraction n° 2, brute).

## 7. Étape suivante

Phase 3 : synthèse narrative (SWiM), GRADE, cadre par phases, avocat du diable (point de contrôle 2). Dossier `../phase3/`.
