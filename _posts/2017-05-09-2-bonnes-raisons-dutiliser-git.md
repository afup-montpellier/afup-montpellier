---
layout: home
layout: post
title: 2 Bonnes raisons d'utiliser GIT
date:  2017-05-09
categories: git
---

Pour [notre prochain Meetup][meetup] nous allons parler de Git. Même si vous n'en avez jamais entendu parler jusqu'à présent, vous avez déjà du entendre le nom de son créateur, Linus Torvalds, le créateur du noyaux Linux. Git est son second projet et il répond à une problématique qui se pose à tous les développeurs du monde : la gestion de version des sources. 

Dans la suite de cet article nous allons tenter de vous expliquer ce que c'est exactement et pourquoi git constitue une avancée importante dans le domaine.

### La gestion des sources : qu'est ce que c'est?

Imaginez que un ou des musiciens-musiciennes cherche à travailler sur une composition. Leurs objectifs peuvent-être très différents, ils peuvent travailler sur un morceau de rock ou bien une symphonie (haha) mais il n'est reste pas moins que l'objectif est de mettre des notes ensemble sur une partition. 

### Un outil de travail collaboratif

Dans le groupe il peut y avoir différent profils (guitariste, chanteur) qui vont travailler sur des parties différentes de la partition et d'autres (bassiste, batteur) qui font avancer de concert sur la rythmique.

Le système de gestion de versions appliqué à la composition va fonctionner de la manière suivante : chaque musicien va travailler de son côté à partir d'une partition vierge ou préalablement composée. Ensuite, quand le musicien le décide, qu'il a composé une partition qui le satisfait, il va l'enregistrer et l'inscrire dans le temps. C'est ce qu'on appelle un commit.

Le système de gestion de versions garde une trace de ces commits, un historique, ce qui permet, à tout moment, de vérifier quels ont été les changements apportés par ce commit. 

Dans un système de gestion de versions, on conserve les différences entre deux versions. C'est à dire, dans le cas de notre partition, les notes ajoutées et supprimées par rapport à la précédente version.

### Gestion des versions d'un document

Viens le moment de fusionner les différentes pistes musicales. Il-y-a plusieurs manières de faire selon les œuvres. Parfois les musiciens décident d'eux même de reporter leurs modifications dans la partie principale, parfois c'est une décision d'équipe, parfois c'est un chef d'orchestre qui vérifiera si les modifications sont acceptables ou non.

Dans tous les cas une fusion est faite entre les modifications du compositeur et la partition principale. Il peut en résulter quelques couacs, par exemple quand deux musiciens ont travaillés sur les mêmes mesures de la partition. Il en génère un conflit qui doit être résolu avant de pouvoir continuer à fusionner les travaux. Ce conflit se résolu en prenant en compte l'évolution du morceau, un “si” pouvait être bienvenue à un moment mais par la suite c'est un “la” qui s'impose. Une fois fusionné, la partition devient la nouvelle partition de référence et sert de base à la suite du travail.

Voilà en quelques chapitres les grandes lignes d'un gestionnaire de versions tel que git. Ce système existe depuis très longtemps.

#### Pour aller plus loin

Le mardi 30 mai 2017, nous organiserons une série de conférences sur GIT. [Découvrez le programme et inscrivez-vous sur notre page Meetup][meetup].

[Renseignements et réservations sur Meetup.com][meetup].

[meetup]: https://www.meetup.com/fr-FR/Montpellier-PHP-Meetup/events/239299792/
