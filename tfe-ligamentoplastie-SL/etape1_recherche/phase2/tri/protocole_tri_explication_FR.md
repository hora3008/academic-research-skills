# Protocole de tri : explication en français (à valider par Maes)

> Le fichier `screening_protocol.md` (en anglais) est **le texte exact que recevront les relecteurs IA**. Il ne sera jamais paraphrasé dans les consignes. Ce document-ci en donne le sens en français, avec des exemples et les questions ouvertes. **Aucune notice n'est triée avant ta confirmation** (règle de fer de `sr-screener`).

---

## 1. Les règles en clair

**On garde au premier tri (titre + résumé)** toute étude clinique sur des patients opérés d'une **réparation ou reconstruction du ligament scapho-lunaire**, qui rapporte des résultats.
**Il n'est pas nécessaire que la rééducation soit citée dans le résumé** : la plupart des études chirurgicales décrivent leur protocole post-opératoire seulement dans le texte complet. C'est au second tri (texte intégral) qu'on vérifiera que le protocole est décrit.

**Techniques qui comptent :** réparation directe ou par ancres, ligamentoplasties avec greffe (Brunelli, 3LT, SLAM, SLIC…), capsulodèses (Blatt, Berger, Viegas, Mathoulin…), *internal brace*, combinaisons, avec ou sans broches.
**Ne comptent pas :** débridement arthroscopique seul, rétraction thermique seule, dénervation, chirurgies de sauvetage (résection de la première rangée, arthrodèses), imagerie ou diagnostic seuls.

**Motifs d'exclusion, dans l'ordre où ils sont vérifiés :**

| Code | Motif |
|---|---|
| E1 | Type de publication : revue, éditorial, lettre, note technique sans patients, cas clinique de 1 à 4 patients, enquête auprès de praticiens… |
| E2 | Pas une étude clinique : cadavre, biomécanique, animal, modélisation |
| E3 | Population : pas une lésion SL de l'adulte (autre ligament, fracture du scaphoïde, luxation péri-lunaire, SLAC en chirurgie de sauvetage, enfants) |
| E4 | Intervention : la lésion SL n'est pas opérée par réparation ou reconstruction (traitement conservateur, diagnostic, débridement seul…) |
| E9 | Autre motif (expliqué) |

**« Incertain »** (la notice passe au texte intégral) : technique non nommée, cohortes mixtes (SL + autre ligament), adultes et adolescents mélangés, nombre de patients non indiqué, pas de résumé mais un titre prometteur, et les trois cas limites de la question 1 ci-dessous.

## 2. Cas limites fictifs (pour vérifier qu'on se comprend)

| # | Notice fictive | Décision attendue | Ce que le cas teste |
|---|---|---|---|
| 1 | « Résultats à 5 ans de la ténodèse à trois ligaments chez 45 patients avec dissociation SL chronique » | **Garder (INC)** | La rééducation n'est pas citée, mais l'étude est retenue |
| 2 | « Reconstruction ligamentaire du poignet : notre expérience » (pas de résumé) | **Incertain (UNC)** | Notice sans résumé |
| 3 | « Instabilité scapho-lunaire : revue narrative des techniques de reconstruction » | **Exclure E1** | Revue |
| 4 | « Comparaison biomécanique du SLAM et de la 3LT sur poignets cadavériques » | **Exclure E2** | Cadavre |
| 5 | « Arthrodèse des quatre os pour poignet SLAC stade III : 60 patients » | **Exclure E3** | Chirurgie de sauvetage |
| 6 | « Programme d'exercices proprioceptifs pour l'instabilité SL dynamique : essai randomisé » | **Exclure E4** | Patients non opérés (pas de preuves transposées) |

Si tu n'es pas d'accord avec une décision attendue, dis-le : les règles seront reformulées.

## 3. Études témoins (*seeds*)

Trois études que l'on sait éligibles servent à tester la recherche et les règles. Les trois ont bien été **retrouvées** par la recherche :
- Bakker 2022 (mobilisation précoce vs tardive après 3LT) → notice R00269
- Kemler 2023 (reconstruction sans immobilisation) → R00156
- Ying 2024 (greffe de long palmaire + rééducation accélérée) → R00090

Si l'IA en exclut une pendant le pilote, ce sont les règles qui posent problème, et on corrige avant le tri complet.

## 4. Questions ouvertes (5 au maximum)

1. **Trois cas limites d'intervention.** Ils passent au texte intégral comme « incertains », mais il faudra trancher au second tri. Mes propositions :
   - (a) stabilisation **sans geste ligamentaire** (RASL, vis scapho-lunaire seule) : **exclure**, ce n'est pas une reconstruction du ligament ;
   - (b) réparation SL faite **pendant l'ostéosynthèse d'une fracture du radius** : **exclure**, sauf si un protocole propre au SL est rapporté séparément, car la rééducation est alors dictée par la fracture ;
   - (c) débridement ou rétraction thermique seuls : **exclure (E4)**.
2. **Les 6 cas limites ci-dessus** : d'accord avec les décisions attendues ?
3. **Les 3 études témoins** : d'accord ?
4. **Le pilote.** La règle de `sr-screener` impose qu'avant le tri complet, **tu classes toi-même un échantillon de notices** (environ 130 à 220, choisies par le script, études témoins comprises). On compare ensuite avec les décisions des relecteurs IA. Le tri complet ne démarre que si l'IA n'a exclu **aucune** notice que tu gardes.
   - La plupart des notices sont clairement hors sujet et se classent en quelques secondes.
   - Je te fournirai une liste numérotée. Tu me réponds simplement avec les numéros à garder.
   - Alternative possible mais plus faible : démarrer sans pilote humain. La raison est alors enregistrée et apparaît dans la section Méthodes.
5. **Le coût.** Avant chaque lancement, je te montrerai l'estimation du nombre d'appels IA et tu donneras ton accord. Estimation actuelle pour le tri des titres et résumés : environ 13 lots × 2 relecteurs, plus l'arbitrage et le contrôle qualité, soit **une cinquantaine d'appels**.
