Title: Suppression des branches distantes inexistantes
Date: 2015-08-25 13:43:05
Author: choiz
Category: text
Tags: git, branch, remote, prune, origin
Slug: 2015-08-25-suppression-des-branches-distantes-inexistantes
Status: published

Lors d'un developpement j'ai créé une branche "add\_namespace" qui m'a
permis d'ajouté des namespaces a différents fichiers PHP.

Une fois la modification faite j'ai envoyé ma branche sur l'origin, en
faisant un "pull request" (github) ou "merge request" (gitlab).

Un autre développeur a accepté mon pull request (il a donc mergé la
branche) et a supprimé ma branche de l'origine.

Sur mon environnement je vois toujours cette branche.

> git branch -a
>
> \* master
>
> remote/origin/HEAD -&gt; origin/master
>
> remote/origin/add\_namespace
>
> remote/origin/master

Pour pouvoir effacer cette branche dans le remote, il suffit de tapper
la commande :

> git remote prune origin
>
> Élimination de origin
>
> URL : <git@git.mondomain.com>:mondepot.git
>
>  \* \[éliminé\] origin/add\_namespace

Maintenant, vérifions que tout est propre :

> git branch -a
>
> \* master
>
> remote/origin/HEAD -&gt; origin/master
>
> remote/origin/master