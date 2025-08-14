<p align="center">
   <img src="https://www.asc-csa.gc.ca/images/satellites/planck/planck-animation.jpg" alt="Planck Space Telescope with stylized Cosmic Microwave Background colours over a space backdrop" height=300> 
   <br> Crédit d'image | Image credit: <a href="https://www.asc-csa.gc.ca/eng/satellites/planck/">ASC-CSA</a>
</p>

<p align="center">
    <a href="#stars">
        <img alt="Étoiles sur GitHub | GitHub Repo stars" src="https://img.shields.io/github/stars/asc-csa/Planck-Telescope-Data-Tutorial">
    </a>
    <a href="#watchers">
        <img alt="Spectateurs sur Github | GitHub watchers" src="https://img.shields.io/github/watchers/asc-csa/Planck-Telescope-Data-Tutorial">
    </a>
    <a href="https://github.com/asc-csa/Planck-Telescope-Data-Tutorial/commits/main">
        <img alt="Dernier commit sur GitHub | GitHub last commit" src="https://img.shields.io/github/last-commit/asc-csa/Planck-Telescope-Data-Tutorial">
    </a>
    <a href="https://github.com/asc-csa/Planck-Telescope-Data-Tutorial/graphs/contributors">
        <img alt="Contributeurs sur GitHub | GitHub contributors" src="https://img.shields.io/github/contributors/asc-csa/Planck-Telescope-Data-Tutorial">
    </a>
    <a href="https://twitter.com/intent/follow?screen_name=csa_asc">
        <img alt="Suivre sur Twitter | Twitter Follow" src="https://img.shields.io/twitter/follow/csa_asc?style=social">
    </a>
</p>

---

<h3 align="center" style="border-bottom: none;">
  <a href="#titre-du-projet">Français</a> |
  <a href="#project-title">English (follows)</a>
</h3>

---

<a id="titre-du-projet"></a>
# Données du télescope spatial Planck - Tutoriel

> **Description brève :**
> Ce tutoriel présente des exemples d'importation, de manipulation et de visualisation des données du télescope spatial Planck.


## À propos
**Données du télescope spatial Planck - Tutoriel** est un tutoriel Jupyter Notebook qui guide les utilisateurs à travers l'importation, la manipulation et la visualisation des données du télescope spatial Planck. Il couvre :

- Importation des fichiers FITS et accès aux informations des entêtes
- Manipulation des données HEALPix
- Visualisation des données sur une carte du ciel
- Analyses de base avec les données du rayonnement cosmique de fond

La mission du satellite Planck est la première mission européenne vouée à l'étude de la naissance de l'Univers. Le télescope spatial Planck a été lancé conjointement avec l'Observatoire spatial Herschel à bord d'une fusée Ariane 5, le 14 mai 2009. Il s'agit du télescope spatial le plus sensible jamais conçu pour étudier le rayonnement cosmique de fond, c'est-à-dire les résidus du rayonnement issu du Big Bang qui se sont produits il y a 13,8 milliards d'années.

*Ce tutoriel est fourni à des fins pédagogiques et expérimentales.*


## Prérequis

- Python 3.8 ou plus récent
- Jupyter Notebook ou Jupyter Lab
- Environnement Linux (recommandé) ou Windows Subsystem for Linux (WSL)
- Connexion Internet (pour le téléchargement des données)
- Bibliothèque Healpy (ne supporte pas Windows nativement)


## Démarrage rapide

1. 📦 **Cloner le dépôt**
   ```bash
   git clone https://github.com/asc-csa/Planck-Telescope-Data-Tutorial.git
   cd Planck-Telescope-Data-Tutorial
   ```
2. 🐍 **Créer un environnement**
   ```bash
   # Avec virtualenv
   python -m venv env
   source env/bin/activate

   # Ou avec conda
   conda create -n planck_env python=3.8
   conda activate planck_env
   ```
3. 📥 **Installer les dépendances**
   ```bash
   pip install -r requirements.txt
   ```
4. 🚀 **Lancer le tutoriel**
   ```bash
   jupyter notebook Planck_Telescope_Data_Tutorial.ipynb
   ```

> **Remarque :** Ce tutoriel repose sur la bibliothèque [Healpy](https://healpy.readthedocs.io/en/latest/index.html), qui ne prend pas en charge Windows nativement. Utilisez Linux ou [WSL](https://learn.microsoft.com/en-us/windows/wsl/install).


## Astuces & Conseils

- **Problèmes d'environnement :** Si vous utilisez Windows, activez WSL et exécutez le tutoriel dans un environnement Linux.
- **Performance :** Les données HEALPix peuvent être volumineuses; assurez-vous d'avoir suffisamment de mémoire disponible.
- **Visualisation :** Si les cartes du ciel ne s'affichent pas correctement, redémarrez le kernel Jupyter.
- **Dépannage :** Vérifiez que toutes les dépendances sont correctement installées avec `pip list`.


## Licence

Ce projet est sous une licence MIT modifiée – voir le fichier [LICENSE](https://github.com/asc-csa/Planck-Telescope-Data-Tutorial/blob/main/LICENSE.txt) pour plus de détails.

---

<h3 align="center">
  <a href="#project-title">English </a> |
  <a href="#titre-du-projet">Français (précède)</a>
</h3>

---

<a id="project-title"></a>
# Planck Space Telescope Data Tutorial

> **Brief description:**
> This tutorial demonstrates how to import, manipulate and visualize data from the Planck Space Telescope.


## About

**Planck Space Telescope Data Tutorial** is a Jupyter Notebook tutorial that guides users through importing, manipulating and visualizing data from the Planck Space Telescope. It covers:

- Importing FITS files and accessing header information
- Manipulating HEALPix data
- Visualizing data on skymaps
- Basic analyses of cosmic microwave background data

Planck is ESA's first mission to study the birth of the Universe. Planck was launched jointly with the Herschel Space Observatory aboard an Ariane 5 rocket, on May 14, 2009. The satellite is the most sensitive telescope ever designed to study the cosmic microwave background--the remnants of radiation from the Big Bang 13.8 billion years ago.

*This tutorial is provided for educational and experimental purposes.* 


## Prerequisites

- Python 3.8 or newer
- Jupyter Notebook or Jupyter Lab
- Linux environment (recommended) or Windows Subsystem for Linux (WSL)
- Internet connection (for data download)
- Healpy library (does not support Windows natively)


## Quick Start

1. 📦 **Clone the repo**
   ```bash
   git clone https://github.com/asc-csa/Planck-Telescope-Data-Tutorial.git
   cd Planck-Telescope-Data-Tutorial
   ```
2. 🐍 **Create environment**
   ```bash
   # Using virtualenv
   python -m venv env
   source env/bin/activate

   # Or using conda
   conda create -n planck_env python=3.8
   conda activate planck_env
   ```
3. 📥 **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```
4. 🚀 **Run the tutorial**
   ```bash
   jupyter notebook Planck_Telescope_Data_Tutorial.ipynb
   ```

> **Note:** This tutorial relies on the [Healpy](https://healpy.readthedocs.io/en/latest/index.html) library, which does not support Windows natively. Use Linux or [WSL](https://learn.microsoft.com/en-us/windows/wsl/install).


## Tips & Tricks

- **Environment issues:** If using Windows, enable WSL and run the tutorial in a Linux environment.
- **Performance:** HEALPix data can be large; ensure you have sufficient memory available.
- **Visualization:** If sky maps do not display correctly, restart the Jupyter kernel.
- **Troubleshooting:** Check that all dependencies are properly installed with `pip list`.


## License

This project is licensed under a modified MIT license - see the [LICENSE](https://github.com/asc-csa/Planck-Telescope-Data-Tutorial/blob/main/LICENSE.txt) file for details.

