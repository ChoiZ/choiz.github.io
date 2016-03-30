C'est toujours la galère lorsque l'on veut que tout soit propre au
niveau des permissions des dossiers / fichiers.

Souvent la première chose que l'on fait : on va dans chaque dossier et
on vérifie un a un ses fichiers et sous-dossiers. Quand il y a 1 ou 2
dossiers ça va mais quand on en a 40… on utilise une autre technique !

J'utilise pour les dossiers : :

    $ find \`pwd\` -type d -exec chmod 755 {} \\;

et pour les fichiers : :

    $ find \`pwd\` -type f -exec chmod 644 {} \\;

Avec \`pwd\` je vais partir du dossier actuel et remplacer tous les
droits des fichiers et dossiers enfants. Vous pouvez remplacer par un
autre chemin par exemple : :

    find /home/choiz/ -type d -exec chmod 755 {} \\;

    find /home/choiz/ -type f -exec chmod 644 {} \\;