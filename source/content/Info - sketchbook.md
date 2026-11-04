td
exo 1
1. 
u:(a,(ba(a)c))
2. 
Par induction, le seul cas avec un b est le deux, et sera toujours suivis d'un a
3. 
De même, par induction, et sur le deuxième cas encore
4. 
de même, par induction, et sur le deuxième cas encore
5. 
Par le lemme de l'étoile.
Supposons $\mathcal{L}(S)$ régulier, alors
Soit $N$ tq $\forall u,\;|u|\geq N,\;\exists xyz=u,\;|xy|< N,\;y\not=\varepsilon ,\;\mathcal{L}(xy^{\star}z)\subset \mathcal{L}(S)$.
Or, pour $S\;\underset{ S.2^{N},S.3 }{ \implies }^{\star}\;u=(ba)^{N}c^{N}$, on doit prendre $y=a^{\delta}(ba)^{k}b^{\sigma}$, et la dernière propriété n'est pas respecté.
Ainsi, $\mathcal{L}(S)$ n'est pas régulier.

exo 2
modification des règles:
$$
\begin{align*}
S&\to aSa|T&&\cr
T&\to bTb|U&&\cr
U&\to cUc|\varepsilon&&\cr
\end{align*}
$$
2. 
Par la règle de $S$, on a forcément un nombre pair de $a$.
3. 
$S\;\underset{ S.1^{n},S.2,T.1^{m},T.2,U.1^{k},U_{2} }{ \implies }^{\star}\;u=a^{n}b^{m}c^{2k}b^{m}a^{n}$.
On peut obtenir tout les mots, et tout les mots obtenus sont bons.
4. 
Voir exo1.5
Donc, il existe $N$ qui va bien.
mais pour $S\;\underset{ S_{1}^{N},S_{2},T_{1},T_{2},U_{2} }{ \implies }^{\star}u=a^{N}bba^{N}\;$.
Mais encore, $y=a^{k}$, et alors on contredis la propriété voulue.


exo 3
1. 
$$
\begin{align*}
S&\to S_{1}|S_{2}&&\cr
S_{1}&\to LK&&\cr
L&\to aLb|\varepsilon &&\cr
K&\to cK|\varepsilon &&\cr
S_{2}&\to L'K'&&\cr
L'&\to aL'|\varepsilon &&\cr
K'&\to bK'c|\varepsilon&&\cr
\end{align*}
$$

2. 3
$$
\begin{align*}
S&\to aSc|T&&\cr
T&\to bT|\varepsilon&&\cr
\end{align*}
$$
3. 6
$$
S\to aSa|bSb|cSc|\varepsilon
$$


exo 4
1. 
Par induction:
$$
\begin{align*}
S&\to S_{1}|S_{2}&&\cr
S&\to S_{1}S_{2}&&\cr
S&\to SS|\varepsilon&&\cr
\end{align*}
$$
2. 
Prenons:
$$
\begin{align*}
L_{1}&=\mathcal{L}(S_{1})&&\cr
L_{2}&=\mathcal{L}(S_{2})&&\cr
\end{align*}
$$
avec $S_{1}$ et $S_{2}$ définit dans exo3.1
Alors l'intersection est bien notre ensemble non algébrique


exo 5
$$
\begin{align*}
S&\to[L]&&\cr
L&\to1;L|1|\varepsilon&&\cr
\end{align*}
$$
exo 6
1. 
Supposons régulier, alors $\exists N$...
Prenons $u=(^{N})$, alors $y=(^{k}$, et on contredis la propriété voulue.
2. 
$$
\begin{align*}
S&\to S(S)|\varepsilon&&\cr
\end{align*}
$$
3. 
$$
S\to Sa_{1}Sb_{1}|\dots|Sa_{n}Sb_{n}
$$
exo 7
$$
\begin{align*}
S&\to &&\cr
P&\to E\times E&&\cr
&&&\cr
\end{align*}
$$










