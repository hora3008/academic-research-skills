# Protocole de revue systématique (PRISMA-P 2015) · version 1.0 (brouillon)

> Produit par `deep-research`, mode `systematic-review`, phase 1 (`research_question_agent` et `research_architect_agent`), à partir du modèle `deep-research/templates/prisma_protocol_template.md`.
> Statut : **brouillon à confirmer par l'auteur.** Les points marqués ⟨choix⟩ attendent ta décision. Une fois confirmé, ce protocole est **figé** : toute modification ultérieure est consignée dans le tableau des amendements.
> Ce document remplace le *Methodology Blueprint* (fichier 02 précédent), conservé pour l'historique.

---

## INFORMATIONS ADMINISTRATIVES

### Titre

**Protocoles de rééducation après reconstruction chirurgicale du ligament scapho-lunaire chez l'adulte : protocole de revue systématique**
*(EN : Postoperative rehabilitation after surgical scapholunate ligament reconstruction in adults: a systematic review protocol)*

Enregistrement : ⟨choix⟩ (a) OSF Registries avant le début de la recherche ; (b) pas d'enregistrement, déclaré comme limite.

### Auteurs et contributions

| # | Rôle | Contribution |
|---|---|---|
| 1 | Auteur principal et garant ⟨nom à compléter⟩ | Choix du protocole, validation du tri, vérification des extractions, interprétation, rédaction finale |
| 2 | Second relecteur humain ⟨choix⟩ : camarade (optionnel) | Tri indépendant d'un échantillon aléatoire (voir *Sélection*) |
| — | Assistance IA (non-auteur) : Claude (Anthropic) via la bibliothèque *academic-research-skills* | Exécution des recherches, tri par deux relecteurs IA en aveugle et un arbitre IA, pré-extraction avec localisateurs, pré-évaluation du risque de biais, aide à la rédaction. Chaque usage est déclaré (PRISMA-trAIce, contrôlé aux étapes 2.5 et 4.5 du pipeline). |

### Amendements

| Date | Section | Modification | Justification |
|---|---|---|---|
| 2026-10-08 | — | Version initiale | — |

### Financement

Aucun financement externe. Aucun conflit d'intérêts déclaré.

---

## INTRODUCTION

### Justification

L'instabilité scapho-lunaire est la forme la plus fréquente d'instabilité du carpe. Non traitée, une lésion complète du complexe ligamentaire scapho-lunaire peut entraîner douleur, perte de fonction et évolution vers l'arthrose de type SLAC (*scapholunate advanced collapse*) [Dréant 2023, PMID 37004985]. De nombreuses techniques de reconstruction sont décrites : ligamentoplasties tendineuses, capsulodèses dorsales, techniques combinées et réparations augmentées [Dréant 2023 ; Terras 2025, PMID 40878732].

Les protocoles post-opératoires rapportés vont de l'immobilisation prolongée avec broches à la mobilisation précoce. Une cohorte multicentrique rapporte des résultats non inférieurs avec une mobilisation active précoce après ténodèse à trois ligaments [Bakker 2022, PMID 36055872]. Une petite étude comparative associe *internal brace* et mobilisation précoce à une reprise du travail plus rapide [Kemler 2023, PMID 36644724]. Pour l'instabilité de stade 1 non opérée, une enquête de pratique ne trouve pas de consensus de rééducation [Holmes 2024, PMID 39464687]. Une revue systématique porte sur le retour au sport et au travail après chirurgie, mais pas sur le contenu de la rééducation [Liew 2023, PMID 36457032].

La recherche exploratoire (PubMed, 2026-10-08) n'a trouvé **aucune revue systématique publiée depuis 2020 sur la rééducation après reconstruction scapho-lunaire**. Cette revue vise à combler ce manque pour les kinésithérapeutes, les étudiants et les patients.

### Objectifs

**Question de recherche (une phrase) :**
Chez l'adulte opéré d'une reconstruction ou réparation du ligament scapho-lunaire, quels protocoles de rééducation post-opératoire sont rapportés depuis 2020, en termes de contenu, chronologie, restrictions et critères de progression, et quels résultats fonctionnels, cliniques et radiologiques leur sont associés, y compris lorsque des protocoles sont comparés entre eux ?

| PICOS | Définition |
|---|---|
| **P** Population | Adultes opérés d'une reconstruction ou réparation du complexe ligamentaire scapho-lunaire, pour une instabilité aiguë ou chronique, dynamique ou statique, sans arthrose avancée |
| **I** Intervention | Protocole de rééducation post-opératoire après toute technique de reconstruction ou réparation SL |
| **C** Comparateur | Autre protocole post-opératoire (p. ex. mobilisation précoce vs immobilisation prolongée), **ou aucun** (études à un seul bras) |
| **O** Résultats | Fonction rapportée par le patient (principal) ; douleur, mobilité, force de préhension, complications, radiologie, retour au travail et au sport (secondaires) ; contenu des protocoles (descriptif) |
| **S** Types d'études | Essais randomisés, études comparatives non randomisées, cohortes, séries de cas (≥ 5 patients) |

**Objectifs secondaires :**
1. Comparer les résultats entre familles de protocoles, quand des données comparatives existent.
2. Recenser les **critères de progression** (passage d'une phase à l'autre, reprise du travail et du sport) et préciser s'ils sont fondés sur le temps écoulé ou sur des critères cliniques.
3. Identifier les **recommandations officielles** (*guidelines*, consensus) existantes sur la rééducation après chirurgie SL.

**Partie non systématique (déclarée comme telle) :** les chapitres de contexte sur la pathologie (anatomie, biomécanique, mécanismes, classifications, histoire naturelle) et sur les techniques chirurgicales s'appuient sur des sources 2020-2026 choisies par l'auteur. Ils peuvent inclure des exceptions antérieures à 2020 selon la règle UC-002. Ils ne relèvent pas de la méthode systématique.

---

## MÉTHODES

### Critères d'éligibilité

| Critère | Inclusion | Exclusion |
|---|---|---|
| **Type d'étude** | Essais randomisés ou quasi randomisés ; études comparatives non randomisées ; cohortes prospectives ou rétrospectives ; séries de cas d'au moins 5 patients | Cas cliniques (< 5 patients), notes techniques sans résultats de patients, études cadavériques, biomécaniques ou d'imagerie seule, revues, éditoriaux, protocoles sans résultats |
| **Date de publication** | 2020-01-01 → date de la recherche (**2020 inclus**, UC-001) | Avant 2020. ⟨choix⟩ proposition : **pas d'exception pour les études incluses**, pour garder un critère fixe et reproductible ; l'exception UC-002 s'applique seulement aux chapitres de contexte |
| **Langue** | Anglais, français, néerlandais, allemand, espagnol | Autres langues (nombre d'exclusions rapporté) |
| **Statut de publication** | Articles publiés avec relecture par les pairs, en texte intégral | Résumés de congrès seuls, prépublications |
| **Contexte** | Tout pays, tout milieu de soins | — |

**Participants :** au moins 80 % d'adultes (≥ 18 ans), ou données des adultes séparables. Instabilité ou dissociation scapho-lunaire traitée chirurgicalement. Exclusions : arthrose SLAC de stade II ou plus, sauf si les données sont séparables ; luxations péri-lunaires ; fractures du scaphoïde associées (sauf si les données sont séparables) ; chirurgies palliatives (résection de la première rangée, arthrodèses).

**Interventions :** toute technique de reconstruction ou réparation SL, ouverte ou arthroscopique (ligamentoplastie avec greffe tendineuse, capsulodèse dorsale, technique combinée, réparation avec augmentation de type *internal brace*). Elle doit être **suivie d'un protocole post-opératoire décrit avec au moins** :
- (a) le type ou la durée de l'immobilisation, ou le délai de début des mobilisations ;
- (b) **et** un autre élément : contenu des exercices, progression, restrictions ou délais de reprise des activités.

Une étude qui ne décrit pas son protocole post-opératoire est exclue (motif « protocole non rapporté », compté dans le diagramme PRISMA).

**Comparateurs :** autre protocole post-opératoire, ou aucun.

**Résultats :**
- *Principal* : fonction rapportée par le patient (PRWE/PRWHE, DASH, QuickDASH, Mayo Wrist Score ou autre questionnaire validé).
- *Secondaires* :
  - douleur (EVA ou EN) ;
  - mobilité (flexion, extension, inclinaisons radiale et ulnaire, en degrés ou en % du côté sain) ;
  - force de préhension (kg ou % du côté sain) ;
  - complications (échec ou perte de réduction, réintervention, infection sur broche, syndrome douloureux régional complexe, raideur, morbidité du site donneur) ;
  - radiologie (diastasis SL, angle SL, angle radio-lunaire, DISI, progression arthrosique) ;
  - retour au travail et au sport (taux et délai) ;
  - satisfaction.
- *Données descriptives du protocole* : phases, délais, techniques, restrictions, critères de progression, encadrement (kinésithérapeute ou programme à domicile).

**Temporalité :** pas de durée minimale de suivi pour décrire les protocoles. Les résultats sont regroupés par moment de mesure : < 6 mois, 6 à 12 mois, > 12 mois.

### Sources d'information

| Source | Accès | Justification |
|---|---|---|
| PubMed/MEDLINE | ✅ accessible depuis la session | Base biomédicale de référence |
| Europe PMC | ✅ accessible | MEDLINE + PMC + revues non indexées dans MEDLINE |
| PEDro | ✅ accessible | Essais et revues en kinésithérapie |
| ClinicalTrials.gov | ✅ accessible | Essais non publiés, contrôle des résultats sélectifs |
| TRIP Database + sites des sociétés savantes (FESSH, ASSH, ASHT, SFCM/GEMMSOR), HAS, KCE | ✅ (TRIP) | Recommandations officielles (objectif secondaire 3) |
| Embase, Scopus, Web of Science, CINAHL, Cochrane CENTRAL | ⟨choix⟩ seulement via l'accès de ton école ; tu me fournis les exports (RIS/CSV) | Couverture complémentaire. *Cochrane est bloqué depuis cette session.* |
| Listes de références des études incluses, et articles qui les citent | ✅ (Crossref, OpenAlex, Semantic Scholar) | Recherche par citations, en amont et en aval |

### Stratégie de recherche (PubMed, brouillon)

Choix méthodologique : **pas de bloc « rééducation » dans l'équation.** Beaucoup d'études chirurgicales décrivent leur protocole post-opératoire seulement dans la partie *Méthodes*, ni dans le résumé ni dans l'indexation. Exiger des termes de rééducation ferait perdre ces études. Le contrôle « protocole décrit » se fait donc au tri en texte intégral.

```
#1 Population / condition
   scapholunate[tiab] OR scapho-lunate[tiab] OR "scapho lunate"[tiab] OR SLIL[tiab]
   OR "scapholunate dissociation"[tiab]
   OR (("Joint Instability"[Mesh] OR instabilit*[tiab]) AND (carpal[tiab] OR carpus[tiab] OR wrist[tiab]))
#2 Chirurgie
   reconstruct*[tiab] OR ligamentoplast*[tiab] OR tenodes*[tiab] OR capsulodes*[tiab] OR repair*[tiab]
   OR "internal brace"[tiab] OR internalbrace[tiab] OR augment*[tiab] OR Brunelli[tiab]
   OR "three-ligament"[tiab] OR "3-ligament"[tiab] OR 3LT[tiab] OR SLAM[tiab] OR SLIC[tiab] OR SLICL[tiab]
   OR ANAFAB[tiab] OR "Reconstructive Surgical Procedures"[Mesh] OR "Tendon Transfer"[Mesh]
#3 #1 AND #2
Filtres : date de publication 2020/01/01 → date de recherche. Aucun filtre de langue ou de type d'étude dans l'équation (appliqués au tri).
```
Taille estimée (test du 2026-10-08) : environ 160 à 310 notices PubMed avant tri. Les équations des autres bases seront adaptées à leur syntaxe et archivées. L'équation est relue avec la checklist PRESS par le `devils_advocate_agent` avant exécution.

### Gestion des notices et sélection

1. **Gestion :** exports RIS ou .nbib de chaque base ; fusion et dédoublonnage avec les scripts de `sr-screener` ; journal de tri exportable (Excel ou CSV).
2. **Tri titre et résumé, puis texte intégral** ⟨choix⟩. Option proposée :
   - deux relecteurs IA en aveugle (`sr-screener` : relecteur A « expert du contenu », relecteur B « méthodologiste ») et un arbitre IA en cas de désaccord ;
   - contrôle qualité automatique : nouvelle vérification des exclusions communes et des cas limites, accord kappa et PABAK ;
   - **toi, tu valides toutes les inclusions et un échantillon aléatoire des exclusions.**
   - La bibliothèque le rappelle : les relecteurs IA assistent, ils ne remplacent pas un second relecteur humain. Si un camarade accepte, il trie indépendamment un échantillon aléatoire de 20 % (accord rapporté par un kappa).
3. **Pilote :** 50 notices triées avant le tri complet, pour calibrer les critères. Tu valides le rapport de calibration.
4. **Documentation :** motif d'exclusion codé et ordonné pour chaque texte intégral exclu ; diagramme de flux PRISMA 2020.

### Extraction des données

- Formulaire standardisé (voir *Données extraites*), testé sur 3 études.
- Pré-extraction par l'IA avec **localisateur** (page, tableau ou section) pour chaque donnée. ⟨choix⟩ proposition : **tu vérifies 100 % des données des études comparatives et 20 % des séries de cas**, tirées au hasard. Si le taux d'erreur dépasse 5 %, toutes les séries sont vérifiées.
- Donnée manquante ou ambiguë : notée « non rapporté ». Contacter les auteurs n'est pas prévu, ce qui est déclaré comme limite.

### Données extraites

| Catégorie | Variables |
|---|---|
| Étude | Auteurs, année, pays, revue, type d'étude, niveau de preuve, financement, conflits d'intérêts, enregistrement |
| Participants | Effectif, âge, sexe, côté dominant, instabilité aiguë ou chronique, dynamique ou statique, classification (Garcia-Elias, Geissler, EWAS), profession et sport |
| Chirurgie | Technique, greffe, fixation (broches : nombre et durée ; vis ; *internal brace*), voie ouverte ou arthroscopique, gestes associés |
| **Protocole de rééducation** | Type d'immobilisation (plâtre, orthèse), position, articulations incluses, durée ; début des mobilisations passives et actives ; DTM ; début du renforcement et muscles ciblés ; proprioception ; électrostimulation ; mise en charge ; restrictions ; **critères de progression (temps ou critères cliniques)** ; délais de reprise du travail et du sport ; encadrement (kiné ou domicile), nombre de séances, observance |
| Résultats | Résultats principal et secondaires, à chaque moment de mesure (moyenne, écart-type, médiane, intervalle) |
| Complications | Type, fréquence, prise en charge |

### Risque de biais

| Type d'étude | Outil |
|---|---|
| Essais randomisés | RoB 2 |
| Études comparatives non randomisées | ROBINS-I |
| Cohortes à un bras et séries de cas | Checklist JBI pour séries de cas |

Pré-évaluation par l'IA (`risk_of_bias_agent`), avec une citation justificative par domaine ; validation par l'auteur. Les résultats servent à l'interprétation, et une analyse de sensibilité exclut les études à risque élevé si une méta-analyse est faite.

### Synthèse

- **Méta-analyse** seulement si au moins 3 études comparatives rapportent le même résultat avec des protocoles comparables. *La recherche exploratoire rend ce cas peu probable.* Le cas échéant : modèle à effets aléatoires, différence moyenne standardisée ou risque relatif, I², tau² et intervalle de prédiction (logiciel : R, package metafor).
- **Synthèse narrative structurée** (guide SWiM) dans les autres cas :
  1. tableaux par famille de techniques et par famille de protocoles (p. ex. mobilisation avant ou après 6 semaines) ;
  2. statistiques descriptives des composantes des protocoles (médiane et étendue des délais) ;
  3. direction des effets pour les études comparatives ;
  4. inventaire des critères de progression.
- **Cadre par phases :** la discussion peut proposer une synthèse des phases et des critères de passage tirée des protocoles inclus. Elle sera **présentée comme une synthèse des auteurs** ; chaque élément portera son niveau de preuve et sa source, et le cadre ne sera jamais présenté comme une recommandation officielle.
- **Sous-groupes prévus :** famille de techniques (greffe tendineuse, capsulodèse, *internal brace*) ; fixation par broches ou non ; instabilité dynamique ou statique.

### Biais de publication et de rapport

- Graphique en entonnoir seulement si au moins 10 études par résultat (peu probable).
- Comparaison avec les enregistrements ClinicalTrials.gov quand ils existent.

### Confiance dans l'ensemble des preuves

GRADE pour chaque résultat comparatif (p. ex. mobilisation précoce vs tardive : fonction, mobilité, force, complications, retour au travail). Les données descriptives à un seul bras ne reçoivent pas de cotation GRADE ; leur niveau de preuve est indiqué (série de cas = faible).

### Respect des contraintes de l'auteur

UC-001 (2020 inclus) · UC-002 (exceptions antérieures à 2020 : contexte uniquement, voir ⟨choix⟩) · UC-003 (pas de preuves transposées : population limitée aux patients opérés) · UC-004 (Vancouver) · UC-005 (aucun cas individuel) · UC-006 (pas de limite de longueur) · UC-007 (recommandations actuelles : objectif secondaire 3).

---

## ANNEXE : correspondance avec la checklist PRISMA-P

| Item PRISMA-P | Section |
|---|---|
| 1 Identification | Titre |
| 2 Enregistrement | Titre (⟨choix⟩) |
| 3a-b Auteurs, contributions | Auteurs et contributions |
| 4 Amendements | Amendements |
| 5a-c Financement | Financement |
| 6 Justification | Justification |
| 7 Objectifs (PICOS) | Objectifs |
| 8 Critères d'éligibilité | Critères d'éligibilité |
| 9 Sources | Sources d'information |
| 10 Stratégie de recherche | Stratégie de recherche |
| 11a-c Gestion, sélection, extraction | Gestion des notices et sélection ; Extraction |
| 12 Données | Données extraites |
| 13 Résultats et priorisation | Critères d'éligibilité (résultats principal et secondaires) |
| 14 Risque de biais | Risque de biais |
| 15a-d Synthèse | Synthèse |
| 16 Méta-biais | Biais de publication et de rapport |
| 17 Confiance | Confiance dans l'ensemble des preuves |
