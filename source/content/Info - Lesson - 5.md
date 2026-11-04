---
deck: info
---
Exo 1.4
- $S\;\implies\; ST\;\implies\;SaS\;\implies\;Sa\;\implies\;a$
- $S\;\implies\;ST\;\implies\;STT\;\implies\;SbST\;\implies\;SbSbS\;\implies\;bSbS\;\implies\;bbS\;\implies\;bb$
- $S\;\implies\;ST\;\implies\;STT\;\implies\;STTT\;\implies\;STTTT\;\implies\;STTTTT\;\implies\;TTTTT\;\implies\;aSTTTT\;\implies\;aTTTT\;\implies\;aaSTTT\;\implies\;aaTTT\;\implies\;aaaSTT\;\implies\;aaaTT\;\implies\;aaaSbT\;\implies\;aaabT\;\implies\;aaabSb\;\implies\;aaabb$
- $S\;\implies\;ST\;\implies\;STT\;\implies\;SSbT\;\implies\;SSbaS\;\implies\;SbaS\;\implies\;baS\;\implies\;ba$



> [!note]- Démo langage régulier sont en fait non-contextuel
> ![[Info - Démo - Non-contextualité des langages réguliers]]

Exercice II.5 Construction d'une grammaire d'un langage de programmation
1. 
$$
\begin{align*}
N&\to NN&&\cr
&\to0&&\cr
&\to1&&\cr
\end{align*}
$$
2. 
$$
\begin{align*}
A&\to N&&\cr
&\to V&&\cr
&\to A\times A&&\cr
&\to A+A&&\cr
&\to(A)&&\cr
V&\to v_{1}|\dots|b_{n}&&\cr
\end{align*}
$$
3. 
$$
\begin{align*}
B&\to A=A&&\cr
&\to A\leq A&&\cr
&\to\neg B&&\cr
&\to B\vee B&&\cr
&\to B\wedge B&&\cr
\end{align*}
$$
4. 
$$
\begin{align*}
A&\to\{SA\}&&\cr
&\to \text{if }B\text{ then }A\text{ else }A&&\cr
S&\to V:=A;&&\cr
&\to\text{while }B\text{ do }S\text{ done};&&\cr
&\to skip;&&\cr
\end{align*}
$$
!! Différent de celui de la prof !!



# III
Dérivation à droite/gauche: on remplace directement l'élément le plus à droite/gauche.















# Nahhh
$N$ et $V$ voir plus haut.
On va définir $T,F,E,P$.
$$
\begin{align*}
T&\to \text{struct }TV\;\{tp\}&&\cr
tp&\to V:TV,tp&&\cr
&\to V:TV&&\cr
F&\to \text{fn }FV(tp)->TV \{E\}&&\cr
O&\to+|\times&&\cr
E&\to &&\cr
P&\to&&\cr
\end{align*}
$$



