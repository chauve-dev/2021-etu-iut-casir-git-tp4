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



 