# Workshop : Créer son jeu en Jeu-Pygame

Ce workshop a pour objectif de vous apprendre à créer un jeu 2D en [Python](https://www.python.org/) grâce à la libraire [Pygame](https://www.pygame.org/new).


## Installation

Pour réaliser ce projet, vous avez besoin de Python, et de la librairie Pygame.


### Installer Python

#### Windows

Télécharger et installer Python depuis le site officiel : [https://www.python.org/downloads/](https://www.python.org/downloads/)

#### Fedora
    
    ```sudo dnf install python3-pip python-dev```

#### Ubuntu

    ```sudo apt install python3-pip python-dev```

### Installer Pygame

Télécharger et installer Pygame grâce à la commande suivante :

    ```pip install pygame```

## Créer vos assets

Pour créer vos assets, vous avez besoin d'un éditeur de map et d'un éditeur d'image.

### Créer vos deux maps

Pour commencer, nous allons créer deux maps de format 32x32. Pour cela, nous allons utiliser un éditeur de map, [Tiled](https://www.mapeditor.org/). Télécharger et installer Tiled depuis le site officiel.

Une fois l'outil installer, créer un nouveau projet de format 32x32. Vous pouvez ensuite ajouter des tuiles à votre map. Pour cela, cliquer sur le bouton "Tileset" en bas à droite de l'éditeur. Une fenêtre s'ouvre alors, cliquer sur "Open Tileset" et sélectionner le fichier souhaité.

Une fois les tuiles ajoutées, vous pouvez créer votre map. Pour cela, cliquer sur le bouton "Tile Layer" en bas à droite de l'éditeur. Une fenêtre s'ouvre alors, cliquer sur "New Tile Layer" et nommer votre map.

Une fois votre map créée, vous pouvez la sauvegarder en cliquant sur le bouton "File" en haut à gauche de l'éditeur. Une fenêtre s'ouvre alors, cliquer sur "Save As" et sélectionner le dossier souhaité.

Vous pouvez trouver des tuiles sur le site [OpenGameArt](https://opengameart.org/) ou encore sur [itch.io](https://itch.io/).

Votre map principale doit au moins contenir une maison et un point de spawn pour le personnage. Pour créer un point de spawn, vous devez créer un objet de type "Spawn" et le placer sur la map.

Pour créer un objet, vous devez cliquer sur le bouton "Object" en bas à droite de l'éditeur. Une fenêtre s'ouvre alors, cliquer sur "New Object" et nommer votre objet.

### Créer vos personnages

Pour créer vos personnages, vous allez devoir créer des sprites. Pour cela, nous allons utiliser un éditeur d'image, [Aseprite](https://www.aseprite.org/). Télécharger et installer Aseprite depuis le site officiel.

Ou télécharger des sprites préfaites sur le site de votre choix.

## Créer votre jeu

Pour créer votre jeu, vous allez devoir créer un fichier Python. Pour cela, créer un nouveau fichier dans votre éditeur de texte préféré et enregistrer le sous le nom de "main.py".

Une fois le fichier créé, vous pouvez commencer à écrire votre code. Pour commencer, nous allons importer les librairies nécessaires à notre jeu.

### Exercice 1 : Créer une fenêtre avec la map

Pour commencer, nous allons créer une fenêtre de 800x600 pixels. Pour cela, nous allons utiliser la librairie Pygame.

Nous allons charger la map créée grâce à Tiled dans notre jeu. Pour cela, nous allons utiliser la librairie Pytmx.

Pour mettre d'avoir un rendu plus proche d'un jeu de r fois la map chargée, nous allons créer un groupe de tuiles. Pour cela, nous allons utiliser la librairie Pyscroll.
### Exercice 2 : Créer un personnage

Pour commencer, nous allons créer un personnage. Pour cela, nous allons utiliser la librairie Pygame.

### Exercice 3 : Déplacer le personnage

À partir des key de mouvement du personnage, faire en sorte que le personnage se déplace dans la map.
### Exercice 4 : Créer des collisions

À l'aide des différentes couches de la map, créer des collisions pour le personnage.

Le but est que le personnage ne puisse pas traverser les murs de la maison ou passer sur la maison.

### Exercice 5 : Créer des reliefs

À l'aide des différentes couches de la map, créer des reliefs pour le personnage.

Le but est que le personnage puisse se déplacer derrière les maisons sans qu'il soit visible.