---
layout: post
title: Python, installation et bonnes pratiques
---

Il existe différents moyens d'installer et de mettre en œuvre le langage de programmation *Python* sur votre ordinateur. Entre droits administrateur, versions de *Python* et installation de modules tierces, vous pourriez rapidement vous décourager dans l'utilisation de *Python*. Suivez les conseils de *Mr Propre* pour une installation et une utilisation optimale de votre nouvel meilleur ami, *Python* !

<div align="center">
    <img src="{{site.baseurl}}/assets/images/mr_propre.png" width="64">
</div>

**Temps de lecture et de mise en œuvre estimé à 30 minutes**

---

[1. Installer *Conda*](#installer-conda)  
[2. Utiliser *Anaconda Powershell Prompt*](##utiliser-anaconda-powershell-prompt)  
[3. Environnement virtuel](##environnement-virtuel)  

## Installer *Conda*

[*Conda*](https://docs.conda.io/en/latest/) est un gestionnaire de packages et un système de gestion d'environnement open source. Il va nous permettre de gérer facilement *Python* et ses modules tierces grâce aux *environnements virtuels*. Pour l'instant, commençons par [télécharger l'installateur de *Conda* pour *Windows*](https://repo.anaconda.com/miniconda/Miniconda3-latest-Windows-x86_64.exe).  

Vous devriez trouver dans votre dossier *Téléchargements* un fichier nommé *Miniconda3-latest-Windows-x86_64.exe*. Aucune élévation administrateur ne vous sera demandée pour exécuter ce fichier (hallelujah!).  

Laissez les paramètres d'installation par défaut, patientez durant l'installation de *Conda* puis décochez les cases *Anaconda Distribution Tutorial* et *Getting Started with Anaconda* avant de quitter l'installateur.

<div align="center">
    <img src="{{site.baseurl}}/assets/images/conda_installer.png">
    <p>Décochez les deux cases avant de quitter l'installateur.</p>
</div>

Pour information, un dossier *Miniconda3* a été créé dans votre répertoire utilisateur. Sachez que dans ce dossier se trouve notamment le programme *Uninstall-Miniconda3.exe* permettant de supprimer *Conda* de votre ordinateur.

## Utiliser *Anaconda Powershell Prompt*

Cherchons maintenant à ouvrir un des programmes apparu avec l'installation de *Conda*. Il s'agit du programme *Anaconda Powershell Prompt*. Vous le trouverez facilement dans le *menu Démarrer* de *Windows* en tapant au clavier ses premières lettres.

<div align="center">
    <img src="{{site.baseurl}}/assets/images/anaconda_powershell_prompt.png">
</div>

Je vous conseille d'épingler ce programme à votre *barre des tâches* pour y accéder rapidement par la suite.  

Lorsque vous exécuter *Anaconda Powershell Prompt*, une fenêtre rustique sur fond noir (appelée *invite de commande*) apparaît sous votre regard ~~ébahi~~ déconcerté, sidéré, embarrassé, médusé, estomaqué, pantois voire pétrifié. Pas de panique. Une grande inspiration...suivie d'une lente expiration. Tout va bien se passer.  

Vérifions dans un premier temps que *Conda* est bien installé en vérifiant sa version. Au clavier, entrez la commande suivante:

```bash
conda --version
```

puis tapez sur la touche *Entrée* de votre clavier. Si l'installation s'est bien déroulée, vous devriez voir apparaître en retour de votre commande le numéro de version de *Conda*.



<div align="center">
    <img src="{{site.baseurl}}/assets/images/hello_world.png">
</div>

## Environnement virtuel

toto

 *Conda* est un gestionnaire de packages et un système de gestion d'environnement open source. Il permet notamment de créer facilement des **environnements virtuels** associés à différentes versions de *Python*.  

Un **environnement virtuel** est un répertoire contenant une installation de *Python* autonome (indépendante de celle du système d'exploitation). Les **environnements virtuels** sont intéressants lorsqu'on souhite:

- avoir une version par défaut de *Python* différente de celle du système;
- installer des librairies dans une version différente de celle du système;
- installer des librairies sans les installer globalement sur le système.

## Télécharger et installer *Conda*

- Télécharger l'installateur de *Miniconda* pour votre système d'exploitation sur [https://docs.conda.io/en/latest/miniconda.html](https://docs.conda.io/en/latest/miniconda.html).
- Exécuter l'installateur en laissant les paramètres d'installation par défaut. Il n'est pas nécessaire d'être administrateur pour installer *Conda*.


