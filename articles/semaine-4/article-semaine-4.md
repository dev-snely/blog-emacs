** Bonjour à tous! 

J'espère que vous aller bien. Ajourd'hui, je vous propose de une légère introduction à l'outil Org-mode. Comme l'explique si bien [sa page de Wikipédia](https://en.wikipedia.org/wiki/Org-mode), Org-mode est un *mode* qui permet la modification, le formattage et l'organisation d'entre autre le planification, les notes et la création à l'intérieur d'Emacs. En gros, Org mode prend du texte brut écrit pas son utilisateur et enregistre ses fichiers en *.org* . Les fichiers *.org* comprennent le markdown et utilise ses attributs pour justement démarqué différent parties de textes en niveau hierarchique.    

** Installation

L'installation est très simple. Dirigez vous dans votre fichier de configuraion *~/emacs*, *init.el** ou *emacs.el*. Écrivez: "(use-package org)" et le tour est joué. Question d'esthétisme totalement subjective, j'ai de mon côté ajouté un package réalisé par Daniel Mendler. Le package s'appele [org-modern](https://github.com/minad/org-modern). Justement, il modernise le mode Org dans Emacs. Ainsi, le contenu rendu est très clair, ce qui est idéal pour un outil servant l'organistation. J'ai pris la liberté de prendre le fichier .org de Daniel Mendler qui montre un début de ce que le Mode Org peut faire. Dans ma configuration Emacs voici ce à quoi ressemble Org-mode: 

![edt-org-mode](https://git.dti.crosemont.quebec/slys/public-md-files/-/raw/main/src/images/org-modern.png) 

** Ce que je trouve les plus intéressants de l'exemple:

*** Niveau hiéarchique

On peut séparer nos sections par sujet, sous-sujet, sous-sous-sujet et ainsi de suite. Le processus est plutôt simple, il ne suffit simplement que de précédé notre titre de section d'astérisques. Un astérisque pour un titre de niveau 1, deux pour un autre de niveau 2. C'est la même chose qu'on fait lorsqu'on écrit du markdown.

Les niveaux hierarchique sont efficaces dans Org-mode parce qu'ils peuvent être fermés. Avec la touche de tabulation, on peut fermé tout une section et la rouvrir. Plus, la touche Maj maintenue avec la touche de tabulation permet de fermé ou ouvrir toutes les sections. Ainsi, en fermant toutes les sections, on voit très bien ce qui forme l'ensemble de de notre fichier org. On peut comparé cela à une table de matière que l'on peut ouvrir et fermé à l'aide de raccourcis clavier. 

*** Liste de tâches

On peut se faire des liste de tâche à faire. Parfait pour mettre à côté de soit si on a plusieurs choses à accomplir au cours d'une journée. Org-mode offre pour cela :

 - Des libelés pour marqué l'état dans nos priorités. Ex: [#A], [#B], [TODO], [DONE] 
 - Des boites à coché pour marqué l'état d'une tâche dans nos priorités. Ex: [X], [-], [ ]
 - Des Timestamps qui permettent d'ouvrir le mode Agenda sur clic et y mettre les tâches dans l'agenda Emacs. 
 - Des libelés personnalisé pour marqué le type de priorité. Ex: Écris du Mardown sur Emacs Org-mode :Markdown:Emacs:Org-mode:  Les libelés sont écris entre deux-points.
    
L'édition des tâches est rapide, surtout quand on connait les raccourcis clavier que nous offre le mode. Entre autre, la touche Maj maintenue avec les touches de flèches permettent la navigation dans les tâches ou l'ajout de libellé comme montré dans l'exemple ci-haut. Prendre le temps d'apprendre à utiliser cet outil de listage peut nous sauver du temps en terme d'édition, parce qu'il faut gardé en tête que rien n'est fait à la souris. Tout ça est possible par le clavier uniquement. Org-mode se charge du rendu visuel à lui seul.

*** Les blocks de code et les tableaux

Pour ce qui sont des blocks de code et des tableaux, je me verrais moins les utiliser. Il n'empêche que leur présence montre un peu la puissance de l'outil Org-mode au nouvel arrivant. Si je peux conseiller un vidéo qui m'a piqué mon intérêt pour org-mode ce serait [celle-ci](https://www.youtube.com/watch?v=SzA2YODtgK4). Selon moi, cette vidéo démontre très bien l'utilisation de block de code et de tableaux. 

** Voilà pour aujourd'hui

Merci d'avoir lu mon article. Org-mode dans Emacs est un outil qui promet énormément selon la communauté Emacs. Ce n'est pas un outil limité au programmeur. C'est plutôt un outil qui offre un grand avantage à celui qui écrit beaucoup au clavier, pour l'école ou le travail. En effet, Org-mode permet de faire d'écrire des textes, faire des listes de priorités et tâches, écrire du code ou même bâtir des tableaux et tout ça sans déplacer la souris une seule fois. 

** Documentation

