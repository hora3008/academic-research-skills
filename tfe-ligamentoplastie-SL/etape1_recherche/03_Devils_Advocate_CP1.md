# Étape 1 · Phase 1 : Avocat du diable, point de contrôle 1

> `devils_advocate_agent` : relecture critique du cadrage avant la recherche bibliographique.
> Échelle : Critical (bloque) · Major (à régler avant la phase 2) · Minor (à garder en tête)

---

## A. Premier passage (cadrage large, v1 et v2) : résumé

| # | Objection | Résolution |
|---|---|---|
| DA-1 | Ambiguïté du terme « méthode de Berger » : il désigne surtout une capsulodèse dorsale ouverte [Terras 2025] ou une voie d'abord dorsale qui épargne les ligaments, alors qu'une « ligamentoplastie » implique en général une greffe tendineuse | **Résolu** : le périmètre couvre explicitement les techniques combinant reconstruction ligamentaire et capsulodèse dorsale, ainsi que les deux familles de protocoles (immobilisation prolongée avec broches, mobilisation précoce) |
| DA-2 | Preuves directes minces sur la rééducation post-opératoire | Étiquetage du niveau de preuve ; marquage [Lacune] |
| DA-3 | La borne ≥ 2020 exclut des travaux fondateurs | **Résolu** : règle d'exception UC-002 |
| DA-4 | Transposition depuis le traitement conservateur | **Résolu** : preuves transposées exclues (UC-003) |
| DA-5 | Biais de confirmation : risque de privilégier un protocole connu | Présenter les protocoles alternatifs et les désaccords (p. ex. le DTM : Bergner 2020 vs Schriever 2021) |
| DA-7 | Un plan « type » peut être lu comme une prescription | Avertissement médical ; repères plutôt que prescriptions |
| DA-8 | « Guidelines actuelles » : aucune recommandation officielle trouvée à ce stade | Recherche ciblée des recommandations officielles ; si aucune n'existe, le dire clairement |

Verdict du premier passage : **PASS**.

---

## B. Point de contrôle 1, mode revue systématique (protocole PRISMA-P v1.0)

Questions imposées par le protocole de la bibliothèque : la question PICOS est-elle assez précise ? La stratégie de recherche est-elle assez complète ? Le protocole est-il complet ?

### Version la plus forte du projet (*steel-man*)

Une revue systématique des **protocoles de rééducation rapportés** comble un vrai manque. Inclure les études chirurgicales qui décrivent leur protocole post-opératoire, et pas seulement les rares études comparant deux protocoles, donne un corpus suffisant pour décrire la pratique actuelle et les critères de progression.

### Objections

| # | Sévérité | Objection | Ce qu'il faut faire |
|---|---|---|---|
| SR-1 | **Major** | **Un seul relecteur humain.** Les standards (Cochrane, AMSTAR 2) attendent une sélection en double par des humains. Les relecteurs IA de `sr-screener` assistent mais ne remplacent pas un second humain. | Le déclarer comme limite. Idéalement, un camarade trie 20 % des notices en double, avec un kappa rapporté. Choix de l'auteur. |
| SR-2 | **Major** | **Confusion protocole / résultat.** Dans les études à un bras, le résultat dépend de la technique, du patient et du chirurgien autant que du protocole. | Synthèse descriptive ; aucune conclusion causale tirée des séries de cas ; GRADE réservé aux comparaisons. Déjà prévu dans le protocole. |
| SR-3 | **Major** | **Couverture des bases.** Sans Embase, Scopus, CINAHL ni Cochrane CENTRAL, une partie de la littérature (revues de rééducation, revues européennes) peut manquer. | Demander à l'auteur s'il a accès à ces bases via son école (exports). Sinon, le déclarer comme limite, en compensant par Europe PMC, PEDro et la recherche par citations. |
| SR-4 | Major | **Équation sans bloc « rééducation ».** Le choix est justifié (protocoles décrits seulement dans le texte intégral), mais il augmente le volume à trier et dépend d'un tri en texte intégral rigoureux. | Accepté ; pilote de 50 notices et contrôle qualité des exclusions. |
| SR-5 | Minor | **Borne 2020-2026** : des études de rééducation plus anciennes, éventuellement de meilleure qualité, sont exclues de la partie systématique. | Décision de l'auteur (UC-001), déclarée dans les limites ; la discussion peut les mentionner via des sources récentes qui les citent. |
| SR-6 | Minor | **Seuil de 5 patients** pour les séries de cas : arbitraire. | Le justifier (exclure les cas cliniques) et le garder fixe. |
| SR-7 | Minor | **Protocole non enregistré** : risque de reproche pour modification non déclarée. | Enregistrement OSF possible (choix de l'auteur) ; sinon, figer la version et tenir le tableau des amendements. |
| SR-8 | Minor | **Hétérogénéité des mesures de résultat** (PRWE, DASH, Mayo…), ce qui empêche probablement une méta-analyse. | Prévu : synthèse narrative selon SWiM. |

### Questions de contrôle

- *PICOS assez précis ?* Oui pour P, I et S. Le C « aucun » est assumé pour un objectif descriptif.
- *La méthode répond-elle à la question ?* Oui : la question principale est descriptive et comparative quand c'est possible.
- *Biais vers une réponse souhaitée ?* Risque DA-5, géré par l'inclusion de toutes les familles de protocoles.

### Verdict

**PASS sous conditions.** Aucun point Critical. Avant la phase 2, l'auteur doit trancher les ⟨choix⟩ du protocole : enregistrement, second relecteur, accès aux bases, exceptions antérieures à 2020 pour les études incluses, niveau de vérification des extractions.
