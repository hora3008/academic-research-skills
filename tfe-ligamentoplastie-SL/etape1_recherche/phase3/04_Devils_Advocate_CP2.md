# Avocat du diable : point de contrôle 2 (après l'analyse)

> `deep-research` / `devils_advocate_agent`, point de contrôle 2. Ce qui est relu : la synthèse (phase 3 : `00_PRISMA_final.md`, `01_synthese_SWiM.md`, `02_GRADE_resume_des_preuves.md`, `03_cadre_par_phases.md`) et la base de preuves (`phase2/extraction/extraction_reconciliee_et_risque_biais.md`), comparées au protocole (`02_Protocole_PRISMA-P.md`, `01_RQ_Brief.md`), aux sources de contexte (`contexte/bibliographie_contexte.md`) et au point de contrôle 1.
> **Vérifications sur les sources :** S1 lu en entier ; passages des protocoles et des résultats vérifiés dans S2 à S8 ; consultés aussi : `phase2/00_journal_phase2.md`, `phase2/declaration_tri_IA.md`, `phase2/recommandations/recherche_recommandations.md` et `phase2/tri/textes_integraux_manquants.md`. Non ouverts : `material_passport*`, le registre d'exécution et `phase2/tri/sr_work`.
> Échelle : **Critique** (bloque le passage à la rédaction) · **Majeur** (à corriger avant la rédaction) · **Mineur** (à améliorer).
> Aucun fichier du dépôt n'a été modifié.

---

## Verdict : ÉCHEC (bloquant, mais réparable)

| Sévérité | Nombre |
|---|---|
| Critique | 1 |
| Majeur | 10 |
| Mineur | 8 |

**Pourquoi ÉCHEC.** Le travail d'analyse est sérieux, et plusieurs choix sont exemplaires (voir « Ce qui est solide »). Mais le constat n° 1 est bloquant. La synthèse et le GRADE présentent comme des faits sur la littérature (« une seule étude a comparé… », « aucune étude… », « il n'existe pas… ») ce qui ne vaut que pour 16 textes intégraux sur 75. Les 59 autres n'ont **pas été cherchés à la main, par choix**. Or 17 d'entre eux sont signalés comme gratuits sur PMC, dont la seule autre étude comparative connue sur la question évaluée par GRADE (Kemler 2023, « *without immobilization* »). En l'état, le tableau GRADE résume un ensemble de preuves que l'on sait incomplet.

**Chemin le plus court vers « PASS AVEC CONDITIONS » :**
1. récupérer au minimum les 17 textes gratuits sur PMC, dont Kemler 2023 (R00156), et tenter Ying 2024 (R00090) ; refaire le tri sur texte intégral et l'extraction pour ces textes ;
2. sinon, si l'auteur maintient l'option (a), requalifier le travail et borner **chaque** affirmation d'absence ou d'unicité (détail au constat n° 1) ;
3. corriger les erreurs factuelles des constats n° 4, 5 et 10, qui touchent des chiffres qu'un kinésithérapeute pourrait appliquer.

---

## Constats critiques

### 1. Corpus incomplet par choix, alors que les conclusions sont formulées comme des faits sur toute la littérature

- **Fichiers et sections :**
  - `00_PRISMA_final.md` (case N ; remarque 2) ;
  - `01_synthese_SWiM.md` §1, §6, §10.3, §11 (messages 1, 3, 5, 6) ;
  - `02_GRADE_resume_des_preuves.md` (domaine « Biais de publication » ; « Phrase de synthèse ») ;
  - `03_cadre_par_phases.md` (en-tête).
- **Problème :**
  - La revue repose sur 16 textes intégraux sur 75 (21 %). Le PRISMA et les limites disent que les 59 autres « n'ont pas pu être lus » faute d'accès libre.
  - En réalité, la recherche manuelle a été **écartée par l'auteur**, et la liste des textes manquants signale elle-même **17 textes gratuits sur PMC** : 11 retenus (« include ») et 6 incertains au tri sur titre et résumé.
  - Parmi eux se trouve **R00156 (Kemler 2023)**, *« Scapholunate Ligament Reconstruction without Immobilization Is Safe and Leads to Better Functional Results »*. C'est une étude comparative sur la question même que cote GRADE, et l'une des trois études témoins.
  - Ying 2024 (R00090), la deuxième étude témoin manquante, porte sur une « *Early Accelerated Motion Rehabilitation* » après reconstruction.
  - La recherche par citations promise par le protocole pour compenser les bases manquantes n'apparaît ni dans le journal de la phase 2 ni dans le PRISMA (pas de branche « autres méthodes »).
  - La recherche des recommandations est marquée « provisoire », et l'interrogation de TRIP n'est pas faite.
- **Pourquoi c'est important :**
  - **Unicité.** « Une seule étude compare deux protocoles » et « Une seule étude a comparé deux calendriers de rééducation » sont démenties par une étude connue, gratuite et non lue. Le tableau GRADE ne représente donc pas l'ensemble des preuves.
  - **Absences.** La « principale lacune » (critères uniquement temporels), « aucun critère clinique n'a été étudié », l'absence du lancer de fléchette, la proprioception citée dans « S1 seulement » et « il n'existe pas de recommandation » ne peuvent pas être tenues pour des faits sur la littérature.
  - **Volume.** Avec le taux d'inclusion observé sur les textes lus (8 sur 16), on peut s'attendre à **environ 25 à 30 études incluables de plus**. Ce n'est qu'un ordre de grandeur, mais la synthèse pourrait ne reposer que sur un quart du corpus.
  - **Biais d'accès.** L'échantillon n'est pas aléatoire. Il manque 10 rapports du *J Hand Surg Eur* et 4 de *Hand Surgery and Rehabilitation*, la revue de la SFCM, la plus proche du public francophone visé.
  - **Faux sentiment de sécurité.** Le contrôle par études témoins (3 sur 3 au tri) rassure à tort : 2 des 3 sont perdues à l'étape de récupération.
- **Preuves :**
  - `phase2/00_journal_phase2.md` §5 : « **Non récupérés** | **59** (option (a) choisie par l'auteur : pas de recherche manuelle des PDF) » ; et « Kemler 2023 est pourtant gratuit sur PMC pour un lecteur humain » ;
  - `phase2/tri/textes_integraux_manquants.md` : 17 lignes « (PMC gratuit : PMC…) », dont R00156 (PMC9836776) ;
  - `00_PRISMA_final.md` : « pas d'accès libre ou téléchargement bloqué » ; `01_synthese_SWiM.md` §10.3 : « 59 rapports sur 75 n'ont pas pu être lus » ;
  - Protocole, *Sources d'information* : « compensée par Europe PMC, PEDro et la recherche par citations » ;
  - `phase2/recommandations/recherche_recommandations.md` : « Statut : **provisoire.** » ; TRIP : « À faire à la main par l'auteur ».
- **Correction :**
  - **Option A (recommandée) :**
    - récupérer les 17 textes gratuits sur PMC, puis Ying 2024 et les autres par la bibliothèque, le prêt entre bibliothèques ou les auteurs, comme le propose déjà la liste des textes manquants ;
    - refaire le tri sur texte intégral, l'extraction, la synthèse et le GRADE ; mettre à jour le PRISMA ;
    - faire la recherche par citations en amont et en aval prévue au protocole, et l'interrogation de TRIP.
  - **Option B (si l'option (a) est maintenue) :**
    - **Titre :** requalifier le travail, par exemple « revue systématique limitée aux textes intégraux en libre accès récupérables automatiquement ».
    - **PRISMA :** remplacer le motif par « téléchargement automatique impossible ; recherche manuelle non faite (choix de l'auteur) ; 17 rapports disponibles gratuitement sur PMC ».
    - **Bornes :** borner chaque affirmation : « parmi les 16 textes lus », « dans les 8 études incluses ».
    - **GRADE :** dans le domaine du biais de publication, remplacer « Non évaluable » par « **preuves manquantes connues** (Kemler 2023, Ying 2024, non lues) : biais suspecté ».
    - **Synthèse :** remplacer la phrase de synthèse par « Parmi les études lues, une seule… ; au moins une autre étude comparative, non lue, existe ».
    - **Recommandations :** écrire « aucune recommandation trouvée dans les sources consultées (recherche provisoire ; TRIP non interrogée) ».

---

## Constats majeurs

### 2. GRADE : un niveau final plausible, mais des justifications incohérentes ou incomplètes

- **Fichier et section :** `02_GRADE_resume_des_preuves.md`, « Règles appliquées » et tableau de résumé.
- **Problèmes :**
  1. **Caractère indirect incohérent avec la population du tableau.**
     - Le tableau définit la population comme « adultes opérés d'une 3LT sans broches ». Pourtant, il abaisse de -1 pour indirect parce que la preuve porte sur « une seule technique (3LT sans broches) » alors que « la question de la revue porte sur toutes les reconstructions ».
     - On ne peut pas restreindre la population **et** abaisser pour cette même restriction.
     - L'argument du temps (« les résultats ne valent qu'à 3 mois ») ne tient pas non plus : le protocole prévoit une fenêtre « < 6 mois », à laquelle un résultat à 3 mois répond directement.
     - Une raison valable n'est pas citée : la rééducation de S1 est délivrée « *in specialized centers for hand surgery and therapy* » (p. 1077), loin du kinésithérapeute généraliste visé par la revue (UC-008).
  2. **Biais de publication.** « Non évaluable (moins de 10 études) » confond l'outil, le graphique en entonnoir, avec le domaine. Ici, des preuves manquantes sont **connues et nommées** (constat n° 1).
  3. **Imprécision mal motivée.**
     - « Une seule étude, 108 patients » n'est pas un critère GRADE. Les critères sont l'intervalle de confiance comparé au seuil, et la taille optimale d'information.
     - La raison existe pourtant : S1 est sous-dimensionnée pour sa propre marge. Elle annonce 70 participants pour une puissance de 0,80 avec une marge de 0,35. Avec la formule usuelle de non-infériorité (différence vraie nulle), il en faudrait environ 100 à 128 **par groupe**, selon le risque alpha unilatéral (0,05 ou 0,025).
     - Avec 54 patients par groupe, la puissance réelle est d'environ 45 à 57 % (mon calcul).
  4. **Risque de biais (D1) peut-être sous-estimé.**
     - Les témoins sont historiques : protocole tardif en 2012-2015, précoce en 2015-2017.
     - Le score de propension ne corrige ni la courbe d'apprentissage des chirurgiens, ni les autres changements de soins entre les périodes.
     - Juger D1 « sérieux » pour tous les résultats est défendable.
  5. **Complications.**
     - « 17 contre 20 (p = 0,54) » compare des **nombres d'événements** par un test du khi² : un patient peut en avoir plusieurs, donc ce p n'est pas interprétable.
     - Les auteurs ont aussi exclu 2 opérations du TFCC dans le groupe précoce (p. 1081). Elles ne figurent nulle part dans la synthèse.
  6. **Formulation des énoncés.**
     - Pour une certitude très faible, la forme GRADE recommandée (Santesso et al., 2020) est « Les preuves sont très incertaines quant à l'effet de X sur Y ».
     - « La mobilisation précoce **pourrait** donner une fonction semblable » et « **ne semble pas** augmenter les complications » commencent par une proposition rassurante, et c'est elle qu'un lecteur non spécialiste retiendra.
  7. **Point de départ.** Il est justifié par « règle de la bibliothèque ». Il faut citer la méthode : GRADE (Guyatt 2011) et GRADE 18 (Schünemann 2019) pour l'usage de ROBINS-I.
- **Pourquoi c'est important :**
  - Le niveau « très faible » reste probable par d'autres voies (D1 sérieux + imprécision ; ou indirect justifié par le lieu de la rééducation + imprécision).
  - Mais avec la logique actuelle du fichier, si l'on retire l'abaissement indirect pour une population 3LT, la fonction, la douleur et les complications remontent à « **faible** ».
  - Le niveau affiché dépend donc d'un jugement mal motivé.
- **Correction :**
  - **Une voie cohérente :** soit population large avec indirect -1, soit population 3LT avec indirect motivé par le lieu de la rééducation, ou D1 sérieux.
  - **Analyse de sensibilité :** l'écrire noir sur blanc (« le niveau reste très faible dans les deux cas »).
  - **Imprécision :** la motiver par l'intervalle de confiance et la puissance.
  - **Complications :** le résultat doit être « patients avec au moins une complication » ; il n'est pas rapporté, donc il faut le signaler comme tel et ajouter les 2 opérations du TFCC.
  - **Énoncés :** reformuler selon la forme GRADE ; citer les références méthodologiques.

### 3. La synthèse incline vers « la mobilisation précoce est sûre » : omissions et formulation

- **Fichiers et sections :** `01_synthese_SWiM.md`, Tableau 5 et message clé 3 ; `02_GRADE_resume_des_preuves.md`, « Phrase de synthèse » ; `03_cadre_par_phases.md`, Phase 4.
- **Problème :**
  - Les directions favorables au protocole précoce sont mises en avant : douleur au repos, infections 0 contre 3. Une direction défavorable est omise : parmi les patients au travail, **retour au poste d'origine 56 % (précoce) contre 76 % (tardif)** (S1, Tableau 3, p. 1082).
  - S1 n'a mesuré **aucun résultat radiologique** et ne peut pas détecter d'échec de la reconstruction. Les auteurs le disent : « *it could have led to an underestimation of uncommon complications, such as failure of the reconstruction* » (p. 1081).
  - Leur hypothèse selon laquelle l'essentiel de l'effet se voit en 12 semaines (p. 1082) est contestable. Le risque propre à la mobilisation précoce, l'allongement de la greffe et la perte de réduction, se manifeste justement plus tard (S4, S5).
  - « Pas de différence significative » et « pas plus de complications » seront lus par le grand public comme « pas de différence » et « sans danger ». La non-infériorité, elle, n'est pas démontrée.
- **Pourquoi c'est important :** c'est le message le plus susceptible d'être repris en pratique.
- **Preuves :** S1, Tableau 3 : « *Original work 16 (76) 10 (56)* » ; Tableau 2 et p. 1081 ; message 3 : « pas de différence significative à 3 mois, et pas plus de complications ».
- **Correction :**
  - **Message 3, proposition :** « Une seule étude lue, avec un suivi de 3 mois, n'a pas montré de différence nette entre un début de mobilisation à la 2e semaine et aux semaines 5-6 après 3LT sans broches. Elle était trop petite pour conclure à une équivalence, ne mesurait pas la tenue radiologique de la reconstruction, et le retour au poste d'origine était moins fréquent dans le groupe précoce (non significatif). On ne peut pas en conclure que la mobilisation précoce est sûre. »
  - **Tableaux :** ajouter la ligne « retour au poste d'origine » au Tableau 5 et au tableau GRADE.

### 4. Erreur de transcription sur la limite de flexion à 30° (S1)

- **Fichiers et sections :** `01_synthese_SWiM.md`, Tableau 1 (ligne « Début de la mobilisation du poignet ») ; `03_cadre_par_phases.md`, Phase 2 (« Restriction d'amplitude »).
- **Problème :**
  - S1 dit : semaine 2, mobilité du poignet avec « *care with flexion* » ; puis « *After 5 weeks, ROM of the wrist was increased to wrist flexion to 30°* ». La flexion est donc **portée à** 30° à partir de la semaine 5, et elle était inférieure avant.
  - La synthèse écrit l'inverse : « flexion limitée à 30° jusqu'à la semaine 5 » (Tableau 1) et « puis flexion limitée à 30° jusqu'à environ 5 semaines » (cadre, Phase 2). Lu ainsi, on autorise 30° dès la semaine 2 et on lève la limite à la semaine 5.
  - Le fichier se contredit : la ligne « Parcours B » du tableau du cadre, §1, est juste (« flexion jusqu'à 30° après 5 sem. »), comme l'extraction réconciliée (« après 5 semaines, flexion du poignet élargie jusqu'à 30° »).
  - **Remarque sur C38.** C38 (Bakker 2025, sur cadavre) vient du même groupe que S1 et a été publiée après lui. Elle ne corrobore donc pas S1 de façon indépendante. De plus, elle n'a été lue qu'en résumé.
- **Pourquoi c'est important :** c'est un chiffre directement applicable par un kinésithérapeute, et l'erreur va dans le sens d'une moindre protection.
- **Preuve :** S1 p. 1077 (« *Early active motion protocol* ») ; extraction §3.
- **Correction :**
  - **Formulation :** « Semaine 2 : mobilisation du poignet avec prudence en flexion (amplitude non chiffrée) ; à partir de la semaine 5 : flexion élargie jusqu'à 30° ; au-delà, NR. » Corriger les deux passages.
  - **C38 :** préciser « même équipe que S1 ; lu en résumé seulement ».

### 5. Message clé 4 faux, et statistiques descriptives qui mélangent des définitions

- **Fichiers et sections :** `01_synthese_SWiM.md`, Tableau 2 et §11, message 4 ; `03_cadre_par_phases.md`, Phase 3 et Phase 4.
- **Problème :**
  - **Le message 4 est faux.** Il affirme : « Le renforcement et la reprise des activités lourdes commencent en général entre 3 et 4 mois, parfois 6 mois ». Pour le renforcement, les données disent autre chose : S3 à 6 semaines, S1 à 7 (6 sur la figure), S5 à 8, S8 à 10-12, S4 seulement après 6 mois. **4 études sur 5 commencent entre 6 et 12 semaines** ; la médiane de la synthèse elle-même est de 9,5 semaines. Seule la reprise des activités lourdes tombe vers 3-4 mois.
  - **Tableau 2, renforcement.** La ligne « renforcement » additionne des choses différentes : kinésithérapie « *to regain grip strength* » (S3), « *increasing load* » (S5), renforcement (S8), et « *strengthening and resisted activities* » (S4). Une médiane sur 4 valeurs hétérogènes donne une précision trompeuse.
  - **Tableau 2, activités lourdes.** La ligne « Activités lourdes, charge complète ou sport autorisés » mélange elle aussi :
    - la mise en charge complète (S5, 16 semaines) ;
    - le sport et le travail lourd (S6) ;
    - le retour au poste et les « mouvements excessifs » (S3) ;
    - le **début** d'une reprise progressive (S8).
  - **Erreur sur S8.** Pour S8, le milieu 11 de « 10-12 » est compté comme une date d'autorisation. Or S8 dit : « *By 10 to 12 weeks… progression… to a strengthening protocol and gradually resumed all unrestricted functional activity* ». La date de reprise sans restriction n'est pas donnée, et la borne basse de l'étendue (11) en dépend.
- **Pourquoi c'est important :** un message clé faux sur le délai de renforcement est une information pratique directement trompeuse (UC-008).
- **Correction :**
  - **Message 4, à réécrire :** « Le renforcement commence, selon l'étude, entre 6 et 12 semaines (4 études sur 5), voire après 6 mois (S4, avec broches) ; les activités lourdes sont autorisées vers 3 mois, jusqu'à 6 mois selon l'étude. »
  - **Tableau 2 :** remplacer les médianes par la liste « étude : valeur, définition », ou séparer « mise en charge », « renforcement », « sport ou travail lourd ».
  - **S8 :** retirer S8 de la ligne des autorisations ou le noter « début de la reprise progressive ».

### 6. Les deux « familles de protocoles » : confusion, poids trompeur et regroupement décidé après coup

- **Fichiers et sections :** `01_synthese_SWiM.md` §2 (item 1), Tableaux 1 et 2, §8, message clé 2 ; `03_cadre_par_phases.md` §1.
- **Problème :**
  - **La famille B, c'est un seul réseau.** S1 et S2 viennent de la même base Xpert Clinics, avec un recoupement probable des patients. Écrire « Le protocole de S2 confirme celui de S1 » (§8) est circulaire : c'est le protocole standard du même réseau, pas une confirmation indépendante.
  - **Une étiquette contradictoire.** La famille B s'appelle « mobilisation précoce », mais elle contient le bras **tardif** de S1 (poignet aux semaines 5-6). Ce bras est proche de la famille A (6-8 semaines). Le vrai contraste porte sur les broches et la durée du plâtre.
  - **« Le protocole dépend de la chirurgie »** (message 2) est trop déterministe, et S1 le contredit. Pour la même 3LT, on trouve un plâtre de 6 semaines dans la description originale (« *the 3LT procedure is followed by immobilization in a cast for 6 weeks* », p. 1077), de 10-16 jours, puis de 3-5 jours. Le changement a été décidé en 2015 pour le confort des patients, pas à cause de la technique. Le protocole dépend donc aussi du centre et de l'époque.
  - **Un regroupement fait après coup.** Le §2 dit ces regroupements « prévus au protocole ». Or le protocole prévoyait « par famille de protocoles (p. ex. mobilisation avant ou après 6 semaines) » et des familles de techniques « greffe tendineuse, capsulodèse, *internal brace* ». La famille « stabilisation dynamique » et la coupure « avec broches / sans broches » ont été décidées après coup.
- **Pourquoi c'est important :**
  - « Deux familles » suggère deux traditions de même poids. En fait, on a d'un côté 6 études de 5 pays, de l'autre un seul réseau néerlandais.
  - Le message 2 sera lu comme une règle : « après une 3LT sans broches, une orthèse permet de bouger dès la 2e semaine ».
- **Correction :**
  - **Nommer :** « Parcours A : avec broches (6 études, 5 pays) » et « Parcours B : sans broches, **un seul réseau néerlandais** (S1, S2) ».
  - **Relativiser :** supprimer « confirme ».
  - **Message 2 :** « Le calendrier varie avec la présence de broches et selon les centres ; une même technique (3LT) a été suivie de plâtres de 3 jours à 6 semaines. »
  - **Déclarer :** présenter les regroupements comme décidés après coup ; montrer aussi le classement selon la coupure prévue au protocole (avant ou après 6 semaines).

### 7. Le cadre par phases franchit la ligne d'une recommandation officieuse

- **Fichier et sections :** `03_cadre_par_phases.md`, en entier (§1 à §5).
- **Problème :**
  - **Les avertissements sont là**, en tête du fichier, mais la **forme** est celle d'une *guideline* :
    - quatre phases nommées, chacune avec un « Objectif » sans étiquette de preuve (« Laisser la reconstruction cicatriser sans la mettre en tension ») ;
    - des lignes « Passage à la phase… » ;
    - une frise chronologique semaine par semaine.
  - **Un parcours composite.** La frise assemble des jalons tirés d'études différentes en un parcours que **personne n'a suivi** : la colonne 16-26 vient de S5 seul (« Charge complète à 16 sem. »), la colonne > 26 de S4 seul (7 patients, risque élevé, patients sélectionnés pour leur observance).
  - **Des titres prescriptifs :**
    - « Muscles à cibler » suppose qu'on doit cibler des muscles ;
    - « Signaux d'alerte rapportés (à signaler au chirurgien) » est une consigne ;
    - « Ce qu'on peut attendre à long terme » promet un résultat au patient.
  - **Une liste d'alerte incomplète.** Pas de SDRC, de troubles vasculo-nerveux ni de problème de plâtre. « Problèmes liés aux broches : Non rapportés » peut se lire « il n'y en a pas ».
  - **Un biais du survivant.** « Ce qu'on peut attendre » s'appuie sur des séries avec beaucoup de perdus de vue : S4 7 sur 56, S5 36 sur 54, S8 24 sur 40, et les 2 échecs de S8 sont retirés des comparaisons cliniques.
  - **Une étiquette trompeuse.** « [Preuve directe : S…] » est apposée sur de simples **pratiques rapportées**, par exemple « Poignet en position neutre [Preuve directe : S5, S6] ». Pour un lecteur, « preuve » veut dire « démontré efficace ».
- **Pourquoi c'est important :**
  - Le protocole exige que le cadre ne soit « jamais présenté comme une recommandation officielle », et le point de contrôle 1 (DA-7) avait signalé le risque d'une lecture comme prescription.
  - Un tableau extrait seul perd l'avertissement du haut.
- **Correction :**
  - **Titre :** « Ce que décrivent les études, étape par étape (synthèse descriptive, non testée) ».
  - **Lignes « Objectif » :** les supprimer ou les étiqueter « [Synthèse des auteurs] ».
  - **Frise :** la remplacer par un tableau **une ligne par étude** (étude, n, risque de biais, broches, délais), ou indiquer dans chaque cellule « S5 seulement, n = 36 ».
  - **Étiquettes :** remplacer « Preuve directe » par « **Pratique rapportée (S…, n = …)** » pour les descriptions, et garder « Preuve comparative (S1, GRADE très faible) » pour la seule comparaison.
  - **Titres prescriptifs :**
    - « Muscles à cibler » devient « Muscles évoqués par des experts (non testé chez des opérés) » ;
    - le §4 devient « Complications rapportées dans les études incluses (liste non exhaustive : tout symptôme inquiétant se signale à l'équipe soignante) » ;
    - le §3 devient « Résultats au dernier suivi, chez les patients revus seulement », avec la part des perdus de vue.
  - **Avertissement :** le répéter sous la frise.

### 8. Contrainte UC-003 et sources de contexte : transposition, conclusions sans fondement et une étude éligible citée comme « contexte »

- **Fichier et sections :** `03_cadre_par_phases.md`, en-tête, Phase 2 (lancer de fléchette), Phase 3 (muscles, proprioception), Phase 4 et §3.
- **Problème :**
  1. **UC-003 relue de façon trop étroite.** Le cadre affirme : « Aucune donnée n'est empruntée à une autre pathologie du poignet (contrainte UC-003) ». Mais le protocole définit UC-003 comme « pas de preuves transposées : population limitée aux patients opérés », et le RQ Brief verrouille la sous-question 3 : « Déviation : aucune (preuves transposées refusées) ».
     - C11 (cadavres, ligament coupé), C14 (2 poignets de cadavre), C15 (revue d'experts fondée sur des cadavres, poignet natif) et C16 (étude expérimentale) ne portent pas sur des opérés. Ils sont pourtant utilisés pour le contenu de la rééducation.
  2. **Lancer de fléchette.** La phrase « dans un poignet dont le ligament SL est coupé, les os du carpe restent mal alignés pendant ce mouvement… On ne peut donc pas affirmer qu'il protège la reconstruction » ne suit pas. Un poignet sectionné **non reconstruit** ne dit rien de la charge sur une reconstruction.
     - Le point de contrôle 1 (DA-5) demandait de présenter le désaccord sur ce mouvement (« Bergner 2020 vs Schriever 2021 »). Seule la source défavorable est citée.
  3. **Proprioception.** « Le ligament SL contient des mécanorécepteurs [C13, C14], ce qui **justifie** l'idée d'un travail proprioceptif » va trop loin.
     - Après reconstruction, le ligament natif est souvent remplacé ou renforcé par un tendon.
     - Selon son résumé, C13 montre que les mécanorécepteurs **diminuent avec le temps écoulé depuis la lésion**. Or la plupart des patients inclus sont chroniques (S1 : 10-11 mois de symptômes).
  4. **Sources lues en résumé seulement.** Toutes les sources C… sont « résumé seulement » (en-tête de `bibliographie_contexte.md`), ce que le cadre ne dit pas.
  5. **Une étude éligible citée comme « contexte ».** C43 (Abola 2026, 9 % de gestes secondaires) est **R00173**, une notice retenue au tri sur titre et résumé puis non récupérée. Elle entre dans la synthèse comme « cohorte de contexte », sans évaluation du risque de biais.
  6. **Étiquettes absentes de la légende.** « [revue systématique de contexte : C44] » et « [cohorte de contexte : C43] » ne figurent pas dans la légende.
- **Pourquoi c'est important :** c'est une contrainte explicite de l'auteur. Des données sur cadavre, présentées en face de « Muscles à cibler », sont exactement le type de preuve transposée que l'auteur a refusé.
- **Correction :**
  - **UC-003 :**
    - déplacer C11 et C13 à C16 dans le chapitre de contexte (sous-question 1, où l'élargissement de population a été approuvé) ;
    - ou demander à l'auteur une dérogation écrite et étiqueter « [Hors population : cadavre ou avis d'experts ; non transposable aux opérés] ».
  - **Raisonnements :**
    - retirer « justifie » ;
    - retirer l'inférence tirée de C11 ou présenter les deux positions.
  - **C43 et légende :**
    - traiter R00173 par la méthode systématique, ou le retirer du cadre ;
    - ajouter les étiquettes manquantes à la légende.
  - **Lecture :** vérifier toutes les affirmations tirées des sources C… sur le texte intégral, comme promis dans la bibliographie.

### 9. La « principale lacune » a une autre explication : la façon dont les études sont rapportées, et l'échantillon

- **Fichiers et sections :** `01_synthese_SWiM.md` §6, Tableau 3, message 5 ; `03_cadre_par_phases.md` (lignes « Passage à la phase… »).
- **Problème :**
  - « 8 études sur 8 utilisent uniquement le temps… C'est la principale lacune mise en évidence par cette revue » peut venir, en grande partie, de la **construction de la revue**, et pas de la pratique :
    - les études incluses sont des articles chirurgicaux, où la rééducation tient en un paragraphe des Méthodes, décrite par convention en semaines ;
    - l'équation de recherche n'a volontairement aucun bloc « rééducation » ;
    - les publications non cliniques sont exclues (E1 = 233 et E2 = 86 au tri), donc les articles de thérapie de la main qui décrivent des programmes ;
    - CINAHL n'a pas été interrogée ;
    - les protocoles institutionnels repérés dans la littérature grise (Université de Virginie 2024, etc.) n'ont pas été examinés ;
    - et 59 rapports n'ont pas été lus.
  - « Aucun critère clinique n'a été **étudié** » dépasse les données : il n'a été **rapporté** dans aucune étude incluse.
  - **La lacune « proprioception » dépend de R00527.** Le §8 indique que son protocole comprend « un travail de mobilité, de force et de proprioception ». L'inclure changerait la ligne « S1 seulement » du Tableau 3 et le message 6.
- **Pourquoi c'est important :** c'est le constat présenté comme le principal apport de la revue.
- **Correction :**
  - **Formulation :** « Dans les 8 études lues, le passage d'une phase à l'autre n'est décrit que par le temps ou l'ablation du matériel. Cela peut refléter la façon dont les articles chirurgicaux décrivent la rééducation plutôt que la pratique ; aucun critère clinique n'a été comparé. »
  - **Littérature grise :** examiner les protocoles repérés, à titre d'illustration, en disant qu'ils ne sont pas une preuve.
  - **R00527 :** trancher la question avant de figer le Tableau 3 et le message 6.

### 10. Résultats à long terme et radiologie : une généralisation, une contradiction, des chiffres mal reportés

- **Fichiers et sections :** `01_synthese_SWiM.md`, message 7 et Tableau 4 ; `03_cadre_par_phases.md` §3.
- **Problème :**
  - **Contradiction.** Le message 7 dit « Une perte progressive de la correction… quelle que soit la technique ». Or le cadre §3 écrit « correction maintenue dans S3, S7 et S8 » : les deux techniques de réparation avec capsulodèse ne montrent pas de perte.
  - **S6 mal classé.** S6 ne montre pas une perte *progressive* : les seules valeurs sont celles d'avant l'opération et du dernier suivi (« *improved in average but remained in the pathologic range* »). La perte de réduction n'y est évoquée que pour un cas (cas 8).
  - **Autres explications non dites.** La perte observée dans S4 et S5 a d'autres explications possibles, que la synthèse ne nomme pas :
    - un suivi plus long (4-6 ans contre 17-26 mois pour S3 et S7) ;
    - une instabilité chronique statique (Garcia-Elias 4), avec une arthrose SLAC I dès l'opération chez 27 patients sur 36 dans S5 ;
    - des perdus de vue (S5 : 18 sur 54 ; S4 : 7 patients revus sur 56) ;
    - la méthode radiologique.
  - **Attribution.** La rééducation ne varie pas d'une étude à l'autre (toutes à immobilisation longue). On ne peut donc l'attribuer ni à la rééducation, ni à la technique.
  - **Chiffres de S2 :**
    - le cadre §3 reprend « 19 conversions sur 480 en 4,5 ans (S2) » **sans** la mention « tous stades confondus ». Ce chiffre inclut des SLAC 2-3 exclues par le protocole, alors que S2 donne le taux conforme au protocole : « *The conversion rate was 2.3% in SLAC 0 (n = 400)* » ;
    - « 9 % de chirurgies dans l'année chez les patients sans SLAC » (Tableau 4) n'est pas soutenu. S2 précise que, pour les complications de grade 3, « *a longer follow-up was established… up to 9 years* », et la ligne SLAC 0 du tableau 3 porte sur l'ensemble des SLAC 0 (n = 400), pas sur le sous-groupe de 95 patients.
- **Pourquoi c'est important :** « quelle que soit la technique » laisse croire que la perte de correction ne dépend pas de la technique, ce que les données ne permettent pas de dire. Les chiffres de S2 mélangent une population hors protocole.
- **Correction :**
  - **Message 7 :** « Une perte de correction radiologique est rapportée dans deux séries de greffes tendineuses pour instabilité chronique statique, avec 4 à 6 ans de suivi (S4, S5) ; la correction est maintenue dans trois autres études (suivi plus court ou lésions aiguës). Ces différences peuvent tenir au stade, au délai, au suivi ou aux perdus de vue ; aucune étude ne les relie à la rééducation. »
  - **S6 :** le retirer de la liste « perte progressive ».
  - **S2 :** utiliser 2,3 % (SLAC 0, n = 400) ; corriger « dans l'année ».

### 11. Extraction par IA seule : une erreur concrète est passée, et seules 12 données clés ont été extraites en double

- **Fichiers et sections :** `phase2/extraction/extraction_reconciliee_et_risque_biais.md` §6.1 ; tout le cadre.
- **Problème :**
  - La double extraction ne porte que sur **12 données clés par étude**. Les détails opérationnels du cadre (limites d'amplitude, port de l'orthèse, contenu des exercices) viennent d'une seule extraction.
  - L'erreur sur les 30° (constat n° 4) et les chiffres de S2 (constat n° 10) sont passés à travers.
  - Ma propre relecture est faite par une IA de la même famille de modèles : les erreurs peuvent être corrélées, et ce rapport ne remplace pas une vérification humaine.
- **Pourquoi c'est important :** le cadre présente des chiffres qu'un kinésithérapeute appliquera. Le protocole d'origine prévoyait que l'auteur vérifie 100 % des données des études comparatives. Ici, une seule étude est concernée, S1, soit 9 pages.
- **Correction :**
  - **Vérification humaine :** que l'auteur vérifie lui-même S1 en entier, puis chaque nombre des messages clés et du cadre à l'aide des localisateurs (environ 1 à 2 heures).
  - **À défaut :** écrire dans la déclaration de transparence que « les délais et restrictions du cadre proviennent d'une extraction IA unique, non vérifiée ».

---

## Constats mineurs

### 12. Analyses de sensibilité incomplètes ou inexactes

- **Fichier et section :** `01_synthese_SWiM.md` §8.
- **Problème :** « Sans S6… Les conclusions restent les mêmes » ne vaut que pour les délais. S6 apporte aussi :
  - le seul suivi de 12 ans ;
  - une des deux sources « 3 mois » pour les activités lourdes ;
  - des valeurs de mobilité et de force ;
  - une partie du message 7.
- **Problème (suite) :** aucune analyse n'est faite sans S7 (patients peut-être mineurs) ni pour R00527 sur la proprioception (constat n° 9).
- **Correction :** refaire le §8 résultat par résultat (délais, long terme, messages clés) ; ajouter les analyses sans S7 et avec R00527.

### 13. Écarts au protocole non déclarés

- **Fichiers :** protocole et phase 3.
- **Problème :**
  - Le protocole prévoit que « Les résultats sont regroupés par moment de mesure : < 6 mois, 6 à 12 mois, > 12 mois » ; le Tableau 4 regroupe par technique, « au dernier suivi ».
  - Le risque de biais devait être validé par l'auteur, et cet écart n'est pas couvert par les amendements du 2026-10-10.
  - La relecture de l'équation avec la checklist PRESS par l'avocat du diable, prévue au protocole, n'est documentée nulle part.
- **Correction :** ajouter ces points au tableau des amendements, ou appliquer le regroupement par fenêtre.

### 14. Effectif total surestimé

- **Fichier et section :** `01_synthese_SWiM.md` §3.
- **Problème :** « environ 300 patients au total » alors que S1 et S2 se recoupent. La somme fait 306, mais le recoupement peut aller jusqu'à 95 patients.
- **Correction :** « entre environ 210 et 306 patients ».

### 15. Échelle JBI : règle de synthèse non déclarée

- **Fichier :** extraction, §5.
- **Problème :** la checklist JBI ne produit pas, à elle seule, de niveau global « modéré » ou « élevé ». La règle utilisée pour passer des items au niveau global n'est pas dite (S3 a quatre « ? » et reste « modéré »).
- **Correction :** énoncer la règle, par exemple « élevé si au moins 2 N sur les items 4, 5 ou 7, ou n < 10 ».

### 16. S1, domaine D5 « Faible » pour le PRWHE : peut-être optimiste (inférence à vérifier)

- **Fichier :** extraction §5.
- **Problème :**
  - S1 n'inclut que des patients avec un PRWHE et une EVA complets avant l'opération et à 3 mois.
  - Il compte 167 opérés sur environ 4,8 ans, alors que S2, dans le même réseau, compte 480 3LT sur 8 ans.
  - S1 pourrait donc être un sous-ensemble de cas complets. C'est une inférence, pas un constat.
- **Correction :** noter cette incertitude dans D2 ou D5. Le GRADE ne change pas (déjà au plancher).

### 17. Retour au travail : dénominateurs et définitions mélangés

- **Fichier et section :** `03_cadre_par_phases.md`, Phase 4.
- **Problème :**
  - « 82-91 % des patients au travail à 3 mois [S1, n = 45] » porte sur 45 répondants sur 108, alors que 26-30 % des patients étaient sans emploi au départ (Tableau 1).
  - Le « 84 % ont repris leurs activités antérieures » de S7 désigne des *activités*, pas un retour au travail, et il est pourtant classé sous « Travail ».
- **Correction :** donner le dénominateur et la définition, et déplacer S7 sous « Activités ».

### 18. « Série de cas = faible » appliqué aux résultats

- **Fichiers :** SWiM, cadre et messages 2, 4, 7.
- **Problème :** l'étiquette « niveau faible » sert à la fois pour décrire une pratique (ce que les études ont fait) et pour des résultats non contrôlés (perte de correction, scores). Pour un résultat sans comparateur, la convention GRADE serait plutôt « très faible ».
- **Correction :** distinguer « pratique rapportée » (fait descriptif) et « résultat observé, non contrôlé (certitude très faible) ».

### 19. Lisibilité pour un public large (UC-008)

- **Fichiers :** tous ceux de la phase 3.
- **Problème :**
  - sigles non expliqués : 3LT, SLAC, SLIL, PRWHE, ECRB, APL, ECU, symboles ⊕ ;
  - l'avertissement n'apparaît qu'en tête du cadre ;
  - « Le kinésithérapeute peut s'en servir » est une consigne, même si elle est anodine.
- **Correction :** ajouter un glossaire, répéter l'avertissement près de chaque tableau chronologique et écrire au conditionnel descriptif.

---

## Observations (sans action requise)

- **Signes des tailles d'effet de S1.**
  - Pour le PRWHE, le groupe précoce a un résultat moins bon (37,5 contre 36,5) et la taille d'effet est **positive** (0,197).
  - Pour l'EVA en charge, le groupe précoce a aussi un résultat moins bon (39,5 contre 31,5), mais la taille d'effet est **négative** (-0,036).
  - Le sens de lecture des tailles d'effet est donc indéterminable, ce qui **renforce** l'encadré de l'extraction (« non concluant »).
- **Règle de non-infériorité de S1.** La règle inhabituelle est confirmée mot pour mot : « *Noninferiority was demonstrated if 1 side of the 95% confidence interval was outside the noninferiority margin* » (p. 1079).
- **Langues.** Cinq notices retenues au tri sur titre et résumé sont dans une langue hors liste. Leur sort n'est pas tracé dans les fichiers lus.
- **Littérature grise.** Les protocoles institutionnels repérés peuvent illustrer la pratique en discussion, à condition de rester hors de l'étiquette « preuve ».

---

## Ce qui est solide (*steel-man*)

1. **Rejet de la non-infériorité revendiquée par S1.** C'est le meilleur point du travail. L'encadré de l'extraction a repéré la règle inhabituelle et l'intervalle de confiance qui dépasse la marge. Je l'ai vérifié dans le texte, et le calcul de puissance le confirme (S1 était sous-dimensionnée). Beaucoup de revues publiées reprennent telle quelle la conclusion des auteurs.
2. **Décision de ne pas méta-analyser**, structure SWiM explicite et absence de comptage de « votes » sur les effets.
3. **Confusion entre broches, technique et centre reconnue noir sur blanc** (SWiM §7 : « l'effet des broches ne peut pas être séparé de celui de la technique ni du centre »), et la phrase de synthèse GRADE interdit l'extension aux reconstructions avec broches.
4. **Marquage des lacunes.** Le Tableau 3 (ce que les études ne rapportent pas) est très utile pour un public de kinésithérapeutes. Le long terme est marqué « Inconnu », et non extrapolé.
5. **Double extraction IA indépendante avec journal de réconciliation**, et détection puis correction de l'incident des tableaux manquants, avec relecture des décisions du tri sur texte intégral. Les autres chiffres que j'ai recoupés sont justes : complications de S1 (Tableau 2), protocoles de S3, S5, S6, S7 et S8, radiologie de S4 (2,0 → 4,2 mm ; 50° → 80°) et effectifs des études.
6. **Application rigoureuse du protocole sur S2** (sous-groupe sans SLAC) et sur S8 : la comparaison aigu contre subaigu y est reconnue comme un facteur pronostique, non coté par GRADE.
7. **Transparence.** Le recoupement S1/S2 est déclaré et les patients ne sont pas additionnés. L'arithmétique du PRISMA est cohérente (1 001 − 439 = 562 ; 562 − 487 = 75 ; 75 − 59 = 16 ; 16 − 7 − 1 = 8). La question de R00527 et de S6 est soumise à l'auteur au lieu d'être tranchée en silence. L'essai en cours NCT06590701 est signalé.
8. **Niveau GRADE final.** « Très faible » est probablement juste. Seules les justifications sont à reprendre (constat n° 2).

---

## Contre-argument le plus fort

> « Cette revue décrit en réalité les protocoles de 8 articles en libre accès, dont un quart viennent d'un seul réseau néerlandais. 59 rapports n'ont pas été cherchés, dont la seule autre étude comparative connue, pourtant gratuite sur PMC. Ses constats d'absence (une seule comparaison, aucun critère clinique, aucune recommandation) sont des effets de l'échantillon. Et son cadre par phases assemble des jalons d'études différentes, avec une erreur sur la limite de flexion, en un parcours que personne n'a suivi ni testé. »

## Ce qui manque

- **Textes non lus :** les 59 rapports, dont 17 gratuits, Kemler 2023 et Ying 2024.
- **Méthodes de recherche non faites :** recherche par citations en amont et en aval (prévue au protocole) ; TRIP ; CINAHL (la base la plus proche de la rééducation) ; Embase et Scopus.
- **Résultats absents :** aucune donnée sur la tenue radiologique de la reconstruction **sous mobilisation précoce** (le vrai risque du protocole précoce) ; aucune donnée sur les complications des broches, le SDRC ou la raideur sous les deux protocoles.
- **Autres dimensions :** le point de vue des patients, l'observance, le domicile comparé à la rééducation supervisée, le coût.
- **Pratique hors des articles chirurgicaux :** protocoles institutionnels et articles de thérapie de la main.

## Tests de résistance

| Test | Résultat |
|---|---|
| Retirer la source la plus forte (S1) : l'argument tient-il ? | **Non.** Le parcours B ne repose plus que sur S2, qui ne donne pas le début de la mobilisation du poignet ; il n'y a plus de comparaison ni de GRADE. |
| Inverser la question (« l'immobilisation longue est-elle préférable ? ») : la position opposée est-elle crédible ? | **Oui.** La description originale de la 3LT prévoit 6 semaines de plâtre, et il n'existe aucune donnée sur la tenue à long terme après mobilisation précoce. |
| Transposer à un autre contexte (kinésithérapeute généraliste francophone) : le constat se généralise-t-il ? | **Non.** Le parcours B vient d'un seul réseau, avec des thérapeutes de la main spécialisés ; le parcours A, de séries hétérogènes de 5 pays. |
| « Et alors ? » : la portée est-elle justifiée ? | **Oui, si le travail est requalifié.** Une cartographie honnête des pratiques rapportées et de leurs lacunes est utile ; une synthèse présentée comme exhaustive ne l'est pas. |

## Suivi du point de contrôle 1

| Point du CP1 | Statut au CP2 |
|---|---|
| SR-1 (un seul relecteur humain) | **Aggravé** (aucun relecteur humain), mais déclaré. Le constat n° 11 donne une raison concrète de faire une vérification minimale. |
| SR-2 (confusion entre protocole et résultat) | **Respecté** dans la synthèse (§4-§7) ; **dérive** dans le cadre §3 (« Ce qu'on peut attendre ») et dans le message 7. |
| SR-3 (couverture des bases) | **Non tenu :** la recherche par citations promise en compensation n'a pas été faite (constat n° 1). |
| SR-4 (pilote de 50 notices) | Supprimé par amendement (déclaré). |
| DA-5 (présenter le désaccord sur le lancer de fléchette) | **Non tenu :** une seule source, défavorable (constat n° 8). |
| DA-7 (un plan type peut être lu comme une prescription) | **Partiel :** l'avertissement est en tête du fichier, mais la forme reste prescriptive (constat n° 7). |
| DA-8 (recommandations actuelles) | **Partiel :** recherche provisoire, TRIP non faite (constat n° 1). |
| Relecture PRESS par l'avocat du diable (protocole) | **Non documentée** (constat n° 13). |

## Note sur mes propres biais

Je suis une instance d'IA de la même famille que les relecteurs, les extracteurs et les rédacteurs de cette revue : mes erreurs peuvent être corrélées aux leurs. J'ai vérifié S1 en entier et des passages ciblés de S2 à S8, pas chaque donnée. Les calculs de puissance (constat n° 2) et l'ordre de grandeur des études manquantes (constat n° 1) sont mes propres estimations ; ils sont signalés comme tels.


---

# Réponse aux constats (session principale, 2026-10-11)

Les corrections ont été faites dans les fichiers de la phase 3, l'extraction réconciliée, le protocole (amendements) et la déclaration de transparence. Le contrôle de fidélité aux sources, mené en parallèle, a trouvé 23 écarts ; ils sont tous corrigés.

| N° | Sévérité | Statut | Ce qui a été fait |
|---|---|---|---|
| 1 | Critique | **Ouvert : décision de l'auteur** | Récupération automatique des 17 textes gratuits sur PMC tentée par Europe PMC (texte XML, PDF), NCBI (efetch, BioC) et le site de l'éditeur : **tous bloqués** (articles hors du sous-ensemble en libre accès ; protection anti-robots). Il faut un lecteur humain. En attendant, l'option B est appliquée à titre provisoire : chaque affirmation d'absence ou d'unicité est bornée aux « 8 études lues », le motif du PRISMA est corrigé, le biais de publication est « suspecté » dans le GRADE, la phrase de synthèse cite Kemler 2023 comme non lue, et les recommandations sont dites « provisoires, TRIP non interrogée ». **Choix soumis à l'auteur :** (A) télécharger les 17 textes (et Ying 2024 si possible), puis tri, extraction et synthèse mis à jour ; ou (B) garder l'option (a) et requalifier le titre |
| 2 | Majeur | Corrigé | Population large et caractère indirect motivé par la technique et le lieu de la rééducation ; imprécision motivée par l'intervalle de confiance et la puissance (calcul indicatif : environ 100-128 patients par groupe nécessaires) ; biais de publication suspecté ; complications notées comme nombres d'événements, avec les 2 opérations du TFCC ; énoncés selon Santesso 2020 ; références GRADE ; vérification avec l'approche GRADE 18 (même niveau final) |
| 3 | Majeur | Corrigé | Message 3 réécrit ; « retour au poste d'origine » (56 % contre 76 %) ajouté au tableau 5 et au GRADE ; conclusion « on ne peut pas en conclure que la mobilisation précoce est sûre » ; absence de radiologie dans S1 signalée |
| 4 | Majeur | Corrigé | « Flexion portée jusqu'à 30° à partir de la semaine 5 » ; C38 retirée du cadre (contrainte UC-003) |
| 5 | Majeur | Corrigé | Message 4 réécrit ; plus de médiane pour les délais de définitions différentes (une ligne par étude) ; S8 noté « début d'une reprise progressive » |
| 6 | Majeur | Corrigé | « Parcours A : avec broches (6 études, au moins 5 pays) » et « Parcours B : sans broches, un seul réseau néerlandais » ; regroupements déclarés comme décidés après coup ; tableau 1 bis selon la coupure du protocole ; « confirme » retiré ; message 2 réécrit (broches, centre, époque) |
| 7 | Majeur | Corrigé | Titre « Ce que décrivent les études, étape par étape (synthèse descriptive, non testée) » ; frise composite remplacée par un tableau d'une ligne par étude (n, risque de biais) ; étiquettes « Pratique rapportée » et « Résultat observé, non contrôlé » ; objectifs marqués « Synthèse des auteurs » ; sections 3 et 4 renommées (patients revus seulement ; liste non exhaustive) ; avertissements répétés |
| 8 | Majeur | Corrigé (en partie) | Sources de laboratoire et avis d'experts hors patients opérés retirés du cadre (UC-003), renvoyés au chapitre de contexte ; C43 (= R00173, rapport éligible non lu) retirée ; étiquette « Contexte, lu en résumé » ajoutée à la légende. **Reste à faire à l'étape 2** : lire en texte intégral les sources C… citées, et présenter les deux positions sur le lancer de fléchette dans le chapitre de contexte (point DA-5 du CP1) |
| 9 | Majeur | Corrigé (en partie) | Constat borné aux 8 études lues ; « rapporté » au lieu de « étudié » ; autre explication (façon de décrire la rééducation dans les articles chirurgicaux) ajoutée. Examen des protocoles de littérature grise à titre d'illustration : **non fait** (proposé pour l'étape 2) |
| 10 | Majeur | Corrigé | Message 7 réécrit ; S6 retiré de la « perte progressive » ; explications concurrentes nommées ; S2 : 2,3 % de conversions chez les SLAC 0 (n = 400) |
| 11 | Majeur | Corrigé (transparence) ; **vérification humaine proposée à l'auteur** | Déclaration de transparence complétée : extraction unique pour les détails des protocoles, et relectures IA de la même famille de modèles. L'auteur peut choisir de vérifier S1 et les chiffres des messages clés (environ 1 à 2 heures) |
| 12 | Mineur | Corrigé | Analyses de sensibilité résultat par résultat ; ajout de l'analyse sans S7 ; R00527 en attente |
| 13 | Mineur | Déclaré | Six écarts au protocole ajoutés aux amendements, **à valider par l'auteur** |
| 14 | Mineur | Corrigé | « Entre environ 210 et 306 patients » |
| 15 | Mineur | Corrigé | Règle de synthèse JBI énoncée (formulée après coup, déclarée) |
| 16 | Mineur | Noté | Réserve ajoutée au domaine D5 de S1 |
| 17 | Mineur | Corrigé | Dénominateurs et définitions du retour au travail ; S7 déplacé sous « autres activités » |
| 18 | Mineur | Corrigé | Distinction entre pratique rapportée et résultat observé non contrôlé (certitude très faible) |
| 19 | Mineur | Corrigé | Glossaire ajouté à la synthèse ; avertissements répétés ; formulations descriptives |
| Obs. | — | Tracé | Les 5 notices « hors langue » sont de **faux signalements**. Pour 18 notices venues d'Europe PMC, une erreur de lecture du fichier CSV (guillemets dans le résumé) a décalé les champs, et du texte du résumé s'est retrouvé dans le champ « langue ». Les 5 notices sont en anglais et font partie des rapports non lus. Les 13 notices touchées qui ont été exclues ont été relues sur leur titre et leur motif : aucune décision ne change (notes techniques, revues, études cadavériques, autres pathologies) |

**Statut du point de contrôle 2 après corrections :** les constats majeurs et mineurs sont traités. Le **constat critique n° 1 reste ouvert** jusqu'à la décision de l'auteur (A ou B). L'avocat du diable refera une vérification après cette décision.
