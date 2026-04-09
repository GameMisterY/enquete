# Game MisterY Site d'Enquêtes

### Liens

Les enqûetes disponibles sont listé ici:

https://gamemistery.github.io/enquete/liens


### Créer une nouvelle enquête `MonEnquete`

1. Créez un nouveau fichier `content/MonEnquete/_index.md` (`_index` avec un tiret du 8 !)

a. Pour une enquête sans mot de passe: modifiez le contenu avec:
```md
---
layout: "affichage-mot-de-passe"
---
```

b. Pour une enquête avec mot de passe: modifier le contenu avec:
```md
---
password: "MonMotDePasse"
title: "MonTitreEnquete"
success_message: "MonMessageBravo"
error_message: "MonMessageMauvaisMotDePasse !"
placeholder: "1234"
layout: "affichage-mot-de-passe"
---

MonMessage
  ```
### Ajouter un onglet `MonOnglet` à l'enquête 

1. Créez un nouveau fichier `content/MonEnquete/MonOnglet/index.md` avec le contenu suivant :
```md
---
title: "MonTitre"
layout: "affichage-en-dossiers"
---

MaDescription
```

`affichage-en-dossiers` peux être remplacé par :
* `affichage-en-photos`
* `affichage-en-videos`
* `affichage-en-genially`

Des paramètres optionnels peuvent être ajoutés:
* `order` permet de définir l'ordre des onglets
* `sidebar: false` permet de ne pas afficher la barre latérale (utile quand il n'y a qu'un onglet)
* `subtitle` permet de définir le sous-titre affiché dans la barre latérale pour cet onglet
* `icon` permet de définir l'icône affiché dans la barre latéral pour cet onglet (Les icônes sont placés dans le dossier `assets/icons`) Mettre uniquement le nom de l'icône. Pax example `icon: suspect.png` utilisera l'icône dans `assets/icons/suspect.png`.

Example:
```md
---
title: "MonTitre"
subtitle: "MonSousTitre"
layout: "affichage-en-dossiers"
order: 3
sidebar: false
icon: suspect.png
---
```

2. (Optionel) Ajoutez des fichiers dans `content/NomEnquete/MonOnglet/` pour créer des nouveaux dossiers.

> NOTE: en affichage-en-dossiers le nom du fichier sera le nom du dossier.

> NOTE: le affichage-en-videos acepte uniquement le format mp4.

> NOTE: le affichage-en-photos acepte uniquement les formats jpeg, jpg et png.

L'enquête est maintenant créée avec le lien https://gamemistery.github.io/enquete/MonEnquete/

### Affichage en genially

Pour créer un onglet avec un genially intégré:
1. Créez un nouveau fichier `content/MonEnquete/MonOngletGenially/index.md`
```md
---
title: "MonTitre"
layout: "affichage-en-genially"
link: "https://lien-du-genially"
---
```


### TODO Développement
- [x] Mot de passe de protection
- [x] Ouvertures des photos sur le site
- [x] Mode téléphone
- [x] Header sous forme de bar latéral
- [x] Autoriser le contenu full-page



memo code Analyse d'indices:

---
title: "Analyse d'indices"
layout: "affichage-en-photos"
icon: loupe.png
order: 6
---


Aucun indice...


---
title: "Suspects"
subtitle: "Fiche de la suspects"
layout: "affichage-en-dossiers"
icon: suspect.png
order: 2
---


Aucun document...
