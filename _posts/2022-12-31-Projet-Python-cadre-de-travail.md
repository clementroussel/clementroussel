---
layout: post
title: Projet Python, cadre de travail
---

Mémo sur la mise en place d'un cadre de travail pour le développement d'un projet de développement avec le langage de programmation *Python*.

<div id="header" align="center">
  <img src="{{site.baseurl}}/assets/icons/python.png" title="python" alt="python" width="40" height="40"/>&nbsp;
</div>

---

[1. Nouveau projet Python](#1-nouveau-projet-python)  
[2. GitHub](#2-github)  
[3. Conda](#3-conda)  
[4. Modules Python](#4-modules-python)  
[5. Documentation web](#5-documentation-web)  
[6. Documentation API](#6-documentation-api)  
[7. PyQt](#7-pyqt)  
[8. PyPI](#8-pypi)  
[9. Stack Overflow](#9-stack-overflow)  
[10. SourceForge](#10-sourceforge)

## 1. Nouveau projet Python

<div id="header" align="center">
  <img src="{{site.baseurl}}/assets/icons/idea.png" title="Idea" alt="Idea" width="40" height="40"/>&nbsp;
</div>

<br/><br/>

> Python est un langage de programmation interprété, multiparadigme et multiplateformes. Il favorise la programmation impérative structurée, fonctionnelle et orientée objet.
 
- attribution d'un nom au projet: **Cross Profile (cross-profile)**
- attribution d'un icone

**Liens:**  
- [Icon archives](https://iconarchive.com/)

## 2. GitHub

<div id="header" align="center">
  <img src="{{site.baseurl}}/assets/icons/github.png" title="GitHub" alt="GitHub" width="40" height="40"/>&nbsp;
</div>

<br/><br/>

> GitHub est un service web d'hébergement et de gestion de développement de logiciels, utilisant le logiciel de gestion de versions Git.

> Markdown est un langage de balisage léger dont le but est d'offrir une syntaxe facile à lire et à écrire.

- initialisation d'un nouveau dépôt *GitHub*
- création du fichier *README.md*
- création du fichier *LICENCE*
- création du fichier *.gitignore*

**Liens:**  
- [GitHub](https://github.com/)
- [GitHub Desktop](https://desktop.github.com/)
- [Choose a license](https://choosealicense.com/)
- [*Markdown*](https://www.markdownguide.org/)

## 3. Conda 

<div id="header" align="center">
  <img src="{{site.baseurl}}/assets/icons/conda.png" title="Conda" alt="Conda" width="40" height="40"/>&nbsp;
</div>

<br/><br/>

> Conda est un gestionnaire de packages et un système de gestion d'environnement open source, multiplateforme et indépendant du langage.

- création d'un environnement virtuel *cross-profile*

```bash
conda create --name cross-profile -y python=3.9
conda activate cross-profile
```

**Liens:**  
- [Conda](https://docs.conda.io/en/latest/)

## 4. Modules Python

<div id="header" align="center">
  <img src="{{site.baseurl}}/assets/icons/matplotlib.png" title="matplotlib" alt="matplotlib" width="40" height="40"/>&nbsp;
  <img src="{{site.baseurl}}/assets/icons/numpy.png" title="numpy" alt="numpy" width="40" height="40"/>&nbsp;
  <img src="{{site.baseurl}}/assets/icons/pandas.png" title="pandas" alt="pandas" width="40" height="40"/>&nbsp;
  <img src="{{site.baseurl}}/assets/icons/scipy.png" title="scipy" alt="scipy" width="40" height="40"/>&nbsp;
</div>

<br/><br/>

> Matplotlib est une bibliothèque du langage de programmation Python destinée à tracer et visualiser des données sous forme de graphiques.

> NumPy est une bibliothèque pour langage de programmation Python, destinée à manipuler des matrices ou tableaux multidimensionnels ainsi que des fonctions mathématiques opérant sur ces tableaux.

> Pandas est une bibliothèque écrite pour le langage de programmation Python permettant la manipulation et l'analyse des données.

> SciPy est un projet visant à unifier et fédérer un ensemble de bibliothèques Python à usage scientifique.

- ajout des modules scientifiques *matplotlib*, *numpy*, *pandas*, *scipy*
- création du fichier *requirements/base.txt*

```bash
pip install matplotlib numpy pandas scipy
pip freeze > requirements/base.txt
```

**Liens:**
- [matplotlib](https://matplotlib.org/)
- [numpy](https://numpy.org/)
- [pandas](https://pandas.pydata.org/)
- [scipy](https://scipy.org/)

## 5. Documentation web

<div id="header" align="center">
  <img src="{{site.baseurl}}/assets/icons/readthedocs.png" title="Readthedocs" alt="Readthedocs" width="40" height="40"/>&nbsp;
  <img src="{{site.baseurl}}/assets/icons/sphinx.png" title="sphinx" alt="sphinx" width="40" height="40"/>&nbsp;
</div>

<br/><br/>

> Sphinx est un générateur de documentation libre.

> Read the Docs est une plate-forme d'hébergement de documentation de logiciels gratuits open source. Il génère une documentation écrite avec le générateur de documentation Sphinx.

- création du répertoire *docs/*
- création du fichier *readthedocs.yaml*

**Liens:**  
- [Sphinx](https://www.sphinx-doc.org/en/master/)
- [Readthedocs](https://readthedocs.org/)

## 6. Documentation API

<div id="header" align="center">
  <img src="{{site.baseurl}}/assets/icons/jupyter.png" title="jupyter" alt="jupyter" width="40" height="40"/>&nbsp;
</div>

<br/><br/>

> Jupyter Notebook est un outil puissant qui permet aux utilisateurs du langage Python de créer et de partager des documents interactifs contenant du code dynamique et exécutable, des visualisations de contenus, des textes de documentation et des équations.

- création du répertoire *notebooks/*

```bash
pip install jupyterlab
```

**Liens:**  
- [Jupyter](https://jupyter.org/)
- [nbviewer](https://nbviewer.org/)


## 7. PyQt

<div id="header" align="center">
  <img src="{{site.baseurl}}/assets/icons/qt.png" title="qt" alt="qt" width="40" height="40"/>&nbsp;
</div>

<br/><br/>

> PyQt est un module libre qui permet de lier le langage Python avec la bibliothèque Qt. Il permet de créer des interfaces graphiques en Python.

- création du répertoire *src/*

```bash
pip install fbs PyQt5
fbs startproject
```

**Liens:**  
- [fbs](https://build-system.fman.io/)
- [Qt](https://www.qt.io/)

## 8. PyPI

<div id="header" align="center">
  <img src="{{site.baseurl}}/assets/icons/pypi.png" title="pypi" alt="pypi" width="40" height="40"/>&nbsp;
</div>

<br/><br/>

> PyPI est le dépôt tiers officiel du langage de programmation Python. Son objectif est de doter la communauté des développeurs Python d'un catalogue complet recensant tous les paquets Python libres.

> Poetry est un outil de gestion des dépendances et de packaging en Python.

- création du répertoire *dist/*
- création du fichier *pyproject.toml*

```bash
poetry build
poetry publish
```

**Liens:**  
- [PyPI](https://pypi.org/)
- [Poetry](https://python-poetry.org/)

## 9. Stack Overflow

<div id="header" align="center">
  <img src="{{site.baseurl}}/assets/icons/stackoverflow.png" title="stack-overflow" alt="stack-overflow" width="40" height="40"/>&nbsp;
</div>

<br/><br/>

> Stack Overflow est un site web proposant des questions et réponses sur un large choix de thèmes concernant la programmation informatique.

**Liens:**  
- [Stack Overflow](https://stackoverflow.com/)

## 10. SourceForge

<div id="header" align="center">
  <img src="{{site.baseurl}}/assets/icons/sourceforge.png" title="sourceforge" alt="sourceforge" width="40" height="40"/>&nbsp;
</div>

<br/><br/>

> SourceForge.net est une forge logicielle, c'est-à-dire un site web hébergeant la gestion du développement de logiciels majoritairement libres. 

**Liens:**
- [SourceForge](https://sourceforge.net/)