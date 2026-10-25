# Étape 1 · Phase 1 : Methodology Blueprint · version 2 (REMPLACÉ)

> ⚠️ **Remplacé** par `02_Protocole_PRISMA-P.md` depuis que l'auteur a choisi la revue systématique (2026-10-08). Conservé pour l'historique de la démarche méthodologique.

> Produit par `deep-research` / `research_architect_agent`, mode `full`, phase 1.
> **v2 (2026-10-08)** : intègre tes réponses (2020 inclus, exceptions antérieures à 2020 encadrées, pas de preuves transposées, style Vancouver, aucun cas individuel). La *forme* de revue de littérature (systématique, de portée, narrative…) **n'est pas choisie ici** : c'est ton choix, demandé par la bibliothèque au point de contrôle en cours.

---

## Research Paradigm

**Selected :** post-positivisme pragmatique, celui de la pratique fondée sur les preuves (*evidence-based practice*).
**Justification :** la question cherche à décrire ce que la littérature rapporte et à juger la solidité des preuves pour guider la pratique. Elle ne vise ni à comprendre une expérience vécue (paradigme interprétatif) ni à tester une hypothèse causale.

## Method

**Type :** recherche secondaire (synthèse de littérature), principalement qualitative et descriptive, avec extraction de données chiffrées (délais, amplitudes, force, scores).
**Specific Method :** revue de la littérature avec **recherche documentée et reproductible** (bases, équations, dates, nombre de résultats) et **gradation du niveau de preuve** de chaque source. La forme exacte sera fixée par ton choix après confirmation de la question.
**Justification :** la question principale est descriptive (« que rapporte la littérature… ») et ses sous-questions couvrent des types d'études très différents : cadavres, biomécanique, séries de cas, cohortes, essais, revues. Une méta-analyse n'est pas envisageable à ce stade : la recherche exploratoire ne trouve pas assez d'essais homogènes sur la rééducation post-opératoire.

## Data Strategy

**Data Type :** secondaire (publications).
**Sources (phase 2) :**
- **Recherche ciblée de recommandations officielles (*guidelines*, consensus, déclarations de sociétés savantes)** : TRIP Database, Guidelines International Network, sites des sociétés de chirurgie et de rééducation de la main (p. ex. FESSH, ASSH, ASHT, SFCM/GEMMSOR), HAS, KCE. Objectif : vérifier si une recommandation officielle existe
- PubMed/MEDLINE : déjà interrogé pour la cartographie exploratoire ; journal dans `journal_recherches/`
- Europe PMC (texte intégral libre)
- PEDro : essais en kinésithérapie
- Cochrane Library
- Littérature francophone : *Hand Surgery and Rehabilitation* (ex-*Chirurgie de la Main*), *Kinésithérapie, la Revue*, EM-Consulte
- *Journal of Hand Therapy* et *Hand Therapy* (revues des thérapeutes de la main)
- Embase/Scopus seulement si ton école y donne accès (tu me fourniras alors les exports)
- Vérification de chaque référence par DOI/PMID via Crossref, OpenAlex et Semantic Scholar (outils intégrés à la bibliothèque)

**Équation de recherche principale (brouillon, PubMed) :**
```
(scapholunate OR scapho-lunate OR "carpal instability")
AND (reconstruction OR ligamentoplasty OR tenodesis OR capsulodesis OR repair OR Brunelli OR "3LT" OR SLAM OR "internal brace")
AND (rehabilitation OR "hand therapy" OR physiotherapy OR "physical therapy" OR mobilization OR immobilization OR orthosis OR splint
     OR "early motion" OR "dart thrower*" OR proprioception OR "neuromuscular" OR "return to work" OR "return to sport")
Filtres : date de publication 2020-2026 ; humains ou cadavres ; anglais/français (+ espagnol/allemand si résumé exploitable)
```
Équations complémentaires, une par sous-question : pathologie et biomécanique ; techniques et résultats ; proprioception du poignet ; retour au travail et au sport. Elles sont déjà testées, voir `04_cartographie_preliminaire.md`.

**Sampling (critères d'éligibilité, brouillon) :**

| | Inclusion | Exclusion |
|---|---|---|
| Population | Adultes avec lésion SL (opérés pour les SQ2 à SQ4) ; cadavres et modèles biomécaniques du complexe SL | Enfants ; SLAC avancé traité par chirurgie palliative ; fractures du scaphoïde ; lésions péri-lunaires |
| Intervention / sujet | Reconstruction, réparation ou capsulodèse SL ; rééducation post-opératoire ; proprioception du poignet | Techniques sans lien avec le complexe SL |
| Types d'études | Revues systématiques, essais contrôlés, cohortes, séries de cas, études biomécaniques ou d'imagerie, revues d'experts, consensus | Éditoriaux sans données, résumés de congrès seuls, prépublications non relues (signalées à part si importantes) |
| Date | 2020 → 2026, **2020 inclus** | Avant 2020, sauf exception (voir règle ci-dessous) |
| Preuves transposées | — | **Exclues** : patients non opérés, sujets sains, greffes d'autres articulations (décision de l'auteur) |

**Règle d'exception pour les sources antérieures à 2020** (décision de l'auteur) : une source antérieure à 2020 n'est retenue que si elle remplit **les trois** conditions suivantes. (1) Elle est vraiment intéressante, typiquement une description originale encore utilisée. (2) Elle complète un point que les sources 2020-2026 ne couvrent pas. (3) Elle est toujours d'actualité : citée comme référence courante par au moins une source 2020-2026, sans être contredite par une source plus récente. Chaque exception est signalée « [Exception < 2020] » et justifiée. Si aucune source ne remplit ces conditions, aucune n'est ajoutée.


**Time Frame :** recherche réalisée le 2026-10-08, à mettre à jour avant la version finale. Le `monitoring_agent` peut produire une veille des nouvelles publications.

## Analytical Framework

**Technique :** extraction structurée puis **synthèse thématique et chronologique** (par phase de rééducation), avec carte des convergences et des contradictions.

**Steps :**
1. Tri des titres et résumés, puis des textes intégraux, selon les critères ci-dessus (méthode de tri selon la forme de revue que tu choisiras)
2. Extraction dans une grille commune. Pour chaque étude de rééducation : technique chirurgicale, type de fixation (broches, vis, *internal brace*), type et durée d'immobilisation, début des mobilisations passives et actives, DTM, début du renforcement et de la proprioception, mise en charge, délais de reprise (travail, sport), critères de progression utilisés, mesures de résultat, complications
3. Gradation de chaque source :
   - niveau de preuve selon la hiérarchie utilisée par la bibliothèque (méta-analyses > essais > cohortes > séries de cas > avis d'experts)
   - grille de risque de biais adaptée au type d'étude : RoB 2 pour les essais, ROBINS-I pour les études non randomisées, AMSTAR 2 pour les revues, JBI pour les séries de cas
4. Synthèse par sous-question, chaque recommandation portant une étiquette **[Preuve directe]** (étude sur des patients opérés) ou **[Avis d'experts]** ; une question sans réponse documentée est marquée **[Lacune]**, sans hypothèse comblée par transposition
5. Construction du **plan de traitement par phases** avec, pour chaque phase : objectifs, techniques, restrictions, **critères d'entrée et de sortie**, et niveau de preuve de chaque élément
6. Contrôle critique du `devils_advocate_agent` (point de contrôle 2) : recherche de sélection biaisée des preuves (*cherry-picking*) et des explications alternatives

**Tools :** scripts de la bibliothèque (vérification des citations sur 4 index, journal de recherche), grille d'extraction en tableau, **style de citation Vancouver** (références numérotées dans l'ordre d'apparition).

## Validity Criteria

| Criterion | Strategy to Ensure |
|---|---|
| Reproductibilité de la recherche | Équations, dates, bases et nombre de résultats archivés (`journal_recherches/`) ; diagramme de flux en fin de phase 2 |
| Exactitude des références | Chaque référence est vérifiée par DOI/PMID ; l'intégrité est contrôlée à l'étape 2.5 puis refaite à l'étape 4.5 (obligatoire) |
| Fidélité aux sources | Aucune affirmation sans citation ; source lue en texte intégral ou mention explicite « résumé seulement » ; localisateurs (page/section) pour les citations clés |
| Distinction preuve / opinion | Étiquettes [Preuve directe] / [Avis d'experts] / [Lacune] sur chaque recommandation |
| Transparence des désaccords | Les contradictions sont exposées avec la qualité de preuve de chaque camp (p. ex. le DTM) |
| Neutralité | Plusieurs techniques et les deux familles de protocoles (immobilisation prolongée avec broches, mobilisation précoce) sont présentées ; aucune n'est prise comme référence par défaut |

## Limitations (By Design)

- **Peu de preuves directes sur la rééducation post-opératoire.** Atténuation : étiquetage explicite ; transpositions signalées ; aucune « recommandation forte » sans base.
- **Hétérogénéité des techniques chirurgicales**, ce qui limite les comparaisons. Atténuation : protocoles présentés par famille de techniques.
- **Restriction aux publications ≥ 2020** : exclut des travaux fondateurs. Atténuation : règle d'exception encadrée (voir *Sampling*).
- **Pas de preuves transposées** : certaines questions (cicatrisation de la greffe, proprioception après chirurgie) auront peu ou pas de réponse directe. Atténuation : lacunes signalées explicitement, ce qui est aussi un résultat.
- **Biais de langue** (anglais/français).
- **Auteur unique assisté par l'IA.** Atténuation : vérification automatique des références, revue simulée par 5 relecteurs à l'étape 3, déclaration IA.

## Ethical Considerations

- Pas de sujets humains : synthèse de littérature publiée.
- Le document contiendra un avertissement : il ne remplace pas un avis médical ni le protocole de ton équipe soignante.
- La déclaration d'utilisation de l'IA est obligatoire.

## Human-Subjects Administrative Status

Non applicable : aucune collecte de données sur des personnes.

> **Human-subjects boundary :** this output does not authorize recruitment, consent, access to identifiable data, intervention, or data collection.

## Reporting Standard

- Recommended guideline : **dépend de la forme de revue que tu choisiras.** PRISMA 2020 pour une revue systématique, PRISMA-ScR pour une revue de portée (*scoping review*), pas de guide EQUATOR obligatoire pour une revue narrative. Ce n'est pas une recommandation de forme, seulement la correspondance forme → guide.

## Preregistration

- Recommended : selon la forme choisie (PROSPERO pour une revue systématique ; OSF possible pour une revue de portée ; non requis pour une revue narrative)
- Platform : N/A pour l'instant
- Status : Not applicable (à revoir après ton choix)
- Completed artifact declaration : not_provided
- Companion handle : none
- Sidecar ownership : dispatching layer only ; do not populate a digest here
