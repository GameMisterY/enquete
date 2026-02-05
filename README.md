# Game MisterY Site d'Enquêtes

### Créer une nouvelle enquête `MonEnquete`

1. Créez un nouveau fichier `content/MonEnquete/_index.md` (`_index` avec un tiret du 8 !)
  a. Pour un enquête sans mot de passe: modifiez le contenu avec:
```md
---
layout: "lock"
---
```

  b. Pour un enquête avec mot de passe: modifier le contenu avec:
```md
---
password: "MonMotDePasse"
title: "MonTitreEnquete"
success_message: "MonMessageBravo"
error_message: "MonMessageMauvaisMotDePasse !"
placeholder: "1234"
layout: "lock"
---

MonMessage
  ```

2. Créez un nouveau fichier `content/MonEnquete/archives/index.md` avec le contenu suivant :
```md
---
title: "MonTitreEnqueteArchives"
layout: "archives"
---

MaDescriptionEnqueteArchives
```

3. Créez un nouveau fichier `content/MonEnquete/photos/index.md` avec le contenu suivant :
```md
---
title: "MonTitreEnquetePhotos"
layout: "photos"
---

MaDescriptionEnquetePhotos
```

4. Créez un nouveau fichier `content/MonEnquete/videos/index.md` avec le contenu suivant :
```md
---
title: "MonTitreEnqueteVideos"
layout: "videos"
---

MaDescriptionEnqueteVideos
```

5. (Optionel) Ajoutez des fichiers dans `content/NomEnquete/archives/` pour créer des nouveaux dossiers.

> NOTE: le nom du fichier sera le nom du dossier.

6. (Optionel) Ajoutez des photos dans `content/NomEnquete/photos/`

7. (Optionel) Ajoutez des vidéos dans `content/NomEnquete/videos/`

> NOTE: Format `.mp4`

L'enquête est maintenant créée avec le lien https://gamemistery.github.io/enquete/MonEnquete/

### TODO Développement
- [x] Mot de passe de protection
- [ ] Ouvertures des photos sur le site
- [ ] Mode téléphone


