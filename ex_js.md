https://jsfiddle.net/tbo47/qsuy92ht/

Sur le lien ci dessus, il y a une partie html, une partie css, une partie javascript.
Le rectangle en bas a droite est le rendu finale. 
Il faut appuyer sur le boutton play en haut a gauche pour rafraichir la partie en bas a droite.


La fonction `openstreetmapGetPOIs` prend 2 arguments. 
Le premier est un carre de coordonnee gps, le deuxieme est le type de point d interet qu on veut lister.
Comme on peut le voir, le premier argument (en ligne 6) est coder en dure. 
Je voudrais que ca soit dynamique et que ca vienne de l'appel javascript `navigator.geolocation.getCurrentPosition`. 
C'est a dire qu on ajoute ou retranche `0.1` a la latitude/longitude pour creer un tableau de 4 valeurs a donner a la fonction `openstreetmapGetPOIs`

Idealement, le candidat ecrira du code lisible asynchrone.