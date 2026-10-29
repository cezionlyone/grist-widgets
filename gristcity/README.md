# Gristcity

Un widget personnalisé pour [Grist](https://www.getgrist.com) qui dessine une table sous la forme d'une ville en 3D isométrique.

Chaque ligne devient un immeuble qui se construit au fil de ses étapes : terrain réservé, chantier, immeuble terminé, gratte-ciel... Les quartiers regroupent les immeubles selon une colonne de votre choix. Une météo signale ce qui est à surveiller (nuage) ou en alerte (orage).

Tout se paramètre dans le widget, sans toucher au code.

<img width="2880" height="1640" alt="image" src="https://github.com/user-attachments/assets/1aadd5bc-9a52-4120-b869-de503a10d845" />

## Six univers

| Univers | Chaque ligne devient | Idéal pour |
|---|---|---|
| 🏙️ Ville | un immeuble | des projets, des demandes, des dossiers |
| 🌳 Jardin | une plante | des parcours de personnes, des formations |
| 🚗 Garage | un véhicule | un parc automobile, du matériel |
| ✈️ Aéroport | un avion | des missions, des déplacements |
| 🚀 Base spatiale | une fusée | des idées, de l'innovation |
| ⚓ Port | un navire | des programmes, des partenariats |



## Installation

1. Dans votre document Grist, ajoutez une vue de type **Personnalisée**.
2. Choisissez l'**URL personnalisée** et collez :
   `https://cezionlyone.github.io/grist-widgets/gristcity/index.html`
3. Dans le panneau de droite, rubrique **Accès**, choisissez **Accès complet**.
4. Suivez l'assistant : choisissez un univers, puis partez d'un modèle prêt à l'emploi ou branchez le widget sur une de vos tables.

## Ce que fait le widget

- **Assistant de création** en 8 étapes, avec un aperçu qui se construit au fil des réponses.
- **Modèles prêts à l'emploi** : portefeuille de projets, plan de charge, suivi des demandes, parc applicatif, organigramme, parc de véhicules... Le widget crée les tables, avec des lignes d'exemple si vous le souhaitez.
- **Plusieurs villes par document**, en onglets.
- **Fiche modifiable** pour chaque immeuble, pièces jointes comprises.
- **Mode Déménager** : glisser un immeuble vers un autre quartier modifie la colonne correspondante.
- **Filtres, recherche et vue en liste**, alternative accessible à la carte.

## Ce que le widget écrit dans votre document

- Une table technique `BIBLIOTHEQUE_VILLE`, créée avec la première ville : une ligne de réglages par ville.
- Dans la table dessinée : uniquement les valeurs modifiées dans une fiche, les immeubles ajoutés et les déménagements. Sa structure n'est jamais modifiée.
- Les tables d'un modèle, seulement si vous en choisissez un.

## Droits

Le widget respecte les droits de chacun dans le document :

- **Lecteurs** : consultation, recherche, filtres, fiche en lecture.
- **Éditeurs** : en plus, modification des fiches, ajouts et déménagements.
- **Paramétrage** : réservable aux propriétaires par une règle d'accès. La marche à suivre est affichée dans le widget.

## Dépendances

- [DSFR](https://www.systeme-de-design.gouv.fr) v1.13.1 (Système de design de l'État)
- API des widgets Grist (`grist-plugin-api.js`)
- [pdf.js](https://mozilla.github.io/pdf.js/) v6.2.108, chargé seulement pour afficher les PDF joints, avec vérification de son empreinte

> **À savoir :** les modalités d'utilisation du DSFR le réservent aux sites de l'État. Vérifiez qu'elles s'appliquent à votre usage avant de déployer ce widget.

## Licence

[MIT](../LICENSE) : vous pouvez utiliser, modifier et redistribuer ce widget librement, en conservant la mention de l'auteur.

---

made **X** Cé
