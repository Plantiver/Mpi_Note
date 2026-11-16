



















# [[Info - Lesson - 6|Décidabilité]]
### 1
On introduit $tr$ qui "oublie" les étiquettes d'un automates, et l'on regarde s'il existe un chemin entre l'un des sommets initiaux vers l'un des sommets terminaux.

On calcule le determinisé de nos deux automates, puis on regarde s'il sont équivalent.

### 2
Supposons l'existence de $He$ l'algorithme qui résout l'arrêt exhaustif.
Alors:
```pseudo-code
H(S,e):
    renvoyer He(
        F(e'):= Si e'!=e Boucler sinon S(e)
    )
```
Or le problème de l'arrêt est indécidable.
Donc $He$ n'existe pas.

Soit $T$ l'algorithme qui résout trivialité, alors:
```pseudo-code
He(S):
    
```
#todo : finish the exo





































