---
layout: home
layout: post
title:  Les 6 trucs que j'aurais aimé qu'on me dise sur GIT quand j'ai commencé à lutiliser...
date:   2017-05-23
categories: git
---

Git est un logiciel puissant qu'on a un peu de mal à aborder. Souvent les débutants ont du mal à percevoir quelques subtilités qui fait tout le sel de git. Pire, une mauvaise utilisation peut conduire à quelques erreurs ou incompréhension de certains concepts. Voilà donc quelques éléments important à connaître quand on démarre Git.

### 1 - On est pas obligé de tout commiter

Contrairement à des logiciels comme CVS ou SVN, sur Git on doit indiquer ce que l'on commit. L'utilisateur doit spécifier, à l'aide de `git add`, ce qu'il veut mettre dans son commit. 

Il est donc tout à fait possible d'envoyer, pour un même fichier, d'ajouter des modifications dans un commit et d'autres dans un autre. On a aussi la possibilité de mettre de coté des modifications dans une planque (stash) locale.

### 2 - Git est un système décentralisé

C'est l'une des forces de git, chaque clone du dépôt contient un historique complet du projet et est complètement autonome. Le dépôt cloné va toutefois conserver une référence au dépôt distant (visible en faisant un `git remote -v`). 

On peut ainsi conserver nombres de modifications en local avant de les partager sur un dépôt distant. Il est tout à fait possible d'avoir plusieurs dépôts distants et pouvoir poussé des modifications sur l'un ou l'autre.

### 3 - L'historique n'est jamais définitif, ni chronologique

C'est une chose à savoir, il est tout à fait possible de reconstruire un historique avec Git. Pourquoi donc? En tant que codeur (ou musicien) vous pouvez être amener a tenter des choses, revenir en arrière, faire plusieurs petits commits et puis, au moment de partager vous modifications, pouvoir nettoyer tout ça pour ne présenter que l'aspect fini de votre travail. 

Avec Git c'est tout à fait possible de faire ceci. Certains flux de travaux utilisent la notion de rebase qui modifie l'historique afin de placer les modifications d'une branche après ceux de la branche de base, sans se soucier de l'ordre chronologique. Ce peut être une très bonne pratique, juste une chose : méfiez vous du `git push -f`

### 4 - Git n'est pas github

C'est une confusion assez classique. Github est un service d'hébergement qui se base sur le logiciel de gestion de versions. 

Github s'est servi de la souplesse de git pour créer un service qui, en quelque sorte, a participer à la popularisation de Git. Un service comme Bitbucket utilise également Git.

Si vous ne voulez pas utiliser des services dans le cloud, vous pouvez vous servir de Gitlab.

### 5 - Les raccourcis c'est la vie

`git status`, `git checkout`, `git commit`, voici des commandes que vous allez taper très souvent. Alors pourquoi ne pas gagner du temps de manière efficace en utilisant les raccourcis. Ils se configurent de la manière suivante : `git config --global alias.co checkout`.

Il suffit de remplacer co par votre alias favori et checkout par la commande que vous voulez appeler. Si, comme moi, vous êtes un peu dyslexique, vous pouvez mettre en alias vos égarements : `git config --global alias commt commit`.

### 6 - L'aide est là pour être lue

Si vous avez un doute sur une fonction, n'hésitez pas à demander de l'aide à Git. Il suffit de faire pour ça un git help suivi du nom de la commande et, ainsi, d'avoir accès au manuel de la fonction. C'est ainsi qu'on peut découvrir de manière de faire, donc je recommande de lire régulièrement quelques pages de fonctions de temps à autre, pour l'hygiène. A noter également que si vous tapez git sans préciser de commandes, une liste des commandes Git habituelles vous sera présenté, avec les situations dans lesquelles les utiliser.

Et pour en découvrir plus, nous vous invitons à [notre prochain Rendez-Vous][meetup] ou vous pourrez découvrir et échanger sur ce puissant logiciel qu'est git.

#### Pour aller plus loin

L'antenne de l'AFUP à Montpellier organise un rendez-vous sur Git le mardi 30 mai 2017 à Épitech. Une série de conférences gratuites sur le thème de Git vous permettra d'approfondir vos compétences.

[Renseignements et réservations sur Meetup.com][meetup].

[meetup]: https://www.meetup.com/fr-FR/Montpellier-PHP-Meetup/events/239299792/
