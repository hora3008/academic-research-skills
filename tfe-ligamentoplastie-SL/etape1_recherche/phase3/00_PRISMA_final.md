# Diagramme de flux PRISMA 2020 (final)

> Nombres issus de `sr-screener` (`../phase2/tri/Screening_TA/TA_prisma_counts.json` et `../phase2/tri/Screening_FT/FT_prisma_counts.json`), arrêtés au 2026-10-11.
> Si l'auteur modifie une décision de tri (question R00527, voir `../phase2/extraction/extraction_reconciliee_et_risque_biais.md`, section 7), ce diagramme sera mis à jour.

```mermaid
flowchart TD
  subgraph ID["Identification"]
    A["Notices identifiées dans les bases (n = 1 001)<br/>PubMed/MEDLINE 531 · Europe PMC 466 · PEDro 4"]
    R["Enregistrements de registres (n = 48)<br/>ClinicalTrials.gov"]
    D["Notices retirées avant le tri :<br/>doublons (n = 439)"]
  end
  subgraph TRI["Tri"]
    S["Notices triées sur titre et résumé (n = 562)"]
    X1["Notices exclues (n = 487)<br/>E1 type de publication 233<br/>E2 pas une étude clinique 86<br/>E3 population 156<br/>E4 intervention 11<br/>E9 autre 1"]
    F["Rapports recherchés en texte intégral (n = 75)"]
    N["Rapports non récupérés (n = 59)<br/>pas d'accès libre ou téléchargement bloqué"]
    E["Rapports évalués sur texte intégral (n = 16)"]
    X2["Rapports exclus (n = 7)<br/>E1 note technique sans patients 1<br/>E3 population (fractures du radius) 1<br/>E4 pas de geste ligamentaire 2<br/>E5 protocole post-opératoire insuffisant 3"]
    U["En attente de classement (n = 1)<br/>âge des patients non rapporté"]
  end
  subgraph INC["Inclus"]
    I["Études incluses dans la revue (n = 8)<br/>rapports : 8"]
    O["Études en cours (registres) : 7 enregistrements<br/>pertinents, traités à part (non inclus)"]
  end
  A --> D
  A --> S
  S --> X1
  S --> F
  F --> N
  F --> E
  E --> X2
  E --> U
  E --> I
  R --> O
```

## Remarques à reporter dans les Méthodes et la Discussion

1. **Bases non interrogées** : Embase, Scopus, Web of Science, CINAHL et Cochrane CENTRAL (pas d'accès).
2. **Textes non récupérés** : 59 sur 75 (79 %). C'est la principale limite de la revue.
   - Seuls les textes en accès libre ont pu être lus (biais d'accès libre).
   - Deux des trois études témoins (Kemler 2023, Ying 2024) en font partie.
3. **Sélection par IA sans vérification humaine** (voir `../phase2/declaration_tri_IA.md`).
4. **Recoupement de populations** : S1 (Bakker 2022) et S2 (Dullemans 2024) viennent de la même base de données néerlandaise. Elles sont comptées comme deux études, mais leurs patients ne sont pas additionnés.
5. **Registres** : les 48 enregistrements de ClinicalTrials.gov ont été examinés par un seul relecteur IA, en dehors de `sr-screener`. Sept concernent directement le sujet, dont **NCT06590701**, un essai en cours qui compare le mouvement de lancer de fléchette précoce à une mobilisation dans les plans anatomiques après reconstruction SL. Aucun n'a de résultats publiés à cette date.
