## Morpion (Ce jeu n'est pas facile non plus !)
- Le but de ce jeu est de réaliser un jeu du morpion, il vous faudra utiliser des tableaux et si possible factoriser au maximum avec des fonctions comme on l'a vu.
- Le jeu se passe au tour par tour entre deux joueurs sur un plateau de cases en 3x3
- Le premier joueur qui débute la partie est aléatoire !
- Ce premier joueur réalisera des ronds, tandis que le second joueur réalisera des croix
- Le but est donc de choisir un emplacement où le joueur décide de mettre son signe (attention, un endroit déjà pris ne doit pas pouvoir être repris à nouveau). Vous pouvez par exemple donner des possibilités de A1 à C3 pour que l'utilisateur choisisse l'emplacement (ou de 1 à 9 si vous préférez)
- La première personne qui gagne est celle qui arrive à faire une ligne complète de son signe (en ligne verticale, horizontale ou diagonale) Cette étape n'est pas facile !
- Le but est d'également afficher dans la console un tableau qui récapitule où l'on en est dans la partie au fur et à mesure des tours des joueurs



Scénarios BDD pour le Morpion
Les scénarios suivants décrivent les comportements attendus pour les fonctionnalités du jeu :

1. Scénario : Démarrer une nouvelle partie
Étant donné que le joueur 1 et le joueur 2 sont prêts à jouer
Quand le jeu commence
Alors un plateau de jeu vide doit être affiché

2. Scénario : Jouer un tour
Étant donné que le joueur 1 a le symbole "O"
Et le joueur 2 a le symbole "X"
Quand le joueur 1 choisit la case A1
Alors la case A1 doit être remplie avec "O"
Et c'est au tour du joueur 2

3. Scénario : Gagner une partie
Étant donné que le joueur 1 a "O" et que le joueur 2 a "X"
Et que le plateau est dans cet état :


O | O | O  
- - -  
X |   | X  
- - -  
  |   |  

Quand le joueur 1 joue sur la case C1
Alors le joueur 1 doit être déclaré vainqueur

4. Scénario : Jouer dans une case déjà occupée
Étant donné que la case A1 est occupée par "O"
Quand le joueur 2 essaie de jouer sur A1
Alors un message d'erreur doit être affiché indiquant que la case est déjà occupée

5. Scénario : Match nul
Étant donné que le plateau est plein et qu'aucun joueur n'a gagné :


O | X | O  
- - -  
X | O | X  
- - -  
X | O | O  

Quand le joueur 2 joue son dernier coup
Alors un message doit indiquer que le match est nul