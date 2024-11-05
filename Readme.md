## Morpion (Ce jeu n'est pas facile non plus !)
- Le but de ce jeu est de r�aliser un jeu du morpion, il vous faudra utiliser des tableaux et si possible factoriser au maximum avec des fonctions comme on l'a vu.
- Le jeu se passe au tour par tour entre deux joueurs sur un plateau de cases en 3x3
- Le premier joueur qui d�bute la partie est al�atoire !
- Ce premier joueur r�alisera des ronds, tandis que le second joueur r�alisera des croix
- Le but est donc de choisir un emplacement o� le joueur d�cide de mettre son signe (attention, un endroit d�j� pris ne doit pas pouvoir �tre repris � nouveau). Vous pouvez par exemple donner des possibilit�s de A1 � C3 pour que l'utilisateur choisisse l'emplacement (ou de 1 � 9 si vous pr�f�rez)
- La premi�re personne qui gagne est celle qui arrive � faire une ligne compl�te de son signe (en ligne verticale, horizontale ou diagonale) Cette �tape n'est pas facile !
- Le but est d'�galement afficher dans la console un tableau qui r�capitule o� l'on en est dans la partie au fur et � mesure des tours des joueurs



Sc�narios BDD pour le Morpion
Les sc�narios suivants d�crivent les comportements attendus pour les fonctionnalit�s du jeu :

1. Sc�nario : D�marrer une nouvelle partie
�tant donn� que le joueur 1 et le joueur 2 sont pr�ts � jouer
Quand le jeu commence
Alors un plateau de jeu vide doit �tre affich�

2. Sc�nario : Jouer un tour
�tant donn� que le joueur 1 a le symbole "O"
Et le joueur 2 a le symbole "X"
Quand le joueur 1 choisit la case A1
Alors la case A1 doit �tre remplie avec "O"
Et c'est au tour du joueur 2

3. Sc�nario : Gagner une partie
�tant donn� que le joueur 1 a "O" et que le joueur 2 a "X"
Et que le plateau est dans cet �tat :


O | O | O  
- - -  
X |   | X  
- - -  
  |   |  

Quand le joueur 1 joue sur la case C1
Alors le joueur 1 doit �tre d�clar� vainqueur

4. Sc�nario : Jouer dans une case d�j� occup�e
�tant donn� que la case A1 est occup�e par "O"
Quand le joueur 2 essaie de jouer sur A1
Alors un message d'erreur doit �tre affich� indiquant que la case est d�j� occup�e

5. Sc�nario : Match nul
�tant donn� que le plateau est plein et qu'aucun joueur n'a gagn� :


O | X | O  
- - -  
X | O | X  
- - -  
X | O | O  

Quand le joueur 2 joue son dernier coup
Alors un message doit indiquer que le match est nul