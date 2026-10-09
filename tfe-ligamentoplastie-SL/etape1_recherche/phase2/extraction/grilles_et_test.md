# Grilles d'extraction et d'évaluation du risque de biais, avec test sur une étude témoin

> Conformes au protocole PRISMA-P v1.0 (rubriques « Données extraites » et « Risque de biais ») et à l'agent `risk_of_bias_agent` de la bibliothèque.
> Le tableur vide correspondant est `grille_extraction.csv` (60 colonnes, une ligne par étude incluse).

---

## 1. Grille d'extraction (à remplir pour chaque étude incluse)

Chaque donnée porte un **localisateur** : page, tableau ou section où elle se trouve. Une donnée absente est notée **« NR » (non rapporté)**, jamais devinée.

| Bloc | Variables | Pourquoi c'est utile pour le document final |
|---|---|---|
| Étude | auteur, année, pays, revue, DOI/PMID, type d'étude, niveau de preuve, financement et conflits d'intérêts, enregistrement | Situer la qualité et l'indépendance de l'étude |
| Patients | effectifs inclus et analysés, âge, sexe, côté dominant, lésion aiguë ou chronique, dynamique ou statique, stade (Garcia-Elias, Geissler, EWAS), profession et sport | Savoir à qui s'appliquent les résultats |
| Chirurgie | technique, greffe, broches (nombre, durée), vis, *internal brace*, voie ouverte ou arthroscopique, gestes associés | La rééducation dépend de ce qui a été fait |
| **Rééducation** | immobilisation (type, position, articulations incluses, durée) ; début des mobilisations passives et actives ; DTM (oui/non, quand) ; restrictions d'amplitude ; début du renforcement et muscles ciblés ; proprioception (type, début) ; électrostimulation ; mise en charge ; autres restrictions ; **type de critères de progression (temps écoulé ou critères cliniques) et leur détail** ; délais de reprise du travail et du sport ; encadrement (kiné ou domicile), nombre de séances, observance | **Cœur de la revue : construire le plan par phases** |
| Résultats | outil du résultat principal (PRWE, DASH, QuickDASH, Mayo…) et valeurs à chaque temps ; douleur ; mobilité ; force ; radiologie ; taux de reprise ; satisfaction | Ce qu'on peut attendre après chaque protocole |
| Sécurité | complications, réinterventions, durée moyenne de suivi | Limites et signaux d'alerte |

**Règle de vérification (protocole) :** pré-extraction par l'IA, puis vérification par l'auteur de **100 % des données des études comparatives** et de **20 % des séries de cas** tirées au hasard. Si plus de 5 % d'erreurs sont trouvées, on vérifie toutes les séries.

---

## 2. Grilles de risque de biais

| Type d'étude | Grille | Domaines | Jugements possibles | Règle globale |
|---|---|---|---|---|
| Essai randomisé | **RoB 2** | D1 processus de randomisation ; D2 écarts aux interventions prévues ; D3 données manquantes ; D4 mesure du résultat ; D5 sélection du résultat rapporté | Faible / Quelques inquiétudes / Élevé | Algorithme RoB 2 (un domaine « élevé » rend l'ensemble « élevé ») |
| Étude comparative non randomisée | **ROBINS-I** | D1 confusion ; D2 sélection des participants ; D3 classement des interventions ; D4 écarts aux interventions ; D5 données manquantes ; D6 mesure des résultats ; D7 sélection du résultat rapporté | Faible / Modéré / Sérieux / Critique / Pas d'information | Le jugement global = le domaine le plus sévère |
| Cohorte à un bras, série de cas | **Checklist JBI pour séries de cas** (10 items) | Critères d'inclusion clairs ; mesure standard de la pathologie ; méthode d'identification valide ; inclusion consécutive ; inclusion complète ; démographie décrite ; données cliniques décrites ; résultats et suivi décrits ; site/contexte décrit ; analyse statistique adaptée | Oui / Non / Incertain / Non applicable par item | Pas de score global imposé ; résumé qualitatif |

Chaque jugement s'appuie sur une **citation ou un localisateur** de l'étude (règle G3 de `risk_of_bias_agent`). Une information manquante est elle-même un signal de risque.

**Après l'évaluation :** **GRADE** pour chaque résultat comparatif (mobilisation précoce vs tardive : fonction, mobilité, force, complications, reprise du travail).
- Point de départ « élevé » pour les essais randomisés, « faible » pour les études observationnelles.
- Abaissement possible pour risque de biais, incohérence, caractère indirect, imprécision, biais de publication.

---

## 3. Test de la grille sur une étude témoin : Kemler et al. 2023

> **Statut : TEST DU FORMULAIRE, pas encore une extraction définitive.**
> Source : page PMC de l'article (PMC9836776), lue via un outil de lecture web qui renvoie un **résumé structuré**, pas le texte exact. Les localisateurs renvoient aux sections de l'article. **Chaque valeur est à vérifier sur le PDF** avant usage dans la revue. L'étude devra aussi passer formellement le tri sur texte intégral.

**Référence (Vancouver) :** Kemler MA, Bootsman JJ, van den Berg J. Scapholunate Ligament Reconstruction without Immobilization Is Safe and Leads to Better Functional Results. J Wrist Surg. 2023;12(1):23-7. doi:10.1055/s-0042-1749164 PMID: 36644724.

| Variable | Valeur extraite | Localisateur |
|---|---|---|
| Type d'étude | Essai **non randomisé**, attribution dans l'ordre d'inclusion | Methods : Group Assignment |
| Patients | 21 (11 *internal brace* + mobilisation précoce ; 10 broches pendant 6 semaines) ; 18-65 ans ; lésion SL confirmée en arthroscopie, Geissler ≥ 2 ; inclusion de juillet 2019 à janvier 2020 | Methods ; Results |
| Chirurgie (commune) | Ténodèse à trois ligaments avec bandelette distale du FCR | Methods : Surgical Procedure |
| Groupe *internal brace* | Augmentation par ruban de suture + vis dans le scaphoïde et le lunatum | Methods : Surgical Procedure |
| Groupe contrôle | 2 broches de 1,5 mm + ancre | Methods : Surgical Procedure |
| Immobilisation, groupe *internal brace* | **Attelle antébrachiale 1 semaine**, puis kinésithérapie de la main | Methods : Postoperative Regimen |
| Immobilisation, groupe contrôle | **Plâtre brachial** (changé à 10 jours), retiré avec les broches **à 6 semaines**, puis kinésithérapie | Methods : Postoperative Regimen |
| Contenu de la kinésithérapie, critères de progression, renforcement, proprioception | **NR** dans le résumé obtenu ; à vérifier dans le PDF | — |
| Mesures | Mobilité active (goniomètre), force (Jamar, position 2), PRWHE, QuickDASH, douleur (EN), effet global perçu (7 points), reprise du travail ; à l'inclusion, 6 semaines, 3 mois, 6 mois, 1 an | Methods : Data Collection and Follow-Up |
| Analysés à 1 an | 10 *internal brace* / 7 contrôle | Results |
| Flexion (variation à 1 an) | +1,8° vs −13,4° (p = 0,004) | Results, Table 2 |
| Extension | +4,5° vs −4,5° (p = 0,03) | Results, Table 2 |
| Force | +8,2 kg vs +7,7 kg (p = 0,9) | Results, Table 2 |
| PRWHE / QuickDASH (variation) | −19,2 vs −14,7 (p = 0,5) / −12,1 vs −5,3 (p = 0,5) | Results, Table 2 |
| Reprise du travail | **35,1 vs 73,6 jours (p = 0,01)** | Results |
| Complications | 1 rupture traumatique par groupe (*internal brace* : à 4 mois, puis résection de la première rangée ; contrôle : chute à 5 mois, refixation) ; 2 perdus de vue dans le groupe contrôle | Results : Complications |

**Pré-évaluation ROBINS-I (IA, provisoire, à valider) :**

| Domaine | Jugement | Justification |
|---|---|---|
| D1 Confusion | **Sérieux** | Les groupes diffèrent par la **chirurgie** (*internal brace* + vis vs broches + ancre) **et** par la rééducation : l'effet de la mobilisation précoce ne peut pas être séparé de celui de la fixation |
| D2 Sélection | Modéré | Attribution selon l'ordre d'inclusion, sans randomisation |
| D3 Classement des interventions | Faible | Protocoles clairement définis |
| D4 Écarts aux interventions | Modéré | Contenu de la kinésithérapie non décrit dans le résumé ; une refixation dans le groupe contrôle |
| D5 Données manquantes | **Sérieux** | 3 sur 10 non analysés à 1 an dans le groupe contrôle |
| D6 Mesure des résultats | Modéré | Évaluateurs et patients non aveugles ; questionnaires subjectifs |
| D7 Sélection du résultat rapporté | Pas d'information | Protocole préenregistré non mentionné |
| **Global** | **Sérieux** | Domaine le plus sévère |

**Ce que le test montre sur la grille :**
- La grille fonctionne.
- Le **contenu exact de la kinésithérapie** (exercices, progression) n'apparaît pas dans un résumé structuré. Il faudra **le texte intégral (PDF)** pour chaque étude.
- Ce test confirme le risque SR-2 identifié par l'avocat du diable : dans beaucoup d'études, protocole de rééducation et technique chirurgicale changent **en même temps**.
