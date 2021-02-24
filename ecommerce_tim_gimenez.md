#Q1: Quelle est la différence entre un fork et un clone ?
Un fork est une copy d'un projet déjà existant dans un dépot différent que celui-ci. Tandis qu'un clone est positionné avec le même dépot distant.

#Q2: Github propose un clone ou download ( bouton vert ), quelle est la différence fondamentale entre les deux ?
Le download télécharge uniquement le contenu du projet sans pour autant y avoir un dépot distant git d'attribué. Le clone quant à lui permet de se brancher directement sur le dépot distant.

#Q3: Quelle est la commande git permettant de visualiser l'historique du projet ?
git log

#Q4: Chaque commit a un numéro unique, seriez vous retrouver celui du cinquième commit de ce repository ?
commit 5651629bb4da4aa2298339d7daa58247d25c4bfb
Author: gbesset <guillaume.besset.pro@gmail.com>
Date:   Thu Jan 21 16:34:42 2021 +0100

#Q5: D'ailleurs comment savoir, quel est le contenu de ce cinquième commit, c'est à dire quelles ont été les modifications apportées au projet au 3ième et 4ième commit ?
La commande permettant de savoir quel est le contenu du cinquième commit est : git diff "l'id du commit"
- git diff 5651629bb4da4aa2298339d7daa58247d25c4bfb

#Q6: Juste avant de commiter, quelle est la commande pour visualiser le contenu de son prochain commit ?
La commande permettant de visualiser le contenu de son prochain commit est "git status"

#Q7: Pourquoi la première personne peut partager ses changements sans problème et les autres sont obligées de faire une opération supplémentaire ?
Parce qu'il faut que le projet soit d'abord mis à jour localement afin de pouvoir corriger les conflits s'il y en a puis de mettre à jour le dépot distant.



