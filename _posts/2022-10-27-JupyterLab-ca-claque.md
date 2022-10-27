---
layout: post
title: JupyterLab, ça claque!
---

Cet article fait suite à celui intitulé [Python - installation & bonnes pratiques](https://clementroussel.github.io/clementroussel/2022/10/26/Python-installations-et-bonnes-pratiques.html), dans lequel, je n'en doute pas, l'usage de *l'Anaconda Powershell Prompt* vous avait probablement perturbé! Dans cet article, je vous propose une solution bien plus attrayante pour travailler efficacement avec *Python*, j'ai nommé: *JupyterLab*!

**Temps de lecture et de mise en œuvre estimé à 30 minutes**

---

## Prérequis

Il est nécessaire d'avoir lu et mis en œuvre l'article [Python - installation & bonnes pratiques](https://clementroussel.github.io/clementroussel/2022/10/26/Python-installations-et-bonnes-pratiques.html) avant de pouvoir suivre paisiblement cet article.

## Fini avec cet horrible *Anaconda Powershell Prompt* ?

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

Nous pourrions également y exécuter des scripts *Python* édités depuis le Bloc-notes de *Windows* par exemple:
```bash
python mon_script.py
```

<div align="center">
    <img src="{{site.baseurl}}/assets/images/bonjour_le_monde.png">
    <p><u>Le Bloc-notes <i>Windows</i> et <i>l'Anaconda Powershell Prompt</i> suffisent pour développer en <i>Python</i>.</u></p>
</div>

Les puristes s'arrêteront ici car finalement, le Bloc-notes *Windows* et *l'Anaconda Powershell Prompt* suffisent amplement pour travailler avec le langage de programmation *Python*.  
Pour les bobos geek, les hypsters du clavier ou les Beatniks adeptes de la trottinnette électrique, il existe une solution bien plus *sexy* pour **écrire**, **documenter**, **partager**, **présenter**..., son code *Python*.

## Installer *jupyter-lab*

    > JupyterLab is the latest web-based interactive development environment for notebooks, code, and data. Its flexible interface allows users to configure and arrange workflows in data science, scientific computing, computational journalism, and machine learning. A modular design invites extensions to expand and enrich functionality. (source: https://jupyter.org/)

<div align="center">
    <img src="{{site.baseurl}}/assets/images/bonjour_le_monde.png">
    <p><u>Le Bloc-notes <i>Windows</i> et <i>l'Anaconda Powershell Prompt</i> suffisent pour développer en <i>Python</i>.</u></p>
</div>

## Apprendre

## A retenir

## Liens et références