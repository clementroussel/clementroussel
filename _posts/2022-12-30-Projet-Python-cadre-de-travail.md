---
layout: post
title: Projet Python, cadre de travail
---

Voici un article qui présente la mise en place d'un cadre de travail pour le développement d'un projet de développement avec le langage de programmation *Python*.

---

## 1. Nouveau projet

Afin de lier l'utilse à l'agréable, prenons comme exemple le développement d'un outil dédié aux profils en travers. Soyons originaux et nommons ce projet **pyCross**.  

Que pouvons-nous imaginer à l'intérieur de ce projet ?  
- une librairie *Python*: le cœur de l'outil;
    - versionnée et hébergée sur le dépôt officiel de *Python*.
    - documentée à l'aide de notebooks *Jupyter*.
- une interface graphique: l'habillage de l'outil;
    - versionnée et hébergée sur un site de téléchargement.
    - documentée sur un site internet.

## 2. GitHub

<div id="header" align="center">
  <img src="{{site.baseurl}}/assets/icons/github.png" title="GitHub" alt="GitHub" width="40" height="40"/>&nbsp;
</div>

---

La première étape consiste à créer un dépôt *GitHub* sur lequel sera hébergé l'intégralité du code ainsi que la documentation du projet.  

Le lien entre notre ordinateur local et ce dépôt distant hébergé sur la plateforme *GitHub*, peut se faire avec le logiciel [*GitHub Desktop*](https://desktop.github.com/).  

En ligne le projet est accessible à l'url: https://github.com/clementroussel/pyCross.

### 2.1. Licence

Le premier fichier présent dans le dépôt *GitHub* contient les termes de la license attachée à notre nouveau projet. Il est simplement nommé *LICENSE*.  

Choisir la licence adéquate: [Choose a license](https://choosealicense.com/).

Ici, nous choississons les termes de la [GNU GPLv3](https://choosealicense.com/licenses/gpl-3.0/).

### 2.2. Lisez-moi

Le deuxième fichier présent dans le dépôt *GitHub* est le fichier *README.md*. Son contenu est écrit en [*Markdown*](https://www.markdownguide.org/), un langage de balisage léger facile à appréhender. Il sera affiché lorsque l'on accède au dépôt du projet en ligne et joue donc le rôle de page d'accueil du projet.  

C'est l'emplacement idéal pour aider les développeurs et contributeurs du projet à reconstruire eux-mêmes les différentes couches du projet (code source, interface graphique et documentation).

