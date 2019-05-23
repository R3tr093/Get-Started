# Premier pas avec Git

## Initialiser les tous !

Pour qu'un dossier puisse être traiter par github il faut qu'il sois initialiser, quand on initialise un dossier cela crée à l'intérieur un dossier .git, c'est grâce à ce dossier que vous pourrez utiliser les capacités de github.

Si un dossier ou ces racines ascendante ne contient pas de dossier .git vous ne pourrez pas utiliser github.

Lorsque qu'un repository est créer depuis github, il contient automatiquement et forcément un dossier .git

Mais si vous désirez envoyer un de vos dossier existant sur votre ordinateur, vers votre compte gitHub il faudra l'initialiser, prêt pour votre première commande ?

git init

Et voilà, votre dossier à été initialiser.


## Clone moi si tu peux !

La première étape consiste à créer un repository depuis github.

Pour cela rendez vous dans le menu et sélectionner créer un repository.

Vous pourrez créer un repository en y créant un fichier README.md lors de la création en cochant une case.

Un fichier avec l'extension md ( markdown ) et un fichier qui vous permet d'éditer un texte avec un style.

Une fois votre repository créer, cliquez le bouton clone or download, vous aurez alors un code qui vous suffira de copier dans votre terminal

![Tux, the Linux mascot](IMG/CLONE.PNG)
![Tux, the Linux mascot](IMG/NEW.PNG)


Rendez vous dans le dossier dans lequelle vous souhaiter stocker votre repository, ensuite entrez la commande suivante :

git clone lienGithub


Ceci aura pour effet de créeer un clone du repository qui se trouvait sur gitHub dans le dossier à partir du quelle vous avez entrer la commande.

Bien joué, vous avez créer votre premier clone. 


## Modifier, commentez !

Vous allez maintenant effectuer votre travail sur votre repository, une fois votre travail vous pourrez laissez un commit.

Un commit est similaire à un commentaire daté, qui permet de garder un oeil sur les modifications apportez a votre repository.

Grâce aux commits vous saurez gardez une trace de vos modifications, pour faire un commit entrer la commande suivante ::


git commit -m " Correction du bug."

Le commit est maintenant accessible sur github, mais aussi depuis votre terminal.

Idéalement un commit est cours et précis, de cette maniére un rapide coup d'oeil vous indiquera en quelques mots le travail effectuer.

<!-- INSERER LA METHODE POUR ACCEDER AU COMMIT DEPUIS LE TERMINAL -->


## Ajouter, pushez !


Une fois que vous avec modifier un fichier, et que vous avez commentez votre travail avec un commit ensuite envoyer votre travail depuis votre terminal vers github.

Avant de pouvoir pushez votre nouveau dossier il va falloir ajouter les fichiers que vous avez modifier pour faire ceci vous allez avoir besoin d'une nouvelle commande :

git add monFichier.txt


Cette commande va ajouter ce fichier vers  votre dossier .git, félicitation votre fichier est prêt à être pushez.

Pushez signifie que votre vous allez envoyer votre dossier vers votre compte github, vous allez mettre à jour le travail que vous avez effectuer sur votre ordinateur vers votre repository, une dernière commande ( oui encore ) :

git push

Cette commande envoye le dossier courant vers github, pour autant que vous soyez en droit de le faire bien sur.


<!-- INSERER CONCLUSION DE FIN ? -->








