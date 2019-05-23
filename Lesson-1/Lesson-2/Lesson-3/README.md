# Créer des branches 

## Quoi de neuf vieille branche ?

Une branche, est un élément que vous allez souvent être amenés à utiliser lorsque vous travaillez sur un repository.

Les branches permettent de travailler sur des versions de code qui divergent de la branche principale contenant votre code de base.

En gros chaque branche va probablement contenir un ou des commits et probablement des modifications dans les fichiers, donc une branche est une autre version du code, dont les commits constituent l'historique.

Vous comprendrez aisément qu'il est très important de savoir se positionner sur la bonne branche, et sur le bon commit.

Nous avons déjà vu comment voir les commits, et s'y positionner.

Nous allons maintenant voir comment créer une branche.

## Manipulez le branchez

Lorsque vous initialisez un repository Git, votre code est placé dans la branche principale appelée master .

Voici les commandes qui vous permettent de manipuler les branches :

Pour voir les branches présentes dans votre repository , utilisez la commande :: 

* git branch -a * 

Elle vous retournera toutes les branches présentes, et ajouteras une étoile devant la branche dans laquelle vous êtes placés.

Pour créer un nouvelle branche, il vous suffit d'ajouter le nom de la branche à créer à la suite de la commande suivante :

* git branch ma-nouvelle-branche *

Votre nouvelle branche hérite du contenu de la branche depuis laquelle vous l'avez instancier, si vous l'avez créer depuis votre branche master qui elle même contenait un dossier HTML  et un dossier CSS, alors votre nouvelle branche sera créer avec ces mêmes dossiers et les fichiers qui les composent.

Vous pouvez donc par exemple créer une branche monProjet-V1.0

Pour vous placer dans une autre branche à l'intérieur de votre repository, vous allez de nouveau avoir besoin du mot clé checkout.

* Git checkout ma-nouvelle-branche. *

Une fois sur cette branche vous pouvez toujours utilisez les commandes git status et et git log

Cela vous permettras de procéder à quelques vérifications avant de travailler sur la branche.

Vous pouvez également utilisez le commutateur -f pour forcer la commande si une erreur survient.

## Fusionnez les branches

Lorsque vous travaillez sur plusieurs branches , il va souvent vous arriver de vouloir ajouter dans une branche A les mises à jour que vous avez faites dans une autre branche B . Pour cela , on se place dans la branche A.

* git checkout brancheA * 

Puis vous pouvez fusionner une branche dans la branche sur laquelle vous vous situez avec la commande git merge 

* git merge brancheB *

En clair vous êtes aller sur la branche, brancheA, et vous avez demander d'y intégrer le contenu de la branche, brancheB

Bravo vous savez comment fusionner vos branches !




