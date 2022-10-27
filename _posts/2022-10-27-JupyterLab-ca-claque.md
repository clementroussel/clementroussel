---
layout: post
title: JupyterLab, ça claque!
---

Cet article fait suite à celui intitulé [Python - installation & bonnes pratiques](https://clementroussel.github.io/clementroussel/2022/10/26/Python-installations-et-bonnes-pratiques.html), dans lequel, je n'en doute pas, l'usage de *l'Anaconda Powershell Prompt* vous avait probablement perturbé! Dans cet article, je vous propose une solution bien plus attrayante pour travailler efficacement avec *Python*, j'ai nommé: *JupyterLab*!

**Temps de lecture et de mise en œuvre estimé à 30 minutes**

---

[1. Prérequis](#1-prerequis)  
[2. Fini avec cet horrible *Anaconda Powershell Prompt* ?](#2-fini-avec-cet-horrible-anaconda-powershell-prompt-?)  
[3. Installer *JupyterLab*](#3-installer-jupyter-lab)  
[4. A retenir](#4-a-retenir)  
[5. Liens et références](#5-liens-et-references)  

## 1. Prérequis

Il est nécessaire d'avoir lu et mis en œuvre l'article [Python - installation & bonnes pratiques](https://clementroussel.github.io/clementroussel/2022/10/26/Python-installations-et-bonnes-pratiques.html) avant de pouvoir suivre paisiblement cet article.

## 2. Fini avec cet horrible *Anaconda Powershell Prompt* ?

Et non. Désolé.  

*L'Anaconda Powershell Prompt* reste le point d'entrée inévitable pour travailler avec *Conda* et *Python*. Pour rappel, cet outil nous avait permis de:

- créer un environnement virtuel, nommé *python38*
```bash
conda create --name python38 --yes python=3.8
```

- activer ce nouvel environnement:
```bash
conda activate python38
```

- installer quelques librairies scientifiques:
```bash
pip install numpy scipy pandas matplotlib
```

- lancer l'interpréteur de commande *Python*:
```bash
python
```

Nous pourrions également y exécuter des scripts *Python* édités depuis le Bloc-notes de *Windows*:
```bash
python mon_script.py
```

<div align="center">
    <img src="{{site.baseurl}}/assets/images/bonjour_le_monde.png">
    <p><u>Le Bloc-notes <i>Windows</i> et <i>l'Anaconda Powershell Prompt</i> suffisent pour développer en <i>Python</i>.</u></p>
</div>

Les puristes s'arrêteront ici car finalement, le Bloc-notes *Windows* et *l'Anaconda Powershell Prompt* suffisent amplement pour travailler avec le langage de programmation *Python*.  
Pour les bobos geek, les hypsters du clavier ou les Beatniks adeptes de la trottinnette électrique, il existe une solution bien plus *sexy* pour **écrire**, **documenter**, **partager**, **présenter**..., son code *Python*.

## 3. Installer *jupyter-lab*

**Une brève introduction à *JupyterLab*...**

> JupyterLab is the latest web-based interactive development environment for notebooks, code, and data. Its flexible interface allows users to configure and arrange workflows in data science, scientific computing, computational journalism, and machine learning. A modular design invites extensions to expand and enrich functionality. (source: https://jupyter.org/)

<div align="center">
    <img src="{{site.baseurl}}/assets/images/jupyterlab_screenshots.png">
    <p><u>Aperçus de l'environnement de développement interactif (IDE) <i>JupyterLab</i></u></p>
</div>

**..avant de procéder à son installation.**

Dans *l'Anaconda Powsershell Prompt*, activez l'environnement virtuel *python38*:

```bash
conda activate python38
```

Puis, installez *JupyterLab*:

```bash
pip install jupyterlab
```

Enfin, lancez *JupyterLab*:

```bash
jupyter-lab
```

La prise en main de *JupyterLab* mériterait un article à elle seule. Je vous oriente donc vers la section [Liens et références](#liens-et-références) pour vous former à la magie de *JupyterLab*.

## 4. A retenir

- *JupyterLab* est un environnement de développement interactif;
- On utilise *l'Anaconda Powershell Prompt* pour:
    - l'installer dans un environnement virtuel:
    ```bash
    pip install jupyterlab
    ```
    - le lancer:
    ```bash
    jupyter-lab
    ```
- Passer du statut de Moldus à celui de Maître Jedi en utilisant *JupyterLab*! 

## 5. Liens et références

- [JupyterLab : l'interface Web Jupyter de nouvelle génération](https://youtu.be/ctOM-Gza04Y)  
- [JupyterLab : L'évolution du bloc-notes Jupyter](https://youtu.be/NSiPeoDpwuI)  
- [Getting Started with JupyterLab - SciPy 2019 Tutorial](https://youtu.be/RFabWieskak)
- [Documentation officielle de *JupyterLab*](https://jupyterlab.readthedocs.io/en/stable/index.html)  
- [Guide Markown](https://www.markdownguide.org/)