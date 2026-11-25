# 📚 WuitDocumentation

Un widget personnalisé pour [Grist](https://www.getgrist.com) : la documentation de votre document, tenue à jour à partir du document lui-même, et des pages d'accueil pour guider les utilisateurs.

## Ce qu'il fait

- **Fiche projet** : nom, finalité, équipe, intégrations, formulaires, règles métier.
- **Tables et colonnes** avec leurs descriptions, formules et relations, et un journal des modifications de structure.
- **Pages et vues** avec leurs descriptions et leurs adresses.
- **Règles d'accès** présentées en clair, **widgets personnalisés** analysés (sécurité, accessibilité, DSFR), **cellules en erreur** repérées.
- **Documentation imprimable**, ou enregistrée en PDF.
- **Visite guidée** du document.

## Une page d'accueil pour votre document

Dans l'onglet **Pages spéciales**, la page « 🏠 Accueil » se compose de blocs :

- **Cartes (pages)** : une carte par ligne, avec icône, titre, description et adresse. Avec une adresse, la carte devient cliquable : une page du document, un formulaire Grist, un site.
- **Liens (boutons)** : un bouton par ligne, libellé et adresse.
- **Sommaire des pages** : la liste des pages du document, composée toute seule, avec leurs descriptions.
- Titres, textes, bandeaux d'information et d'alerte, étapes, chiffres clés, contacts, tableaux.

L'accueil, ou toute autre page spéciale, se publie ensuite sur une page des utilisateurs, sans la documentation : les utilisateurs ne voient que la page d'accueil.

L'adresse d'une page se recopie depuis la barre du navigateur ; celle d'un formulaire, depuis son lien de partage dans Grist.

## Installation

1. Dans votre document Grist, ajoutez une vue de type **Personnalisée**.
2. Choisissez l'**URL personnalisée** et collez :
   `https://cezionlyone.github.io/grist-widgets/dsfr/wuitdocumentation/`
3. Dans le panneau de droite, rubrique **Accès**, choisissez **Accès complet**.

## Ce que le widget écrit dans votre document

- Une table technique `BIBLIOTHEQUE_CENTRALE`, créée si elle n'existe pas : fiche projet, descriptions, blocs des pages spéciales, réglages des pages des utilisateurs.
- Les descriptions des colonnes et des vues, dans les métadonnées du document : jamais la structure de vos données.
- La table `GristDocTour` si vous créez une visite guidée.
- Une table technique `ADMIN_ONLY` si vous cachez la page d'administration.

Les règles d'accès sont lues pour être expliquées, jamais écrites.

## Dépendances

- [DSFR](https://www.systeme-de-design.gouv.fr) v1.13.1 (Système de design de l'État)
- [DOMPurify](https://github.com/cure53/DOMPurify) v3.4.17
- API des widgets Grist (`grist-plugin-api.js`)

> **À savoir :** les modalités d'utilisation du DSFR le réservent aux sites de l'État. Vérifiez qu'elles s'appliquent à votre usage avant de déployer ce widget.

## Licence

[MIT](../../LICENSE) : vous pouvez utiliser, modifier et redistribuer ce widget librement, en conservant la mention de l'auteur.

---

made **X** Cé
