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
[2. Utiliser *Anaconda Powershell Prompt*](#utiliser-anaconda-powershell-prompt)  
[3. Travailler avec les environnements virtuels](#travailler-avec-les-environnements-virtuels)  

## Installer *Conda*

[*Conda*](https://docs.conda.io/en/latest/) est un gestionnaire de packages et un système de gestion d'environnement open source. Il va nous permettre de gérer facilement *Python* et ses modules tierces grâce aux *environnements virtuels*. Pour l'instant, commençons par [télécharger l'installateur de *Conda* pour *Windows*](https://repo.anaconda.com/miniconda/Miniconda3-latest-Windows-x86_64.exe).  

Vous devriez trouver dans votre dossier *Téléchargements* un fichier nommé *Miniconda3-latest-Windows-x86_64.exe*. Aucune élévation administrateur ne vous sera demandée pour exécuter ce fichier (hallelujah!).  

Laissez les paramètres d'installation par défaut, patientez durant l'installation de *Conda* puis décochez les cases *Anaconda Distribution Tutorial* et *Getting Started with Anaconda* avant de quitter l'installateur.

<div align="center">
    <img src="{{site.baseurl}}/assets/images/conda_installer.png">
    <p><u>Décochez les deux cases avant de quitter l'installateur.</u></p>
</div>

Pour information, un dossier *Miniconda3* a été créé dans votre répertoire utilisateur. Sachez que dans ce dossier se trouve notamment le programme *Uninstall-Miniconda3.exe* permettant de supprimer *Conda* de votre ordinateur.

## Utiliser *Anaconda Powershell Prompt*

Cherchons maintenant à ouvrir un des programmes apparu avec l'installation de *Conda*. Il s'agit du programme *Anaconda Powershell Prompt*. Vous le trouverez facilement dans le *menu Démarrer* de *Windows* en tapant au clavier ses premières lettres.

<div align="center">
    <img src="{{site.baseurl}}/assets/images/anaconda_powershell_prompt.png">
    <p><u>Recherchez le programme <i>Anaconda Powershell Prompt</i>.</u></p>
</div>

Je vous conseille d'épingler ce programme à votre *barre des tâches* pour y accéder rapidement par la suite.  

Lorsque vous exécuter *Anaconda Powershell Prompt*, une fenêtre rustique sur fond noir (appelée *invite de commande*) apparaît sous votre regard ~~ébahi~~ déconcerté, sidéré, embarrassé, médusé, estomaqué, pantois voire pétrifié. Pas de panique. Une grande inspiration...suivie d'une lente expiration. Tout va bien se passer.  

Vérifions dans un premier temps que *Conda* est bien installé en vérifiant sa version. Au clavier, entrez la commande suivante:

```bash
conda --version
```

puis tapez sur la touche *Entrée* de votre clavier. Si l'installation s'est bien déroulée, vous devriez voir apparaître en retour de votre commande le numéro de version de *Conda*.  

Entrez ensuite la commande suivante:

```bash
python --version
```

Puis tapez sur la touche *Entrée*. Cette fois-ci, vous devriez voir apparaître le numéro de version de *Python*, signifiant également que *Python* est maintenant bien présent sur votre ordinateur (re-hallelujah!).

Pour finir cette section en beauté, entrez finalement la commande:

```bash
python
```

Cette dernière commande lance le programme *Python*. Vous devriez remarquer les trois chevrons ```>>>``` vous invitant à, littéralement parlant, *discuter* en *Python* avec votre ordinateur. Demandez lui, par exemple, de vous afficher le message *Hello World !* grâce à *l'instruction* suivante:

```python
print("Hello World !")
```

Sans surprise, *Python* vous répond en affichant le texte passé en paramètre de la fonction ```print```.  

<div align="center">
    <img src="{{site.baseurl}}/assets/images/hello_world.png">
    <p><u>Invite de commande et interpréteur <i>Python</i>.</u></p>
</div>

La dernière *instruction* passée à *l'interpréteur Python* ```exit()``` ferme *l'interpréteur Python* et redonne la main sur *l'invite de commande*.  

Félicitations! *Python* est maintenant installé sur votre ordinateur et vous pouvez y accéder en utilisant l'invite de commande *Anaconda Powershell Prompt* maintenant épinglée à votre *barre des tâches*. Cependant, je vous ~~oblige~~ invite très fortement à suivre la section suivante pour adopter de bonnes pratiques et être en droit de porter fièrement le T-shirt officiel *Python*.

<div align="center">
    <img src="{{site.baseurl}}/assets/images/t-shirt.png" height="512">
    <p><u><i>Proud to be a <i>Python</i> Geek</i>.</u></p>
</div>

## Travailler avec les environnements virtuels

De nouveau, pas de panique. La notion, pour l'instant abstraite *d'environnement virtuel*, n'aura bientôt plus de secret pour vous. Commençons par une tentative de définition.  

Un *environnement virtuel* est un espace contenant une installation de *Python* autonome, c'est-à-dire indépendante de celle du système d'exploitation. Un *environnement virtuel* permet notamment:
- d'avoir une version par défaut de *Python* différente de celle du système;
- d'installer des *librairies* dans des versions spécifiques;
- d'installer des *libriaires* sans les installer globalement sur le système d'exploitation.

Passons à la pratique pour assimiler plus facilement ces notions.  

Dans *l'Anaconda Powershell Prompt*, vous avez peut-être remarqué l'indication ```(base)``` qui débute chaque nouvelle ligne de *l'invite de commande*. Elle signifie que vous êtes actuellement dans *l'environnement virtuel* nommé *base*. C'est *l'environnement virtuel* de *Conda* par défaut. Dans la section précédente, nous avons constaté que *Python* y était présent en vérifiant notammenet sa version. **Par convention, on ne travaille jamais dans *l'environnement virtuel* par défaut.**  

Respectons cette convention et créons notre propre *environnement virtuel*. Dans *l'Anaconda Powershell Prompt*, entrez la commande suivante:

```bash
conda create --name python38 --yes python=3.8
```

Cette commande demande à *Conda* de créer un *environnement virtuel* nommé *python38* avec une version spécifique de *Python*, ici la version 3.8. *Conda* se débrouille alors pour télécharger et générer les fichiers nécessaires à la création de ce nouvel environnement. A la fin du processus de création de notre environnement, il vous indique même le message suivant:

```bash
# To activate this environment, use
#
#     $ conda activate python38
#
# To deactivate an active environment, use
#
#     $ conda deactivate
```

