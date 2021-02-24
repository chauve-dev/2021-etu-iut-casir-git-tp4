__**Q1: Quelle est la différence entre un fork et un clone ?**__

La différence entre un fork et un clone est que lorsqu’on fork un lien existe entre notre fork et le projet original. Cela permet de pouvoir faire des pull request sur le projet original, cela veut dire que nos modifications pouront être examinée par l'auteur du dépôt original. C'est trés utilile pour les projet open source car tous le monde peut y participer.

Lorsqu’on clone un projet, on ne va pas pouvoir contribuer au projet d'origine et on ne pouras pas non plus accéder au données remote et donc on ne poura pas contribuer au projet.A moins bien sur que le propriétaire du projet d’origine ne nous accorde des droits spéciaux pour pouvroire le faire.



__**Q2: Github propose un clone ou download ( bouton vert ), quelle est la différence fondamentale entre les deux ?**__

Le clone permet aussi de récupérer les branche alors que le download ne permettra que de récupérer le code source de la branche active. Il nous le téléchargera alors en .zip



__**Q3: Quelle est la commande git permettant de visualiser l'historique du projet ?**__

La commande permettant la visualisation du projet et le `git log`. Elle permet d'acces a l'historique des commits.



__**Q4: Chaque commit a un numéro unique, seriez vous retrouver celui du cinquième commit de ce repository ?**__

Le numéro du commit et le `5651629bb4da4aa2298339d7daa58247d25c4bfb` je les retrouver en effectuant la commande `git log` et en comptant depuis le premier commit jusqu'à 5 j'ai trouver le numero du commit.



__**Q5: D'ailleurs comment savoir, quel est le contenu de ce cinquième commit, c'est à dire quelles ont été les modifications apportées au projet au 3ième et 4ième commit ?**__

La commande pour connaitre les modification entre le 3ème et le 5ème commit et la suivante : `git diff 5651629bb4da4aa2298339d7daa58247d25c4bfb 5bf2b0e7ce93189056af052a731a1207b36254fa`


__**Q6: Juste avant de commiter, quelle est la commande pour visualiser le contenu de son prochain commit ?**__
La commande pour visualisée le statut et `git status`

__**Q7: Pourquoi la première personne peut partager ses changements sans problème et les autres sont obligées de faire une opération supplémentaire ?**__

Les autre devlopper doivent récupérer les changements emis par le premier dans le but de modifier la même base de code ensuite.

__**Q8: Quel est le concept en git qui nous permet de procéder ainsi ?**__
Le consepte et celui des commit atomique. Pour ce faire avant de faie le commit il faut ajouter cellement les fichier concerner par le commit avec  `git add nomfichier`

__**Q9: Quelles sont les étapes pour résoudre des conflits sous git ?**__
* Etape 1 : Faire un `git push` et avoir un conflie indiquer
* Etape 2 : Faire un `git pull` pour récupérer le code distant
* Etape 3 : Modifier le ou les fichier responsable du conflit
* Etape 4 : Ajouter les fichier une fois modifier avec un `git add <lesfichiers>`
* Etape 5 : Commit les modification apporter avec un `git commit -m"Edit : Mes modif"`
* Etape 6 : Faire un `git push` pour résoudre définitivement le conflit

__**Q10: Comment vous vous assurez que git n'est plus en état de conflit ?**__
La commande `git status` indiquera si le fichier et encore en état de conflit

__**Q11: Quel fichier a été modifié par le script ?**__
le fichier modifier par le script et le script.js. Pour le savoir j'ai utiliser la commande `git status`

__**Q12: Ecrasez les modifications faites sur ce fichier en utilisant git**__
pour revenir au status précédent du fichier j'ai utiliser la commande `git checkout -- src/js/script.js` qui permmet de faire revenir un fichier spécifique à son précédent state

__**Q13: Faire un git status, qu'observez vous ?*__
Dans le git status il y avait une immage non ajouter.

__**Q14: NB: vous pouvez faire ça uniquement sur des commits non partagés. Pourquoi ?**__
car on ne peut pas faire des ammend car si des personne on utilise une ancinne version du commit il vas y avoir des confli sur le nouveau commit; 

__**Q15: Erreur script:__**
    
**Visualiser votre historique, que s'est t-il passé ?**
Il y a eu 5 nouveau commit ajoutatn
    
**Comment revenir en arrière et donc ignorer les 5 derniers commits ?**
il faut utiliser la commande `git revert 13644c973b62e37ae0f7b1aa7361f3355a3e9903` qui vas annuler tous les changement jusqu'à ce momment lagit

__**Q16: Résumé en une phrase l'intérêt des branches :**__
Les branche permettre de séparer le devloppement d'une application par fonctionalite version stable et de dévloppement. c'est particulièrement utile lorsque plusieur perssone travail sur des fonctionalitée différente.

__**Q17: Sans le savoir vous travaillez déjà avec des branches, quel est le nom de la branche par défaut de git ?**__
on travail depuis le début sur master

