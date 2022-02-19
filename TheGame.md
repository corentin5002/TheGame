# The Game

# Pioche

*Pile* de **carte**s

100 cartes

# Carte

- une valeur
- une image/visuel de la carte

# Poser

- Si **pile de jeu** croissante on peut poser la carte si:
    - `PileDeJeuY.sommet < carteMain.valeur`
    - `PileDeJeuY.sommet - 10 == carteMain.valeur`

- Si **pile de jeu** décroissante on peut poser la carte si:
    - `PileDeJeuY.sommet > carteMain.valeur`
    - `PileDeJeuY.sommet + 10 == carteMain.valeur`

- sinon :
    - carteMain n'est pas posable.

# Main

- id joueur (1 à 5)
En fonction du nombre de joueurs :
- 8 cartes pour 1 joueur
- 7 cartes pour 2 joueurs
- 6 cartes pour 3,4,5 joueurs

# Tour

Boucle ou structure indiquant à qui c'est le tour de jouer (et pour les variantes, qui comptabilise le nombre de tours de table).

# Pile de jeu

- id de la pile (y'en a quatre max dans les règles originales)
- type = croissant ou décroissant
- valeur sommet
- pile contenant les cartes successives


- Setter : selon si c'est croissant ou décroissant -> valeur de pile 100 ou 1

# Fonctionnalité

clic and drag : clic gauche pour sélectionner carte de la main et:
- clic gauche pour tenter de poser sur une **pile de jeu**.
- clic droit pour déselectionner la carte

Garder les pile de jeux pour la fin de partie et pour voir la courbe d'évolution des valeurs du sommet des piles de jeux.
