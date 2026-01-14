**Git** :outil de gestion de versions pour le code source.



**version control:**permet aux développeurs de gérer le versionnement des fichiers, au lieu de conserver plusieurs copies différentes du même fichier.



**centralisé:**il consiste à avoir un seul dépôt dans lequel tous les développeurs peuvent interagir simultanément.

Le principal problème de cette méthode est que lorsqu’un développeur travaille sur un ou plusieurs fichiers, ceux-ci sont verrouillés afin d’éviter les conflits.

Ainsi, deux développeurs ne peuvent pas travailler en même temps sur un même fichier.



**distribué:(Git)** : Chaque développeur possède une copie complète du dépôt. Le système fournit un dépôt distant ainsi qu’une copie locale pour chaque utilisateur.





**commit:**un objet git ; enregistrant un instantané des fichiers modifiés, indiquant qui l’a réalisé et quand, et faisant partie d’un historique relié par des liens entre commits. 



**comment enregistrer des parametre specifique** :git config --global user.name "Nom"

&nbsp;					     

**branche:**un label de projet ,permet d’isoler des changements au sein d’une chaîne de commits.





**stagging area:**Aussi appelée index ou cache, c’est une zone temporaire où l’on prépare (ou « stage ») les modifications avant de les commiter.

Lorsque vous y ajoutez des fichiers, Git enregistre les changements en stockant le hash et les métadonnées du fichier, ce qui permet de contrôler exactement quelles modifications seront incluses dans le prochain commit.





**interactive rebase:(git rebase -i)** permet de réécrire l’historique des commits : réorganiser, fusionner (squash), modifier, corriger (fixup) ou supprimer des commits afin de garder un historique propre et cohérent.



**stash:**`git stash` met temporairement de côté (ou « stash ») les modifications de votre répertoire de travail, afin de pouvoir travailler sur autre chose, puis revenir et réappliquer ces changements plus tard.





**merge:**Fusionne les changements d’une branche vers une autre tout en conservant les branches divergentes et leur historique.



&nbsp;

**rebase:**Déplace les commits de la branche à rebaser au-dessus des commits de la branche cible, en réécrivant l’historique pour donner l’impression que la branche rebasée a été créée à partir du dernier commit de la branche cible.





**fork :**une copie personnelle du dépôt de quelqu’un d’autre sur une plateforme Git (comme GitHub).

Il permet d’expérimenter et de modifier librement sans impacter le projet original, puis de proposer ses changements via une pull request.



**Cherry-pick :**La commande `git cherry-pick` permet d’appliquer un commit spécifique d’une branche sur une autre.



**Git hooks :** des scripts personnalisés, écrits dans le langage de votre choix, qui s’exécutent automatiquement lors de certains événements Git (commit, push, rebase, etc.).

Ils permettent d’appliquer des règles, d’automatiser des tâches ou d’intégrer d’autres outils, par exemple un hook pre-commit pour lancer des tests ou des linters avant un commit.



**Git Flow :**un modèle de branches strict, conçu pour gérer de grands projets avec des cycles de release planifiés.Il utilise plusieurs branches \*\*longue durée\*\* comme `main` et `develop` (qui ne sont jamais supprimées), ainsi que des branches \*\*courte durée\*\* comme `feature`, `release` et `hotfix`, qui se créent et se fusionnent de manière structurée.





**GitHub Flow :**un workflow plus simple et léger, popularisé par GitHub.

Le développement se fait sur des branches de fonctionnalités créées depuis `main`.

Une fois prêtes, les modifications sont proposées via une pull request, revues, puis fusionnées directement dans `main`.

Les déploiements se font généralement en continu depuis `main`.



**trunk-based development** privilégie des commits \*\*petits et fréquents\*\* directement sur une branche principale unique, appelée `trunk` ou `main`.

Il n’y a généralement pas de branches de release longue durée.

Le code est intégré en continu dans la branche `trunk` (ou `main`) et les releases sont souvent créées directement depuis le trunk, soit en taguant un commit spécifique.



