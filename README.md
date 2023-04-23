le projet est composé de 5 dossier au total : 
1) IA
2) player
3)player2
4)readme
5)requirements

premièrement, le dossier readme et requirements permettent d'expliquer respectivements les stratégies mises en places et les dépendances nécessaires au bon fonctionnement du programme.

Ensuite, vient les dossiers constituants véritablement le programme : 
le dossier IA :
 il est constitué de plusieurs parties. Premierement, l'objet "serverAI" qui sera notre lien avec le serveur, elle possède plusieurs fonction dont sa connexion au serveur de jeu ainsi que ses interactions avec celui-ci. Via les modules sockets et json nous pouvons envoyer une réponse au serveur qui nous autorisera à jouer notre partie. pour imformations le module "logging" n'est pas nécessaire au bon fonctionnement du programme, il permet simplement de vérifier les bonnes connexions que l'IA effectuent.

 Deuxiemement, l'objet randomAI simule une IA qui aurait un comportement erratique, elle peut effectuer des "badmoves" ( déplacement invalides aupres du serveur ) et ne tient pas compte de la partie qui se déroule. 


 Dernierement, l'objet AI qui est notre IA principal. contrairement à l'ia random elle possède une réelle logique. 

les dossiers player et player 2 sont très ressemblant, en effet , ces deux dossiers permettent simplement de ne pas surcharger le ficher IA car il possèdent les réponses à envoyer au serveur principal et le moyen de les encoder en utilisant le module json. 


Fin de la brève explication 

Maintenant pour expliquer plus en détail le projet j'expliquerai surtout la partie intelligence de l'IA car je ne pense pas que les autres parties méritent de plus amples imformations. 

La grande différence entre l'IA et la random IA se trouve dans leurs choix. en effet, la random IA est codé de facon a ce que les mouvements qu'elles effectuent aient une part de randomness si il lui reste un mouvement a faire, l'IA random  le fera or l'IA principal décidera elle même de ne pas jouer si cela est impossible évitant ainsi tout ("badmoves").













