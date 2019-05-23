# Positionnez-vous 

## Se positionner sur un commit

Lorsque vous effectuez une série de commits sur un projet , il peut vous arriver de vouloir remonter dans le temps à la recherche d'erreurs éventuelles par exemple .

Pour vous positionner sur un commit donné de votre historique , il vous suffit d'utiliser la commande  git checkout  de la façon suivante : 

git checkout SHADuCommit

Pour revenir à votre branche master , on utilise la même commande :

git checkout master

Si vous rencontrez un problème vous pouvez utilisez le commutateur -f dans votre commande.

git checkout -f master

La commande checkout permet de se repositionner sur une branche ou un commit, et donc à un moment précis de l'historique du projet.

L'option ou commutateur -f permet de forcer la commande dans le cas ou une erreur se serait produite.

Pour savoir sur quelle branche vous vous situez, utilisez la commande :

git status


## Petite astuce

Vous avez effectuer un commit sur vos modifications, mais dans la précipitation vous vous rendez compte que vous avez omis une information.

Pas de panique, si vous désirez simplement modifier le message de votre dernier commit , vous pouvez utilisez la commande suivante :

 git commit  --amend -m "Votre nouveau message"
 
 Bien sur cette commande modifiera le contenu textuel du message du commit sur lequel vous vous trouvez.
