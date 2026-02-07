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


2. (Optionel) Ajoutez des fichiers dans `content/NomEnquete/MonOnglet/` pour créer des nouveaux dossiers.

> NOTE: en affichage-en-dossiers le nom du fichier sera le nom du dossier.
> NOTE: le affichage-en-videos acepte uniquement le format mp4.
> NOTE: le affichage-en-photos acepte uniquement les formats jpeg, jpg et png.

L'enquête est maintenant créée avec le lien https://gamemistery.github.io/enquete/MonEnquete/

### TODO Développement
- [x] Mot de passe de protection
- [x] Ouvertures des photos sur le site
- [ ] Mode téléphone


