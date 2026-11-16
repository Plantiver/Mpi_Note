# Énoncé
Le problème de l'arrêt est-il décidable ?
# Idée
On introduis le bon algo (à connaitre), et on déroule le fil.
# Démo
Par l'absurde, supposons que le problème de l'Arrêt est décidable via un algorithme $H$.
Introduisons:
```pseudo-code
algo D(s) ->
    Si H(S,S):
        Boucler
    Sinon:
        Renvoyer
```
Alors, $D(D)$ est absurde.
# Conséquence
Il est impossible de construire un algorithme qui répond à ce problème, pas très pratique pour les compilateurs.