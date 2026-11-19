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
### 14
Q1
Prenons $U_{i}=>^{\star}u_{i}$, alors
$$
S\to U_{i}Sa_{i}|\varepsilon.
$$
fonctionne. (FAUX, On n'accepte pas le mot vide)

Q2
Supposons $\mathcal{L}_{u}\cap \mathcal{L}_{v}\not=\emptyset$, soit $w$ un élément des deux.
Ainsi, $w=u_{i_{1}}\dots u_{i_{m}}a_{i_{m}}\dots a_{i_{1}}=v_{i_{1}'}\dots v_{i_{m}'}a_{i_{m}'}\dots a_{i_{1}}$. Alors, la séquence des $(u_{i_{1}},v_{i_{1}'}),\dots,(u_{i_{m}},u_{i_{m}'})$ fonctione.
De même, dans l'autre sens, une bonne séquence permet de former un élément dans l'intersection.

Q3
Prenons $\mathcal{L}_{u}$ associé à $\mathcal{L}(G_{1})$ et $\mathcal{L}_{v}$ associé à $\mathcal{L}(G_{2})$.
On a alors: $\mathcal{L}_{u}\cap \mathcal{L}_{v}=\emptyset \iff \mathcal{L}(G_{1})\cap \mathcal{L}(G_{2})=\emptyset$, par construction.
Ainsi, s'il existait un programme qui décidait de la non vacuité de l'intersection de la transformé des deux (calculable par l'existence de grammaire) des deux, on pourrait alors répondre au problème de Post. Donc, ce programme n'existe pas.

Q4
Soit $G_{1},G_{2}$ deux grammaires non-contextuelles non ambiguë, prenons $G$ tq
$$
S\to S_{1}|S_{2}.
$$
Alors, $G$ est ambiguë ssi $G_{1}\cap G_{2}\not=\emptyset$ ssi on peut construire avec $G_{1}\times G_{2}$ une instance positive du problème de Post.

Q5
De même, s'il y avait un programme qui répondrait à la question de l’ambiguïté d'une grammaire, alors, par la grammaire non-contextuelle précédente, on peut répondre au problème de la non-vacuité de l'intersection de ces grammaires.
Donc, ce programme n'existe pas.

Q6
Prenons
$$
\begin{align*}
S&\to \bigcup_{s\in\Sigma}\bigcup_{a\in A}MaMsM&&\cr
M&\to \bigcup_{s\in\Sigma}s|\bigcup_{a\in A}a|MM|\varepsilon.&&\cr
\end{align*}
$$
Q7
On a (en utilisant une syntaxe douteuse)
$$
\begin{align*}
S&\to &&\cr
B&\to LC&&\cr
C&\to c^{\star},\;c\in A&&\cr
L&\to l^{\star},\;l\in\Sigma&&\cr
\end{align*}
$$
Une horreur...

En fait, il s'agit du complémentaire du langage $\mathcal{L}_{u}$.

Q8
Bon, il suffit de regarder la question précédente.

Q9
$$
\begin{align*}
\mathcal{L}_{u}^{c}\cup \mathcal{L}_{v}^{c}\not=(\Sigma|A)^{\star}&\iff \mathcal{L}_{u}\cap \mathcal{L}_{v}\not=\emptyset &&\cr
&\iff \exists\text{ une instance positive du problème de Post}&&\cr
\end{align*}
$$
Par Q2

Q10
Bon, si un programme existait pour répondre à "cette grammaire engendre-t-elle tout les mots ?", alors on construisant l'union des complémentaire de $G_{1}$ et $G_{2}$, on peut répondre au problème de la non-vacuité de leur intersection. Donc ce programme n'existe pas.

Q11
Si un programme répond à "$\mathcal{L}(G_{1})=\mathcal{L}(G_{2})$", alors, en construisant la grammaire $G$ tq $\mathcal{L}(G)=\Sigma ^{\star}$, alors en vérifiant si le langage engendré par une grammaire et le même que celui engendré par $G$, alors on répond au problème de "cette grammaire engendre-t-elle tout les mots ?".

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

### 3
Prenons $\mathcal{P}_{1}$ le problème de l'arrêt, et $\mathcal{P}_{2}$ le problème proposé, et montrons que $\mathcal{P}_{1}\leq \mathcal{P}_{2}$.

Par l'absurde, notons $P_{2}$ un programme qui réponds à $\mathcal{P}_{2}$.

Introduisons
$$
tr:(<A>,e)\to (\mathcal{M}_{u},<()\to A(e);Vrai>).
$$
Alors
$$
\begin{align*}
(<A>,e)\in \mathcal{P}_{1}^{+}&\iff A(e)\text{ s'arrète}&&\cr
&\iff<()\to A(e);Vrai>\text{ s'arrète et renvoie }Vrai&&\cr
&\iff&&\cr
\end{align*}
$$







