# Déclaration de transparence : sélection des études par IA (brouillon pour les Méthodes et la Discussion)

> Rédigée à partir de la décision de l'auteur du 2026-10-10, enregistrée mot pour mot dans le registre du projet. Elle sera reprise et adaptée lors de la rédaction (étape 2), puis contrôlée par la vérification d'intégrité (étapes 2.5 et 4.5) et par le mode `disclosure` de la bibliothèque (étape 5).

## Pour la section Méthodes

La sélection des études a été réalisée avec l'outil `sr-screener` (bibliothèque *academic-research-skills*, v3.23.0), à partir d'un protocole de tri fixé et confirmé par l'auteur **avant** toute lecture des notices.

**Tri sur titre et résumé :**
- Chaque notice a été classée **indépendamment par deux relecteurs IA**, sans accès à la décision de l'autre :
  - relecteur A, avec la consigne d'un expert du contenu ;
  - relecteur B, avec la consigne d'un méthodologiste.
- Les désaccords « retenir contre exclure » ont été tranchés par un **troisième relecteur IA (arbitre)**.
- Un contrôle qualité automatique a fait relire par un relecteur IA senior un échantillon tiré au sort des exclusions communes, ainsi que les exclusions « limites ».

**Modèle :** les relecteurs sont des instances du même modèle de langage (Claude Sonnet, via l'alias `sonnet` de Claude Code).

**Rôle de l'auteur :**
- Il a défini la question de recherche, les critères d'éligibilité et les règles de tri, et confirmé les protocoles.
- Les consignes envoyées aux relecteurs IA (*prompts*) ont été générées automatiquement par l'outil à partir de ce protocole confirmé.
- **L'auteur n'a pas classé d'échantillon pilote et n'a vérifié aucune décision de tri** (ni les études retenues, ni les études exclues). L'outil prévoit normalement ces deux étapes humaines. Cette dérogation a été choisie par l'auteur, et sa raison est enregistrée dans le journal de l'outil (`pilot_override.json`).

## Pour la section Discussion (limites)

- **Absence de vérification humaine.** Toutes les décisions de sélection reposent sur l'IA. Les erreurs de sélection (études pertinentes exclues à tort, ou études hors sujet retenues) n'ont pas été contrôlées par une personne. Les standards méthodologiques des revues systématiques (Cochrane, AMSTAR 2) attendent une sélection en double par des humains.
- **Indépendance limitée des relecteurs IA.** Les deux relecteurs ont travaillé en aveugle l'un de l'autre, mais ce sont deux instances du **même modèle**. Leurs erreurs peuvent donc être corrélées : une même lecture erronée peut être partagée. L'accord élevé entre eux ne prouve pas que leurs décisions sont justes.
- **Pas de calibration sur un classement humain.** Faute de pilote étiqueté par l'auteur, la sensibilité de l'IA (sa capacité à ne rater aucune étude pertinente) n'a pas été mesurée sur ce sujet.
- **Atténuations réelles :**
  - protocole fixé à l'avance ;
  - trois études témoins connues ;
  - arbitrage systématique des désaccords ;
  - relecture obligatoire d'un échantillon d'exclusions ;
  - équations de recherche et décisions archivées et reproductibles.
- **Portée du document.** Ce travail est un exercice de formation et d'information. Il n'a pas été soumis à un jury ni à une revue par les pairs, et il ne doit pas être utilisé comme recommandation clinique.
