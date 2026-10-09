# Guide du pilote : ce que j'attends de toi

## 1. Pourquoi ce pilote existe

Le tri des 562 notices est fait par **deux relecteurs IA indépendants**, plus un troisième qui arbitre leurs désaccords. Une IA peut toutefois mal comprendre une règle, par exemple exclure une étude chirurgicale parce que le résumé ne parle pas de rééducation.

Le pilote vérifie cela **avant** le tri complet. Sur un échantillon de **182 notices**, toi et les relecteurs IA classez les mêmes notices, chacun de votre côté. On compare ensuite.

**Règle de `sr-screener` :** le tri complet ne démarre que si l'IA n'a exclu **aucune** notice que toi tu gardes. Si elle en a raté, on corrige la formulation des règles et on refait le pilote. Toute correction est notée dans le journal des amendements.

C'est aussi ce qui rend la méthode défendable devant un jury. Dans la section Méthodes, tu pourras écrire que le tri automatisé a été calibré sur un échantillon classé par l'auteur, avec la sensibilité mesurée.

## 2. Ce que tu dois faire, concrètement

**Les fichiers :**
- `pilote_liste_titres.md` : les 182 titres numérotés de 1 à 182, en tableau. **Commence par là.**
- `pilote_titres_resumes.md` : les mêmes notices avec leur résumé. Ouvre-le seulement quand le titre ne suffit pas.

**Pour chaque notice, une décision :**

| Décision | Quand |
|---|---|
| **Garder** | Étude clinique sur des **patients opérés** d'une réparation ou reconstruction du ligament scapho-lunaire, qui rapporte des résultats |
| **Incertain** | Ça pourrait correspondre, mais le titre et le résumé ne permettent pas d'être sûr. Exemples : technique non nommée, cohorte mélangeant SL et autre ligament, pas de résumé mais un titre prometteur, réparation SL faite pendant l'opération d'une fracture du radius |
| **Exclure** | Tout le reste, et c'est la grande majorité |

**Les trois questions à te poser, dans l'ordre :**
1. **Est-ce une étude sur des patients ?** Si c'est une revue, un éditorial, une note technique sans patients, un cas isolé (1 à 4 patients), ou une étude sur cadavre, biomécanique ou modèle informatique : **exclure**.
2. **Est-ce le ligament scapho-lunaire, chez l'adulte ?** Si c'est une fracture du scaphoïde, le TFCC, le ligament luno-triquétral, une luxation péri-lunaire, un poignet SLAC traité par arthrodèse ou résection, ou des enfants seulement : **exclure**.
3. **Les patients ont-ils été opérés par réparation, ligamentoplastie, ténodèse, capsulodèse ou *internal brace* ?** Oui : **garder**. Pas sûr : **incertain**. Non : **exclure**. « Non » couvre le traitement conservateur, le diagnostic ou l'imagerie seuls, le débridement seul et les broches ou la vis seules sans geste sur le ligament.

⚠️ **Le piège principal : la rééducation n'a PAS besoin d'être mentionnée dans le résumé.** Une étude « Résultats à 5 ans de la ténodèse à trois ligaments » doit être **gardée**, même sans un mot sur la rééducation. On vérifiera la rééducation au second tri, sur le texte complet.

En cas d'hésitation entre garder et exclure, choisis **incertain**. Rater une étude pertinente est plus grave que d'en vérifier une de trop.

## 3. Les règles d'indépendance (importantes pour la validité)

- **Je ne te montrerai pas les décisions de l'IA** avant que tu m'aies envoyé les tiennes.
- **Ne cherche pas l'article ailleurs** (Google, PubMed) : juge uniquement ce qui est écrit dans la liste, comme les relecteurs IA.
- **Ne me demande pas mon avis sur une notice précise** pendant le classement, cela biaiserait la comparaison. Tu peux en revanche me poser une question sur **une règle en général** (par exemple « une capsulodèse seule compte-t-elle ? »).
- **Une fois envoyées, tes réponses sont figées.** Le fichier est enregistré avec une empreinte, et tu ne pourras pas les modifier après avoir vu les résultats de l'IA.

## 4. Comment me répondre

Envoie seulement les numéros que tu **gardes** et ceux qui sont **incertains**. Tout le reste est compté comme **exclu**.

> **Garder :** 3, 17, 45, …
> **Incertain :** 12, 88, …
> **(tout le reste exclu)**

Tu peux répondre **en plusieurs messages**, par exemple « Partie 1/3 (notices 1 à 60) : … ». Je ne lancerai la comparaison qu'après la dernière partie.

Les codes d'exclusion (E1, E2…) ne sont **pas obligatoires**. Tes exclusions seront enregistrées comme « exclu par l'auteur, motif non codé ». Seule la distinction garder ou exclure sert à la comparaison.

**Durée estimée : 1 h à 1 h 30.** La plupart des titres sont clairement hors sujet et se décident en quelques secondes.

## 5. Ce qui se passe ensuite

1. J'enregistre tes réponses dans `pilot_labels.csv` (auteur : Maes) et je lance la comparaison.
2. **Si l'IA n'a raté aucune notice que tu gardes**, je te montre l'accord entre vous (sensibilité, kappa). Je lance ensuite le tri complet des 380 notices restantes, l'arbitrage, et le contrôle qualité obligatoire : un relecteur IA senior revérifie 100 exclusions communes tirées au sort, plus les exclusions « limites ».
3. **Si l'IA en a raté**, on regarde ensemble pourquoi, on corrige la formulation de la règle (amendement daté), et on refait le pilote sur les mêmes notices.
4. **Ton second rôle, après le tri complet** : vérifier **toutes** les notices retenues et un échantillon des exclusions. C'est une règle de `sr-screener` : les décisions finales appartiennent à l'auteur, l'IA aide à décider.
5. Ensuite viennent les textes intégraux : je récupère ceux en accès libre et je te donne la liste des autres à obtenir via ta bibliothèque.
