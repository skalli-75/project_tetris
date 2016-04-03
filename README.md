# project_tetris

Equipe du projet Tetris-ESIEA 

 *       Abdellatif SKALLI
 *       Natacha VARIERAS    
 *       Guillaume MERCADAL

Classe utilisée dans le cadre des tests unitaires :  PieceObjectServiceTest (classe fille) (dans la classe mère : AppTest)
Le menu principal de notre projet : App

Principe SOLID :

1. « Single Responsibility  Principle »
Chaque classe dans la conception a un seul rôle, en effet :
  La classe « Piece1 » contient les attributs et les méthodes d’une forme géométrique quelques soit sa forme : son rôle est de décrire la forme de la pièce.
  La classe « Panneau » gère la logique du jeu en termes des mouvements.
  La classe « Grille » contient les parties non mobiles de ce qui seront affichées sur le frame.
  La classe « Gestion » contient les différentes formes des pièces du jeu. Son rôle est de gérer la communication entre la classe panneau et les classes (Grille et piece1).
  La classe « Client »
  La classe « Connexion » permet d'établir et de gérer la connexion entre les différents joueurs
  La classe « Serveur » 

2. « Open closed principle »
  La différenciation entre les deux classes « Piece1 » et « Gestion » permet d’utiliser la classe « Piece1 » dans un autre contexte. Nous avons opté donc pour un choix de composants flexibles à l’extensions et fermés aux modifications.

3. « Dependency inversion principle »

  Ce principe peut être appliqué si nous souhaitons par exemple différencier entre les pièces qui sont en mesure d’effectuer des rotations. Finalement, nous avons remarqué qu’il existe uniquement une seule pièce qui n’admet pas de rotation. 
