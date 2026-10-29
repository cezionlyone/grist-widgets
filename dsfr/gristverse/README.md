# 🌐 Gristverse

Un widget personnalisé pour [Grist](https://www.getgrist.com) : le bureau virtuel de votre équipe, dessiné en pixel art.

Chaque personne a son emoji, son bureau, sa maison et son île. On voit d'un coup d'œil qui est au bureau, qui télétravaille et qui est absent, et on se déclare d'un clic : le personnage s'y rend, à pied, à vélo ou en trottinette.

Tout se paramètre dans le widget, sans toucher au code.

## Le plan

- **Un bâtiment par site**, avec un bureau par personne. L'aménagement se fait automatiquement, ou case par case.
- **L'espace commun** : l'accueil, la salle de réunion et la bibliothèque des projets.
- **Dehors** : une maison par personne pour le télétravail, et une île pour les absences. Le motif d'une absence n'est jamais demandé.

## Les pièces

Chaque pièce est facultative. Gristverse crée sa table, ou vous la branchez sur une table qui existe déjà dans votre document.

| Pièce | Ce qu'on y trouve |
|---|---|
| 🪑 Bureau de chacun | Où il travaille, jour par jour ou par période ; ses tâches sur le paperboard ; ses activités (heures par projet) et son relevé mensuel ; ses réunions |
| 📺 Salle de réunion | Les réunions du jour, un rappel 15 minutes avant, le bouton de la visio, la télé qui ouvre le canal de discussion |
| 📚 Ressources | Les liens et documents utiles rangés sur les étagères de l'accueil, avec une recherche ; les fichiers joints se consultent dans le widget |
| 🗄️ Bibliothèque des projets | Une étagère par statut, un classeur par projet avec sa fiche et ses documents, et le planning des projets |
| 👋 Accueil | Le planning « qui est où », avec le total par site et par jour |

## Installation

1. Dans votre document Grist, ajoutez une vue de type **Personnalisée**.
2. Choisissez l'**URL personnalisée** et collez :
   `https://cezionlyone.github.io/grist-widgets/dsfr/gristverse/`
3. Dans le panneau de droite, rubrique **Accès**, choisissez **Accès complet**.
4. Suivez l'assistant en 5 étapes : le modèle (deux sites, un site ou sur mesure), l'équipe, les pièces, l'aménagement des bureaux, puis « Ouvrir Gristverse ». Des données d'exemple sont proposées pour découvrir le widget.

## Pièces jointes

Les colonnes de type « Pièces jointes » de la table des projets et de celle des ressources s'affichent avec leurs fichiers. Les images et les PDF s'ouvrent dans une visionneuse, y compris sous Firefox, en plein écran si besoin. Les autres fichiers se téléchargent. Gristverse consulte les fichiers, il n'en envoie ni n'en retire aucun.

## Ce que le widget écrit dans votre document

- Les tables des pièces choisies, seulement si vous ne les branchez pas sur des tables existantes : Équipe, Présences, Réunions, Tâches, Ressources, Projets, Activités.
- Une table technique `BIBLIOTHEQUE_GRISTVERSE_`, qui garde les réglages.
- Dans les tables existantes : uniquement les déclarations de présence, les tâches, les activités et les valeurs modifiées. Leur structure n'est jamais modifiée.

## Accessibilité

- Chaque bureau et chaque salle est un bouton accessible au clavier, avec un nom complet.
- Une vue en liste remplace le plan pour les lecteurs d'écran.
- L'aménagement des bureaux a un tableau équivalent à la grille cliquable.
- Les animations s'arrêtent quand le système demande de les limiter.

## Dépendances

- [DSFR](https://www.systeme-de-design.gouv.fr) v1.13.1 (Système de design de l'État)
- API des widgets Grist (`grist-plugin-api.js`)
- [pdf.js](https://mozilla.github.io/pdf.js/) v6.2.108, chargé seulement pour afficher les PDF joints, avec vérification de son empreinte

> **À savoir :** les modalités d'utilisation du DSFR le réservent aux sites de l'État. Vérifiez qu'elles s'appliquent à votre usage avant de déployer ce widget.

## Licence

[MIT](../../LICENSE) : vous pouvez utiliser, modifier et redistribuer ce widget librement, en conservant la mention de l'auteur.

🇬🇧 English edition, without the DSFR: [en/gristverse](../../en/gristverse/)

---

made **X** Cé
