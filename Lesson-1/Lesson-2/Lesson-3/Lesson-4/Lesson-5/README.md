# Annuler des changements

> Attention les tutoriels suivants sont inspirés de [This link](https://learngitbranching.js.org/)
> Nous ferons de notre mieux pour y ajouter des informations supplémentaires



## Revert ou Reset ?

Il y a de nombreuses façons d'annuler des changements avec Git. De même que pour les commits, annuler des changements avec Git est à la fois un aspect bas-niveau (gestion des fichiers et morceaux de fichiers) et un aspect de plus haut niveau (comment les changements sont effectivement annulés). Nous allons nous intéresser à ce dernier point.

Il y a principalement deux façons d'annuler des changements avec Git : l'une est git reset et l'autre est git revert. Nous allons maintenant voir chacune de ces façons.

## Reset

git reset annule des changements en déplaçant la référence en arrière dans le temps sur un commit plus ancien.


En ce sens, on peut considérer cela comme une façon de "réécrire l'histoire"; 

git reset fait remonter une branche en arrière comme si le(s) commit(s) n'avait jamais eu lieu.

Que va faire la commande suivante : 

* git reset HEAD~1

elle va simplement déplacé la référence de la branche courante en la faisant revenir sur d'un niveau dans l'arborescence;

Désormais notre repository est dans le même état que si le commit sur lequelle vous étiez n'avait jamais eu lieu.


## Revert

EN utilisant la commande revert, le résultat sera légérement différent, testons la commande suivante :

* git revert HEAD

Un nouveau commit est apparu en bas sous le commit que nous voulions annuler. 
 
Ce nouveau commit introduit des modifications (celles qui correspondent justement à l'annulation de celles du commit sur lequelle vous avez effectuer la commande.)

