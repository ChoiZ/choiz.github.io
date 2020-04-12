Title: Faire un va et vient avec des interrupteurs muraux Xiaomi
Date: 2020-04-12 17:37:45
Author: choiz
Category: text
Tags: Domotique, Electricité, Xiaomi
Slug: 2020-04-12-faire-un-va-et-vient-avec-des-interrupteurs-muraux-xiaomi
Status: published

J'ai recherché longtemps comment faire un va et vient avec des interrupteurs muraux Xiaomi.

![Xiaomi switch wall]({static}/images/xiaomi-switch-wall.png)

La seule solution proposée était de mettre :

- un interrupteur filaire.

- un interrupteur sans fil.

Cette solution ne me convient pas car j'ai des interrupteurs encastrés, je n'ai pas envie d'avoir un interrupteur sans fil collé, alors que j'ai potentiellement de l'electricité a cet endroit et je ne veux pas changer les piles…

J'ai donc pas mal fait de recherches, tests etc… pour au final trouver comment faire un va et vient "classique" comme on le fait avec des interrupteurs standards.

![Schéma va et vient]({static}/images/schema-va-et-vient-classic.png)

Pour que le va et vient fonctionne avec deux boutons xiaomi filaire il vous faut :

- un va et vient electrique type lumière d'escalier

- un circuit classique type lumière d'une entrée (avec un seul interrupteur) qui soit a coté d'un des deux interrupteurs va et vient

- un interrupteur deux boutons Xiaomi (un bouton sera alimenté par le deuxième circuit electrique, l'autre bouton sera pour le va et vient (slave) et n'aura pas besoin d'alimentation car il fonctionnera en sans fil et sans pile, il enverra l'ordre au master d'allumer ou éteindre)

- un interrupteur un bouton (ou deux boutons) pour le deuxième bouton du va et vient (master).

- un wago 2 bornes

- 2 wago une borne (pour la deuxième navette inutile)

- un cache (obturateur) si on remplace 2 interrupteurs un bouton par un interrupteur deux boutons.

Je prend l'exemple d'un va et vient dans un escalier (RDC - premier étage), avec 2 interrupteurs en bas :

- un qui alimente l'ampoule de l'entrée

- un qui alimente l'ampoule de l'escalier (va et vient)


**ATTENTION :**

**Avant toute intervention sur votre installation électrique, couper le disjoncteur général. Je ne pourrais en aucun cas être tenu pour responsable de vos agissements. Ce document est uniquement a titre d'information. Je ne pourrait être tenu pour responsable de tout dommages ou incidents.**

![Schéma va et vient xiaomi]({static}/images/schema-va-et-vient-xiaomi.png)

Je démonte au RDC, mon interrupteur de l'entrée, et mon ancien interrupteur avec va et vient classique, je me retrouve donc avec sur l'interrupteur de l'entrée :

- la phase pour la lumière de l'entrée

- le câble allant vers la lumière de l'entrée

sur l'interrupteur va et vient (bas) :

- la phase

- deux navettes

Je remplace mon interrupteur de l'entrée par l'interrupteur xiaomi :

- la phase sur le "L"

- le câble allant vers la lumière de l'entrée sur le "L1" ou "L2" a voir quel bouton vous souhaitez utiliser pour l'entrée et votre va et vient

Je prend mon wago ou équivalent, je branche :

- la phase de l'interrupteur va et vient (bas)

- une navette (pour alimenter mon second interrupteur du premier étage)

- le wago une borne sur la navette restante

- je referme avec un "obturateur" pour avoir une finition propre

Au premier étage j'ai toujours mon interrupteur classique fonctionnel je le laisse connecté pour savoir laquelle des deux navettes est sur notre wago (avec la phase). L'autre navette n'est pas connectée pour l'instant.

N'oubliez pas de re-couper le disjoncteur !

Démonter l'interrupteur du haut. Marquer d'un morceau de scotch electrique rouge de préférence la navette avec la phase.

Sur l'autre navette mettre le deuxième wago une borne.

Connecter votre interrupteur Xiaomi du haut un bouton (ou deux boutons) en plaçant :

- la phase obtenu par le Wago et par la navette avec le scotch rouge sur la borne "L" de votre interrupteur

- le fil précédent allant sur votre ampoule sur la borne "L1" de votre interrupteur.

Refixer l'interrupteur et tester le fonctionnement de celui-ci.

Si vous avez un interrupteur deux boutons en haut le deuxieme bouton peut également être utilisé en mode sans fil pour un autre appareil ou êteindre votre entrée d'en haut par exemple (a voir si c'est utile).

Pour que le va et vient soit fonctionnel, il ne vous reste plus qu'a activer le mode sans fil sur le deuxième bouton de votre interrupteur de l'entrée. Celui-ci doit déclencher sans fil l'interrupteur de l'escalier qui se trouve en haut.

J'ai personnellement trois va et vient qui fonctionnent ainsi grâce à plusieurs boutons situés a proximité les uns des autres.