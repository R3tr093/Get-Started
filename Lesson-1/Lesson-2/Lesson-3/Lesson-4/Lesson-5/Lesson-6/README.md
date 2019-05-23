# Déplacer votre travail

## Introduction

Nous avons maintenant pratiqué les bases de git.

Ces seuls concepts sont suffisants pour utiliser 90% du pouvoir des dépôts git et satisfaire les principaux besoins des développeurs.

Les 10% restants, cependant, peuvent être assez utiles pour les systèmes assez complexes (ou quand vous vous êtes mis tout seul dans le pétrin). Le prochain concept que nous allons aborder est "le déplacement de travail" (moving work around) -- en d'autres termes, c'est une façon pour les développeurs de dire "Je veux ce travail ici et cet autre là.".

Cela peut sembler compliqué, mais c'est un concept simple.

## La commande : Cherry-pick

La première commande de cette série est git cherry-pick. Elle a le prototype suivant :

    git cherry-pick <Commit1> <Commit2> <...>

C'est une manière simple de dire qu'on voudrait copier une série de commits en-dessous de notre emplacement actuel (HEAD).
