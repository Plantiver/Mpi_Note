# [[Info - Lesson - 5|Grammaire]]

### 11
Q1:
Tout mot engendré par S contient au moins 1 a.

Q2:
$$
\begin{align*}
S&\to AS_{1}|\varepsilon&&\cr
S_{1}&\to SB&&\cr
A&\to a&&\cr
B&\to b&&\cr
\end{align*}
$$
Q3:

| a   |     |     |     |
| --- | --- | --- | --- |
|     | a   |     |     |
|     |     | b   |     |
|     |     |     | b   |

---

### 12
Q1
$$
S\to Sa|Sb|a
$$
Q2
$$
\begin{align*}
S&\to S'a|S'b|\varepsilon &&\cr
S'&\to S\_a|S\_b&&\cr
S\_&\to Sa|Sb&&\cr
\end{align*}
$$
Q3
$$
\begin{align*}
S&\to Sa|Tb&&\cr
T&\to Ta|\varepsilon&&\cr
\end{align*}
$$
Q4
Soit $L$ reconnaissable par un automate fini $A$, mq il existe une grammaire régulière gauche qui engendre $L$.
On se munit de $e$ l'expression régulière associée à l'automate $A$, et l'on procède par induction:
Montrons par induction que pour toute expression régulière, on peut construire une grammaire régulière droite qui reconnait le même langage:
- Si $e=\varepsilon$, on prend $S\to\varepsilon$
- Si $e=a\in\Sigma$, on prend $S\to a$

- Si $e=e'|e''$ on prend $S\to S'|S''$
- là c'est plus compliqué...


---
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


