---
layout: post
title: Projet Python, cadre de travail
---

Mémo sur laa mise en place d'un cadre de travail pour le développement d'un projet de développement avec le langage de programmation *Python*.

---

## 1. Nouveau projet

<div id="header" align="center">
  <img src="{{site.baseurl}}/assets/icons/idea.png" title="Idea" alt="Idea" width="40" height="40"/>&nbsp;
</div>

---

- nom du projet: **pyCross**;  
- logo: [icon archives](https://iconarchive.com/).

## 2. GitHub

<div id="header" align="center">
  <img src="{{site.baseurl}}/assets/icons/github.png" title="GitHub" alt="GitHub" width="40" height="40"/>&nbsp;
</div>

---

- à l'aide de *GitHub Desktop*, initialisation d'un nouveau dépôt *pyCross*:
    - avec un fichier README;
    - avec une license GNU-GPLv3;
    - sans fichier .gitignore

**Liens:**  
- [GitHub](https://github.com/)
- [GitHub Desktop](https://desktop.github.com/)
- [Choose a license](https://choosealicense.com/)
- [*Markdown*](https://www.markdownguide.org/)

Le dépôt *GitHub* est accessible à l'url: https://github.com/clementroussel/pyCross.

### 3. Conda 

<div id="header" align="center">
  <img src="{{site.baseurl}}/assets/icons/conda.png" title="Conda" alt="Conda" width="40" height="40"/>&nbsp;
</div>

---

- à l'aide de *Conda*, création de plusieurs environnements virtuels:
    - *pyCross*

On utilise [*Conda*](https://docs.conda.io/en/latest/) pour créer nos environnements virtuels et gérer les dépendances de notre projet:  
- un premier environnement virtuel nommé *pyCross* dédié à la librairie *Python* et à l'interface graphique de notre projet;
- un second environnement virtuel nommé *pyCross-docs* dédié à la documentation (site internet) de notre projet.


## 4. Arborescence des dossiers

L'arborescence des dossiers nous est dictée par le module *Python* nommé [*fbs*](https://build-system.fman.io/) qui a la lourde charge de produire un exécutable permettant à tous de pouvoir travailler avec un logiciel interfacé sur son ordinateur.
