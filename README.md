# GitHub à l'ETML.
><div align="justify">Voici le document crée à l'ETML. Ce document vous expliquera les thermes liés à Git et GitHub. <br> Il vous servira de tutoriel et de document théorique sur les différents thermes et commandes Git.</div>

# Pull Request | Fork

## 1. Pull Request
***<div align="justify">Les pull requests sont la façon dont on vérifie les modifications du code source dans une branche. Quand on ouvre une pull request, on peut visualiser et collaborer sur les modifications de code avant le merge.</div>***

### 1.1 Git bash
> Commande sur git bash :
```git
git request-pull [-p] <start> <url> [<end>]
```
### 1.2 GitKraken
![Capture3](https://user-images.githubusercontent.com/74264318/145035421-fa99b2f0-1825-466f-8dd2-52c98cb9aebd.PNG)

![Capture4](https://user-images.githubusercontent.com/74264318/145035557-dcdcf66a-e61c-4364-9cf3-a56ae9ea006d.PNG)

### 1.3 GitHub
- Aller dans la section "Pull requests" du dépôt.
- Appuyez sur "New pull request".
- Sélectionnez les branches à comparés

![Capture](https://user-images.githubusercontent.com/74264318/145034157-b0448636-7dcf-4445-b855-a5e4137d3545.PNG)

- Après cela, mettez votre commentaire et créer la pull request.

![Capture2](https://user-images.githubusercontent.com/74264318/145034626-e2b34065-0f47-4225-bdcd-0c586898e977.PNG)


## 2. Fork
***<div align="justify">Un fork est une copie d'un dépôt. Cela permet de faire des modifications sur un dépôt sans que le dépôt principal soit affecté.</div***

### 2.1 GitKraken
- Cloner le dépôt initial.
- Ajouter un remote.
- Forkez le dépôt.
- Le lien de référence avec la marche à suivre complète :  
https://support.gitkraken.com/working-with-repositories/fork/

### 2.2 GitHub
- Aller sur dépôt initial.
- En haut à droite un bouton "Fork" est présent.
- Vous appuyez dessus.

# Therme Git

## 1. Branch
***<div align="justify">Une branch est essentiellement un ensemble unique de modification de code avec un nom unique. Chaque repo peut avoir une ou plusieurs branch. La branch principale qui s’appelle master, dans laquelle toutes les modifications sont finalement fusionnées. Il s’agit de la version officielle du projet et celle qu’on voit quand on visite le repo du projet.</div>***
> Lien de référence :  
https://www.atlassian.com/fr/git/tutorials/using-branches

### 1.1 Git bash
> Créer la branch et switch immédiatement dedans :
```git
git checkout -b <branch-name>
```
> Push la branch local sur le dépôt distant :
```git
git push -u <remote> <branch-name>
```

## 2. Commit 
***<div align="justify">À un niveau général, Git peut être considéré comme un utilitaire de gestion de la chronologie. Les commits constituent les piliers d'une chronologie de projet Git. Cela interagit dans le dépôt local, ce qui ne nécessite aucune interaction avec d'autres dépôts Git. On peut y ajouter une description de l'ajout effectué en local, afin de l'envoyer dans le dépôt distant.<div>***
> Lien de référence :  
https://www.atlassian.com/fr/git/tutorials/saving-changes/git-commit

### 2.1 Git bash
> Faire un commit avec git bash :
```git
git commit -m "commit message"
```

## 3. Pull
***<div align="justify">Les pull requests sont une fonctionnalité facilitant la collaboration des développeurs avec Git Kraken. Elles fournissent une interface conviviale pour discuter des changements proposés avant de l’intégrer au projet officiel.</div>***
> Lien de référence :  
https://www.atlassian.com/fr/git/tutorials/syncing/git-pull

### 3.1 Git bash
> Faire un pull avec git bash :
```git
git pull
```

## 4. Push
***<div align="justify">Le push est la commande la plus couramment utilisée pour publier des changements locaux et les charger vers un dépôt centralisé. Après qu’un dépôt local a été modifié, un push est exécuté pour partager les changements avec les membres de l’équipe distants.</div>***
> Lien de référence :  
https://www.atlassian.com/fr/git/tutorials/syncing/git-push

### 4.1 Git bash
> Faire un push avec git bash :
```git
- git push
- git push <remote> <branch>
```

## 5. Fetch
***<div align="justify">Le fetch permet, tout comme le pull, de télécharger le dépôt distant dans une copie locale. La seule difference est que fetch ne télécharge pas les métadonnées associées à un projet. C'est à dire qu'il ne met pas à jour les fichiers déjà présents dans le dépôt local.</div>***
> Lien de référence :  
https://www.atlassian.com/fr/git/tutorials/syncing/git-fetch

### 5.1 Git bash
> Faire un fetch avec git bash :
```git
- git fetch <remote>
- git fetch <remote> <branch>
```

## 6. Origin
***<div align="justify">C'est l'origine du dépôt et non pas le nom d'une branche. Comme dans une arborescence de fichier : <br> - Origin/NomDeLaBranche</div>***

## 7. Upstream
***<div align="justify">Upstream définit l'emplacement que le dépôt local contient. Imaginons que j'ai un dépot avec 2 branches : <br> - Origin/master <br> - Origin/Dev <br> Depuis le dépôt local, si je clone le dépôt distant, le upstream, donc le "lien" du dépôt distant (Dépôt + branche) sera déjà défini.</div>***
> Lien de référence :  
https://www.atlassian.com/git/tutorials/git-forks-and-upstreams

### 7.1 Git bash
> Faire un upstream avec git bash :
```git
git push --set-upstream origin master 
```

## 8. Stage
***<div align="justify">Le stage est une zone tampon, autrement dit il stock temporerement les fichiers modifiés dans une liste d'attente afin d'être ajouté par le prochain commit.</div>***
> Lien de référence :  
https://www.atlassian.com/fr/git/tutorials/saving-changes

### 8.1 Git bash
> Faire un stage avec git bash :
```git
git add .
```

## 9. Tag
***<div align="justify">Le tag est un balisage pour marquer des points soécifiques de l'historique Git.Les tags sont généralement utilisés pour capturer un point de l'historique .utilisé pour une version marquée (c.-à-d., v1.0.1).</div>***
> Lien de référence :  
https://www.atlassian.com/fr/git/tutorials/inspecting-a-repository/git-tag

### 9.1 Git bash
> Faire un tag avec git bash :
```git
git tag <tagname>
```

# Créateurs
- [David Dieperink](https://github.com/dieperid)  
- [Alexis Rojas](https://github.com/Alexis1476)
- [Stefan Petrovic](https://github.com/XiJune)
- [Thomas Rey](https://github.com/ThomasRey1)
- [Damien Loup](https://github.com/dam277)