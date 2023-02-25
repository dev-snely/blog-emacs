
## Bonjour chers lecteurs et lectrices,
Aujourd'hui nous allons voir 3 extensions qui lorsque combinés, boostent la productivité des utilisateurs **GNU Emacs**.
- Le package **Ivy**
- Le mode **Dired**
- L'outil de recherche **Swiper** 

## Introduction au package Ivy
Emacs est un éditeur de texte extrêmement puissant, mais il peut être difficile à utiliser pour les débutants comme moi en raison de sa complexité. Heureusement, il existe des extensions qui peuvent aider à rendre Emacs plus *convivial et plus facile à utiliser*. L'une de ces extensions est [Ivy (Ce dépôt Github contient les informations sur Ivy & Swiper)](https://github.com/abo-abo/swiper). Comme la documentation le dit, le package Ivy offre des outils flexibles et simples pour la complétion de mini-tampons (mini-buffers) dans Emacs. *En gros*, c'est un outil de complétion de texte qui permet de naviguer rapidement dans les fichiers et les répertoires.

Ivy est un package Emacs qui fournit une interface utilisateur pour les outils de complétion de texte. Il utilise une liste déroulante, en dessous du mini-buffer, pour afficher les suggestions de complétion, ce qui permet de naviguer facilement dans les fichiers et les répertoires. Ivy est **très flexible** et peut être utilisé avec une variété d'outils Emacs, tels que Dired et Swiper.

## Ivy + Mode Dired, l'outil de navigation dans le répertoire
Dired, venant de **Dir**ectory **ed**itor, est un mode d'Emacs disponible dès une fois Emacs installé qui permet de naviguer dans les répertoires de manière interactive. Une fois Ivy activé, la navigation dans Dired peut être beaucoup plus facile à comprendre. 

Pour utiliser Ivy avec Dired, la chose est simple. Il suffit d'activer Ivy en tapant M-x ivy-mode. Ensuite, lorsque vous êtes dans le mode Dired (C-x D), vous pouvez utiliser C-x C-f pour ouvrir un fichier et Ivy affichera une liste déroulante avec les fichiers correspondants dans le répertoire courant. Vous pouvez également utiliser M-x dired-jump pour ouvrir un répertoire et Ivy affichera une liste déroulante avec les fichiers et répertoires disponibles dans le répertoire choisi.

En plus de la navigation, Dired est capable d'effectuer plusieurs autres tâches utiles pour la gestion des fichiers et des répertoires:

- Copier, coller et renommer des fichiers à partir de l'interface.
- Supprimer des fichiers : Dired permet de supprimer des fichiers et des répertoires en utilisant la commande dired-flag-file-deletion.
- Créer des répertoires : Dired permet de créer des nouveaux répertoires en utilisant la commande dired-create-directory.

Pour en savoir plus, consulter [la documentation officielle sur Dired](https://www.gnu.org/software/emacs/manual/html_node/emacs/Dired.html) 

## Ivy + Swiper, le package qui trouve les termes que vous cherchez
[Swiper](https://github.com/abo-abo/swiper) est un outil de recherche de texte pour Emacs qui permet de rechercher rapidement des chaînes de caractères ou si vous voulez, des "Strings" dans un fichier. Swiper utilise Ivy pour naviguer rapidement entre les correspondances de recherche dans un fichier selon la chaîne de caractère demandé. Lorsque vous utilisez Swiper, Ivy affiche une liste déroulante avec les correspondances de recherche, ce qui permet de naviguer facilement entre les résultats trouvé. La liste déroulante est illustré ci-bas. *Grosso modo*, si vous avez déjà utilisé Visual studio code, il y a un outil GUI clickable avec un logo de loupe. C'est ce principe qu'utilise Emacs, mais dix fois plus clair.

Pour utiliser Ivy avec Swiper, vous devez d'abord activer Ivy en tapant M-x ivy-mode. Ensuite, lorsque vous utilisez Swiper (C-s) pour rechercher du texte, Ivy affichera une liste déroulante avec les correspondances de recherche. Vous pouvez naviguer dans cette liste à l'aide des touches fléchées (up, down) ou des touches (C-p pour previous, C-n pour next) et appuyer sur Entrée pour ouvrir le fichier à l'emplacement correspondant.

![ivy-swiper](https://camo.githubusercontent.com/c24c95ba6098d8356fd3ce53a0be20398f1c42b0ff8e1c5f68153160686bbdb1/68747470733a2f2f6f72656d6163732e636f6d2f646f776e6c6f61642f6976792d7377697065722d312e706e67)

Vous pouvez regarder [une démo Youtube d'une dizaine de minute résumant Ivy, Swiper et même Dired en cliquant le lien](https://www.youtube.com/watch?v=VvnJQpTFVDc)

## Documentation

1. Emacs Tw. GitHub - emacs-tw/awesome-emacs : A community driven list of useful Emacs packages, libraries and other items. GitHub. Consulté le 24 février 2023, à l'adresse [https://github.com/emacs-tw/awesome-emacs](https://github.com/emacs-tw/awesome-emacs)
2. abo-abo. GitHub - abo-abo/swiper : Ivy - a generic completion frontend for Emacs, Swiper - isearch with an overview, and more. Oh, man ! GitHub. Consulté le 24 février 2023, à l’adresse [https://github.com/abo-abo/swiper](https://github.com/abo-abo/swiper)
3. Dired (GNU Emacs Manual). (s. d.). Consulté le 24 février 2023, à l’adresse [https://www.gnu.org/software/emacs/manual/html_node/emacs/Dired.html](https://www.gnu.org/software/emacs/manual/html_node/emacs/Dired.html)
4. abo-abo. (2015, 17 avril). swiper screencast [Vidéo]. YouTube. Consulté le 24 février 2023, à l’adresse [https://www.youtube.com/watch?v=VvnJQpTFVDc](https://www.youtube.com/watch?v=VvnJQpTFVDc)

## Conclusion 
Voilà qui conclu, Ivy est une extension très utile pour Emacs qui aide vraiment à rendre la navigation dans les fichiers et les répertoires plus intuitive. Un débutant Emacs qui utilise Dired & Swiper avec Ivy, je pense peux passer un meilleur temps dans l'éditeur de texte. J'espère que vous en ferai bon usage dans votre propre utilisation d'Emacs.

Merci d'avoir pris le temps de lire.

Snely 


