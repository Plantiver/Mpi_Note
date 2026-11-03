# Énoncé
On a un graphe connexe pondéré non-orienté, et l'on cherche à calculer l'arbre couvrant de poids minimal.
# Algorithme
```pseudo-code
Entree: G=(A,S,w), un graphe connexe pondéré non-orienté
Sortie: Un ensemble d'arrètes décrivant

R <- []
pour a dans A.sort(w) faire
	si les sommets de a ne sont pas reliés dans R faire
		R <- R+[a]
	fait
fait
=> R
```
# Preuve
#todo : thingies
# Implémentation
