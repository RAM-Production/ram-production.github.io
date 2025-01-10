# Documentation
Cette documentation explique comment mettre à jour le site uniquement en utilisant l'interface Web de GitHub.

## Ajouter un projet

### Première étape: Ajout des images du projet

1. Sur votre ordinateur, créer un dossier nommer [nom-du-projet] contenant toutes les images dont une image "thumbnail.jpg" qui servira d'illustration sur la page d'accueil.
2. Sur l'interface GitHub, aller dans le dossier `assets/img/projects`.
3. Sur l'interface GitHub, cliquer sur le menu "Add file" en haut à droite. Dans le menu déroulant, cliquer sur `Upload files`.
4. Sur la page d'ajout de fichiers, faites glisser votre dossier [nom-du-projet] de votre explorateur de fichiers vers la page Web. Normalement, les fichiers vont s'uploader.
5. En bas de la page, vous pouvez ajouter un titre à la modification; p.ex., "Ajout d'images pour [nom-du-projet]"
6. Enfin cliquer sur le bouton vert "Commit changes"

NB: Essayer de compresser les images avant upload sinon le site sera lent à charger.

### Deuxième étape: Ajout du texte du projet

1. Sur l'interface GitHub, aller dans le dossier `projects`.
2. Sur l'interface GitHub, cliquer sur le menu "Add file" en haut à droite. Dans le menu déroulant, cliquer sur `Create new file`.
3. En haut de la page, nommer le fichier `[nom-du-projet].md`.
4. Remplir le fichier en suivant le modèle ci-dessous
5. Une fois le fichier complété, cliquer sur le bouton vert `Commit changes...`.
6. Vous pouvez cliquer directement sur `Commit changes` sur le pop-up qui s'ouvre pour valider le commit. 


### Modèle de texte

```
---
layout: post
title: 'Nouveau projet super méga cool'
---
Voici la présentation de notre nouveau projet 

{% include image.html url="https://www.youtube.com/watch?v=[id]" image="projects/[nom-du-projet]/thumbnail.jpg" text="Voir vidéo" %}

#### Photos du tournage

{% include image.html image="projects/[nom-du-projet]/1.jpg"%}

{% include image.html image="projects/[nom-du-projet]/2.jpg"%}

```


### Troisième étape: Ajout à la page d'accueil

1. Aller dans le dossier `_data` et ouvrez le fichier `settings.yml`
2. Cliquer sur le bouton crayon en haut à droite.
3. Dans la section projects du fichier, ajouter la ligne suivante: `- {name: 'Titre du projet super cool',   url: '[nom-du-projet]'}`
4. Cliquer sur le bouton vert `Commit changes...`.
5. Vous pouvez cliquer directement sur `Commit changes` sur le pop-up qui s'ouvre pour valider le commit.

Le site sera automatiquement mis à jour! En cas de catastrophe, contacter Marc et il règlera le problème 😉

## Modification des pages existantes

### Modification d'un projet

Pour modifier le texte d'un projet, aller dans `projects` et d'ouvrir le fichier `[nom-du-projet].md`.
Ensuite, cliquer sur le bouton crayon en haut à droite. Vous pouvez désormais modifier le texte.
Une fois terminé, cliquer sur `Commit changes`.

Pour supprimer une image, il faut aller dans `assets/img/projects/[nom-du-projet]`.
Ouvrir l'image. En haut à droite de l'interface, cliquer sur les trois petits points `...`. Dans le menu déroulant, cliquer sur `Delete this file` puis cliquer sur `Commit changes`.
Pour ajouter une image, il faut aller dans `assets/img/projects/[nom-du-projet]`. Cliquer sur le menu "Add file" en haut à droite. Dans le menu déroulant, cliquer sur `Upload files`.
Une fois une image ajoutée ou supprimée, **n'oublier pas de modifier le fichier texte faisant référence à cette image**.

### Modification des pages "A propos" et "Contact".

Pour modifier les pages (autres que les projets), aller dans le dossier `pages` et ouvrez la page voulue.
Ensuite, cliquer sur le bouton crayon en haut à droite. Vous pouvez désormais modifier le texte.
Une fois terminé, cliquer sur `Commit changes`.
