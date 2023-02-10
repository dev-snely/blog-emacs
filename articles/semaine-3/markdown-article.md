## Introduction

Bonjour aux lecteurs et lectrices d'aujourd'hui,
J'ai pu faire ma veille technologique de cette semaine sur Emacs. Elle a été assez fructueuse. Je vous partage donc mon avancement dans la configuration de mon environnement Emacs et ce que j'ai appris du fameux outil Magit.

## Modus-themes 

Au cours de cette semaine, j'ai pu apporter des améliorations à mon thème environnement. La version vanille de Emacs ne me plaisaît pas. Le soir, j'avais mal au yeux avec le thème claire proposé par défaut et j'aime bien quand mon éditeur de texte à un air moderne. 

Après avoir chercher un peu sur la communauté Reddit d'Emacs [r/emacs](https://www.reddit.com/r/emacs/), j'ai pu trouvé une personne nommée Protesilaos Stavrou qui a lui-même créé des thèmes sombres et claires, puis qui les a plubliés sur le gestionnaire de packages Elpa. Protesilaos a créé sa série de thème, nommées [Modus-Themes](https://protesilaos.com/emacs/modus-themes-pictures) pour qu'ils soients accessibles pour GNU Emacs et conformes aux normes les plus élevées *pour le contraste des couleurs entre les valeurs d'arrière-plan et de premier plan* (WCAG AAA).

On compte deux thèmes, un claire et un sombre. Pour ma part, j'aime les deux et suis à l'aise devant l'écran, ce qui me permet de resté concentré assis sur ma chaise pendant longtemps. Le thème claire a été nommée modus-operandi, du latin pour *manière d'opérer*. Le thème sombre lui a été nommé modus-vivendi, du latin pour *mode de vie*. 

[Voici quelques captures des thèmes réalisés par Protesilaos Stavrou](https://protesilaos.com/emacs/modus-themes-pictures)   

### Les configurations que j'ai pu faire pendant la semaine

#### Avant

![alt text](https://git.dti.crosemont.quebec/slys/public-md-files/-/raw/main/src/images/emacs-vanilla.png)

![alt text](https://git.dti.crosemont.quebec/slys/public-md-files/-/raw/main/src/images/emacs-configure-par-defaut.png)

#### Après

![alt text](https://git.dti.crosemont.quebec/slys/public-md-files/-/raw/main/src/images/emacs-congure-modus-operandi.png)

![alt text](https://git.dti.crosemont.quebec/slys/public-md-files/-/raw/main/src/images/emacs-configure-modus-vivendi.png)

### Brève explication des configutations apportés

À l'aide de mon fichier de configuration situé dans **~/.emacs.d/init.el**, j'ai pu : 

1. Désactiver la barre de déroulement qui était à droite de l'écran.
2. Désactiver les options de menus qui me force à apprendre les raccourcis clavier dont j'ai besoin uniquement. C'est options de menu sont présent par défaut dans le haut de l'éditeur GUI.
3. Désactiver l'écran d'acceuil avec le menu, parce qu'il présente trop d'information sans que ce soit nécessaire.
4. Changer la police de caractère par défaut par JetbrainsMono taille 11. C'est la police qui me fait le plus de sens pour le moment.
5. Ajouter les numéros de ligne sur la gauche de l'éditeur qui me permet de connaître ma location dans dans le fichier.
6. Personnaliser le mode line. Un peu plus gros, avec une couleur accentué sans bordure.
7. Personnaliser le surlignage du contenu, seulement l'arrière plan. Ce qui me permet de voir la couleur de la police de caractère dans un code python par exemple.

### Avantages

Les modus-themes me permettent d'avoir un éditeur de texte très contrasté. Un IDE très constraté facilite beaucoup la tâche du programmeur parce qu'il lui permet de lire plus rapidement, plus clairement et plus facilement. *Lire correctement* est extrêmement important. Lorsque qu'un bug apparaît soudainement, il se peut qu'il soit difficile à trouver dans le code. Un mauvais agencement de couleur pourrait entrainer le programmeur à chercher ou regarder au *mauvais endroit longtemps* dans le code et utlimement le ferait perdre du temps précieux. 

Je n'ai même pas 50 lignes dans mon fichier de configuration **~/.emacs.d/init.el** et je commence déjà à me sentir à l'aise. Pourtant les options sont sans limites. Il ne suffit que d'aller explorer le web pour voir des git avec des fichiers de configurations publics possédant les 1000 lignes. Il y par exemple [celui-ci](https://github.com/mrcnski/init.el/blob/master/init.el) et [celui-là](https://github.com/thierryvolpiatto/emacs-config/blob/main/init.el). 

D'ailleurs, cette article a été écrit avec une extension de config que j'ai pu ajouté depuis ELpa. Cette extension me permet d'écrire du markdown plus clariement sur Emacs. Je ne connais pas tous les raccourcis clavier pour le moment, mais avoir un rendu visuel instantané aide à l'écriture de l'article.

![md-file](https://git.dti.crosemont.quebec/slys/public-md-files/-/raw/main/src/images/markdown-showcase.png)

## Magit


### Qu'est ce que Magit


Magit est un outil Git, puissant de contrôle de version de fichiers Git. Il est intégré dans Elpa comme package disponible pour tous. Magit propose au programmeur utilisant Git dans Emacs une interface conviviale lui permettant d'effectuer les commandes Git habituellement fait en ligne de commande en quelque touches seulement. Il est à noter qu'il faut un mettre un peu de temps pour comprendre le fonctionnement de l'outil et la façon d'y naviguer, cependant l'apprentissage en vaut la peine. Voici à quoi ressemble le menu Magit accessible par **ctrl-x g** (ctrl-x pour commande et g pour git surement?) : 

![ss-magit-menu](https://git.dti.crosemont.quebec/slys/public-md-files/-/raw/main/src/images/emacs-ss-magit-menu.png)

### Quelques fonctionnalités possibles: 

- b, commandes de branches. ex: b, b - permet a l'utilisateur de créer se diriger vers une autre branche ).
- c, commandes sur les commits.
- F, recupérer des branches, depot distants.
- l, voir des logs de commits et le contenu changer depuis son commits parents.
- h, permet de d'obtenir de l'aide on ouvrant la documentation Magit
- et encore plus comme illuster ci-haut 

Les options sont donc beaucoup, mais reste très accessibles. On peut parfois remarquer des noms de commandes Git dont on ne connaissait même pas l'existant.

### Essai de l'option -l ( log )

En appuyant sur la touche -l dans le menu Magit, j'ai pus avoir accès à un log des commits de ma branche actuelle, soit le main. Chaque commit peut être séléctionné en y plaçant le curseur et cliquantsur la touche retour / enter. Magit m'offre alors des d'informations généraux sur le commit séléctionné comme l'auteur, la date et l'heure de création du commit, puis son commit parent. Magit propose aussi une vue plutôt très pertinente qui montre la **différence** dans les fichiers entre le commit actuel et le commit parent. Il est à noter que les zones grise *@@ -0,0 _1,25 @@* peuvent être tabulé, ce qui par conséquence nous permet une lecture plus agréable des changements les plus importants effectués dans un commit. 

Voici à quoi ressemble la sortie de l'option: 

![ss-magit-log](https://git.dti.crosemont.quebec/slys/public-md-files/-/raw/main/src/images/emacs-ss-magit-log.png)

Magit n'est donc vraiment pas l'outil a sous-estimer dans Emacs. 
## Documentation

## Salutation

Merci d'avoir pris le temps de lire la veille technologique de cette semaine. On se retrouve la semaine prochaine pour en connaître plus sur les outils que nous offre Emacs.

Cordialement,

	Snely
