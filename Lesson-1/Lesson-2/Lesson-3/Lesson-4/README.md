# Résoudre un conflit

## Comment résoudre un conflit de fusion

Nous avons vu comment fusionner des branches , nous avons utilisez un exemple assez simple ou tout s'est bien passé. Mais il arrive très souvent qu'il se produise des conflits entre les deux branches qui empêchent de les fusionner , par exemple lorsque plusieurs personnes travaillent en même temps sur un même fichier .

Exemple : Dans votre branche Master il y a un fichier Hello.md avec une ligne de texte " Hello world " . Votre branche universal contient un fichier Hello.md avec une ligne de texte : Hello brave new world " .

Si vous tentez de fusionner la branche universal dans la branche master :

* git checkout master

* git merge universal

Git va reconnaitre qu'il existe un conflit entre les deux branches car la 1re ligne du fichier Hello.md est différente dans chacune des branches et vous verrez s' afficher le message suivant.

Auto mergin hello.md
CONFLICT(content): Merge conflict in hello.md
Automatic merge failed ; fix conflicts and then commit the result

Vous allez donc devoir ouvrir le fichier hello.md dans votre éditeur de texte, ou à partir de la commande vim : vim hello.md

Vous allez alors voir les différences de contenu du fichier hello.md entre les deux branches , et vous pouvez choisir quel contenu garder pour la branche master dans laquelle vous souhaitez fusionner.

Par exemple vous pouvez garder "Hello world" sauvegarder le fichier et revenir dans la console .

Maintenant que vous avez résolu le conflit, il vous reste à le dire à Git, car pour l'instant si vous faites un git status, git vous dira que vous avez des branches non fusionnées ("unmerged paths").

Pour cela faites un commit sans message :  Git commit

Git va détecter que vous avez résolu le conflit et vous proposer un message de commit par défaut .

Vous pouvez alors personnaliser le message du commit si vous le souhaitez. Dans notre cas, la résolution étant assez simple, nous allons garder le message proposé par défaut.

Git va alors vous confirmer que vos branches ont été fusionnées, et si vous consulter l'historique des commits avec la commande que vous connaisez déjà ::  git log, vous verrez alors apparaitre le dernier commit de résolution du conflit avec le message :

Merge branch universal
CONFLICTS:
Hello.md
