# 📨 WuitFusion

Un widget personnalisé pour [Grist](https://www.getgrist.com) : chaque ligne d'une table devient un document prêt à imprimer, comme un publipostage Word, sans quitter Grist.

## Ce qu'il fait

- **Un éditeur de texte façon traitement de texte**, avec une barre d'outils au-dessus du document : styles, polices, tableaux, images, encadrés, colonnes, sauts de page.
- **Des champs** tirés des colonnes de la table, insérés dans le texte, avec formats (montants et dates en toutes lettres...).
- **Des passages conditionnels** : un paragraphe qui ne s'affiche que si une colonne est remplie ou vaut une valeur.
- **Des filtres** pour ne produire qu'une partie des lignes.
- **Les sorties** : impression, PDF (joint à la ligne si vous le demandez), document Word rempli à partir d'un modèle .docx.
- **Une numérotation chronologique** facultative, au format de votre choix.
- **Des pages des utilisateurs** : les utilisateurs impriment leurs documents sans toucher au paramétrage, et peuvent les retoucher si vous le permettez.

## Dix modèles pour commencer

Courrier, convocation, programme ou déroulé, liste d'émargement, compte rendu, checklist, attestation, carton d'invitation, fiche interlocuteur, rapport de suivi. Un modèle crée ses tables s'il en a besoin, ou se branche sur les vôtres. Vous pouvez aussi partir d'un document vierge.

## Installation

1. Dans votre document Grist, ajoutez une vue de type **Personnalisée**.
2. Choisissez l'**URL personnalisée** et collez :
   `https://cezionlyone.github.io/grist-widgets/dsfr/wuitfusion/`
3. Dans le panneau de droite, rubrique **Accès**, choisissez **Accès complet**.

## Ce que le widget écrit dans votre document

- Une table technique `BIBLIOTHEQUE_CENTRALE`, créée si elle n'existe pas : une ligne de réglages par modèle de document.
- Dans votre table, seulement si vous le demandez : la marque « imprimé », le PDF joint, le numéro chronologique.
- Les tables d'un modèle, à la demande, et une table des retouches si vous autorisez les utilisateurs à retoucher leurs documents.
- Les pièces jointes du document : logos, modèles Word, PDF produits.

Les colonnes à formule ne sont jamais écrites.

## Dépendances

- [DSFR](https://www.systeme-de-design.gouv.fr) v1.13.1 (Système de design de l'État)
- [DOMPurify](https://github.com/cure53/DOMPurify) v3.4.17
- API des widgets Grist (`grist-plugin-api.js`)

Le PDF, le ZIP et le Word sont produits par le widget lui-même, sans autre bibliothèque ni service extérieur.

> **À savoir :** les modalités d'utilisation du DSFR le réservent aux sites de l'État. Vérifiez qu'elles s'appliquent à votre usage avant de déployer ce widget.

## Licence

[MIT](../../LICENSE) : vous pouvez utiliser, modifier et redistribuer ce widget librement, en conservant la mention de l'auteur.

---

made **X** Cé
