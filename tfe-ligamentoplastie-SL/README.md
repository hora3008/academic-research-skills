# Projet : rééducation après ligamentoplastie scapho-lunaire

Travail mené avec la bibliothèque **academic-research-skills (ARS) v3.23.0**, pipeline complet (`academic-pipeline`).
Langue de sortie : français (termes techniques conservés en anglais quand c'est l'usage).

## État du pipeline

```
Étape 1  RESEARCH ......... [EN COURS]
           Phase 1 cadrage ........ [FAIT] forme choisie : REVUE SYSTÉMATIQUE
           Protocole PRISMA-P ..... [FAIT] v1.0 confirmé (Maes) ; enregistrement OSF à faire par l'auteur
           Phase 2 recherche ...... [EN COURS] recherches faites : 1 001 notices → 562 uniques
                                    protocole de tri sr-screener : [FAIT] v1.0 confirmé (Maes)
                                    pilote (182 notices) : IA en cours ; TES ÉTIQUETTES ATTENDUES
                                    puis tri complet → textes intégraux → extraction → risque de biais
           Phase 3 synthèse ....... [ ] synthèse narrative (SWiM) + GRADE + avocat du diable (point de contrôle 2)
           Bilan fin d'étape 1 .... [ ]
Étape 2  WRITE ............ [ ]
Étape 2.5 INTEGRITY ....... [ ] obligatoire, ne peut pas être sautée
Étape 3  REVIEW ........... [ ] jury simulé : 5 relecteurs dont un avocat du diable
Étape 4  REVISE ........... [ ]
Étape 3' RE-REVIEW ........ [ ]
Étape 4' RE-REVISE ........ [ ] si nécessaire
Étape 4.5 FINAL INTEGRITY . [ ] obligatoire
Étape 5  FINALIZE ......... [ ] MD, puis DOCX/PDF à ta demande
Étape 6  PROCESS SUMMARY .. [ ] journal de collaboration humain-IA (facultatif)
```

## Fichiers

| Fichier | Contenu |
|---|---|
| `etape1_recherche/01_RQ_Brief.md` | Question de recherche, sous-questions, périmètre, scores FINER |
| `etape1_recherche/02_Protocole_PRISMA-P.md` | **Protocole de la revue systématique** (PICOS, critères, bases, tri, extraction, risque de biais, synthèse) |
| `etape1_recherche/02_Methodology_Blueprint.md` | Ancien plan méthodologique (remplacé, gardé pour l'historique) |
| `etape1_recherche/03_Devils_Advocate_CP1.md` | Critique contradictoire du cadrage (point de contrôle 1) |
| `etape1_recherche/OSF_enregistrement_guide.md` | Comment enregistrer le protocole sur OSF |
| `etape1_recherche/phase2/00_journal_phase2.md` | **Journal de la recherche systématique** (bases, équations, nombres PRISMA) |
| `etape1_recherche/phase2/tri/` | Protocole de tri `sr-screener` (anglais) + explication en français + configuration |
| `etape1_recherche/phase2/recommandations/` | Recherche de recommandations officielles et registres d'essais |
| `etape1_recherche/contexte/bibliographie_contexte.md` | **Bibliographie commentée** des chapitres pathologie et chirurgie (44 sources, Vancouver, niveau de preuve) |
| `etape1_recherche/phase2/extraction/` | Grille d'extraction (tableur), grilles RoB 2 / ROBINS-I / JBI, test sur Kemler 2023 |
| `etape1_recherche/phase2/tri/ft_protocol_BROUILLON.md` | Brouillon du protocole de tri sur texte intégral (à confirmer plus tard) |
| `etape1_recherche/04_cartographie_preliminaire.md` | Recherche exploratoire PubMed : sources clés par sous-question |
| `etape1_recherche/journal_recherches/` | Résultats bruts des recherches (reproductibilité pour le jury) |
| `material_passport.yaml` *(local, non publié)* | Passeport du matériel : traçabilité et contraintes confirmées |
| `material_passport_run_ledger.yaml` *(local, non publié)* | Registre des décisions mot pour mot (lu par script uniquement) |

> ⚠️ Document éducatif. Il ne remplace pas l'avis de ton chirurgien ni le protocole de ton kinésithérapeute.

> Les exports de recherche contenant les résumés des articles (droits des éditeurs) restent dans la session et ne sont pas publiés ici. Les équations sont archivées, ce qui permet de refaire les recherches.
