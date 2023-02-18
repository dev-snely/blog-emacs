** Bonjour à tous! 

J'espère que vous aller bien. Ajourd'hui, je vous propose de une légère introduction à l'outil Org-mode. Comme l'explique si bien [sa page de Wikipédia](https://en.wikipedia.org/wiki/Org-mode), Org-mode est un *mode* qui permet la modification, le formattage et l'organisation d'entre autre le planification, les notes et la création à l'intérieur d'Emacs. En gros, Org mode prend du texte brut écrit pas son utilisateur et enregistre ses fichiers en *.org* . Les fichiers *.org* comprennent le markdown et utilise ses attributs pour justement démarqué différent parties de textes en niveau hierarchique.    

** Installation

L'installation est très simple. Dirigez vous dans votre fichier de configuraion *~/emacs*, *init.el** ou *emacs.el*. Écrivez: "(use-package org)" et le tour est joué. Question d'esthétisme totalement subjective, j'ai de mon côté ajouté un package réalisé par Daniel Mendler. Le package s'appele [org-modern](https://github.com/minad/org-modern). Justement, il modernise le mode Org dans Emacs. Ainsi, le contenu rendu est très clair, ce qui est idéal pour un outil servant l'organistation. J'ai pris la liberté de prendre le fichier .org de Daniel Mendler qui montre un début de ce que le Mode Org peut faire. Dans ma configuration Emacs voici ce à quoi ressemble Org-mode: 

![edt-org-mode]() 

