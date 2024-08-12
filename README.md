<p align="center">
    <a href="https://www.asc-csa.gc.ca/eng/satellites/planck/">
        <img alt="Planck Space Telescope with stylized Cosmic Microwave Background colours over a space backdrop" src="https://www.asc-csa.gc.ca/images/satellites/planck/planck-animation.jpg" height="200">
    </a>
</p>

<p align="center">
 <a href="#stars">
  <img alt="Étoiles sur GitHub | GitHub Repo stars" src="https://img.shields.io/github/stars/asc-csa/Planck-Telescope-Data-Tutorial">
 </a>
 <a href="#watchers">
  <img alt="Spectateurs sur Github | GitHub watchers" src="https://img.shields.io/github/watchers/asc-csa/Planck-Telescope-Data-Tutorial">
 </a>
 <a href="https://github.com/asc-csa/Planck-Telescope-Data-Tutorial/tree/main/commits/main">
  <img alt="Dernier commit sur GitHub | GitHub last commit" src="https://img.shields.io/github/last-commit/asc-csa/Planck-Telescope-Data-Tutorial">
 </a>
 <a href="https://github.com/asc-csa/Planck-Telescope-Data-Tutorial/tree/main/graphs/contributors">
  <img alt="Contributeurs sur GitHub | GitHub contributors" src="https://img.shields.io/github/contributors/asc-csa/Planck-Telescope-Data-Tutorial">
 </a>
 <a href="https://twitter.com/intent/follow?screen_name=csa_asc">
  <img alt="Suivre sur Twitter | Twitter Follow" src="https://img.shields.io/twitter/follow/csa_asc?style=social">
 </a>
</p>

# Extraction de données du télescope spatial Planck - Un tutoriel (English Follows)

## Contexte
La mission du satellite Planck est la première mission européenne vouée à l'étude de la naissance de l'Univers. Planck a été lancé conjointement avec l'Observatoire spatial Herschel à bord d'une fusée Ariane 5, le 14 mai 2009. Ce satellite est le télescope le plus sensible jamais conçu pour étudier le rayonnement cosmique de fond, c'est-à-dire les résidus du rayonnement issu du Big Bang qui s'est produit il y a 13,8 milliards d'années. Le télescope Planck mesure la température du rayonnement fossile cosmologique et cherche des régions légèrement plus chaudes ou plus froides que la moyenne. Ces faibles fluctuations de température, nommées anisotropies, seraient à l'origine des galaxies qui existent aujourd'hui.

Le télescope spatial Planck fournira aux astronomes un aperçu des conditions qui régnaient au tout début de l'Univers. L'objectif de la mission est d'aider à répondre à certaines des grandes questions de la science moderne : comment l'Univers s'est-il formé, comment a-t-il évolué jusqu'à sa forme actuelle et quelle forme prendra-t-il dans l'avenir? Les scientifiques espèrent ainsi établir quelle théorie explique le mieux l'origine de l'ensemble des structures cosmiques.

Le but de ce tutoriel est de faire connaître ces données et d’améliorer leur accessibilité. Dans ce tutoriel, vous êtes fourni des exemples de la façon d’importer des fichiers FITS, d’accéder aux informations d’en-tête, de manipuler les données HEALPix, de visualiser les skymaps et d’effectuer des analyses de base des données.

## Démarrage rapide

Veuillez noter que le code de ce didacticiel repose sur la bibliothèque Python [Healpy](https://healpy.readthedocs.io/en/latest/index.html), qui ne prend pas en charge Windows en mode natif. Si vous souhaitez exécuter le code sur Windows, veuillez utiliser le [Windows Subsystem for Linux](https://learn.microsoft.com/en-us/windows/wsl/install).

Si vous souhaitez interagir directement avec le notebook:

1. Télécharger [Planck_Telescope_Data_Tutorial.ipynb](https://github.com/asc-csa/Planck-Telescope-Data-Tutorial/blob/main/Planck_Telescope_Data_Tutorial.ipynb).
2. Ouvrez un terminal à l’emplacement du notebook et entrez la commande suivante pour installer les bibliothèques requises:
``` pip install -r requirements.txt ```
3. Si vous n’avez pas encore utilisé Jupyter Notebooks, installez-le avec:
``` pip install notebook ```
4. Entrez la commande suivante pour lancer un serveur Jupyter Notebook local:
``` jupyter notebook ```
5. Ouvrez l’URL qu’il fournit dans votre navigateur et expérimentez le didacticiel.

Sinon, vous pouvez simplement utiliser le code directement dans vos propres scripts Python.

# Extracting Planck Space Telescope data - A Tutorial  (Le français précède)

## About
Planck is Europe's first mission to study the birth of the Universe. Planck was launched jointly with the Herschel Space Observatory aboard an Ariane 5 rocket, on May 14, 2009. The satellite is the most sensitive telescope ever designed to study the cosmic microwave background--the remnants of radiation from the Big Bang 13.8 billion years ago. Planck's detectors measure the temperature of this light, searching for regions that are slightly warmer or colder than the average. These small fluctuations in temperature, called anisotropies, provided the seeds for the formation of galaxies that exist today.

The Planck satellite is giving astronomers a glimpse of conditions near the beginning of the Universe. The mission's objective is to help answer some fundamental questions of modern science: How was the Universe formed? How has it evolved to its present form? And what shape will it take in the future? Scientists thereby hope to establish which theory best explains the origin of all cosmic structures.

The purpose of this tutorial is to raise awareness of this data and enhance its accessibility. In this tutorial, you are provided examples of how to import FITS files, access header information, manipulate the HEALPix data, visualize skymaps, and conduct basic analyses of the data in Python. 

## Quick Start
Please note that the code in this tutorial relies on the [Healpy](https://healpy.readthedocs.io/en/latest/index.html) Python library, which does not support Windows natively. If you wish to run the code on Windows, please use the [Windows Subsystem for Linux](https://learn.microsoft.com/en-us/windows/wsl/install).

If you wish to interact with the notebook directly:

1. Download [Planck_Telescope_Data_Tutorial.ipynb](https://github.com/asc-csa/Planck-Telescope-Data-Tutorial/blob/main/Planck_Telescope_Data_Tutorial.ipynb).
2. Open a terminal in the location of the notebook and enter the following command to install the required libraries:
``` pip install -r requirements.txt ```
3. If you have not previously used Jupyter Notebooks, install it with:
``` pip install notebook ```
4. Enter the following command to launch a local Jupyter Notebook server:
``` jupyter notebook ```
5. Open the URL it provides in your browser, and experiment with the tutorial.

Otherwise, you may simply use the code directly in your own Python scripts.