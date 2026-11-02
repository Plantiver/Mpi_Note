# Problème 1
## Partie I

### Q1.
$$
C_{t}=\begin{pmatrix}
0 & 1 \\
t & 0
\end{pmatrix},\;C_{t}^{2}=\begin{pmatrix}
t & 0 \\
0 & t
\end{pmatrix}
$$
Ainsi, $P=X^{2}-t$ est un polynôme annulateur de $C_{t}$.

---
### Q2.
Supposons $t>0$, alors:
$$
\begin{align*}
\chi_{A_{t}}&=X^{2}-X+\frac{1-t}{4}&&\cr
&=\left( X-\frac{1+\sqrt{ t }}{2} \right)\left( X-\frac{1-\sqrt{ t }}{2} \right)&&\cr
\end{align*}
$$
est un polynôme scindé à racine simple, donc les valeurs propres de $A_{t}$ en sont les racines.
Et donc:
$$
\mathrm{Sp}A_{t}=\mathrm{Set}\left(  \frac{1\pm \sqrt{ t }}{2}  \right).
$$

Alors,
$$
\begin{cases}
E_{\frac{1+\sqrt{ t }}{2}}(A_{t})&=\mathrm{Ker}\begin{pmatrix}
-\sqrt{ t } & 1 \\
t & -\sqrt{ t }
\end{pmatrix} &= \mathrm{Vect}(v_{1}=\begin{pmatrix}
1 \\
\sqrt{ t }
\end{pmatrix}) \\
E_{\frac{1-\sqrt{ t }}{2}}(A_{t})&=\mathrm{Ker}\begin{pmatrix}
\sqrt{ t } & 1 \\
t & \sqrt{ t }
\end{pmatrix}&=\mathrm{Vect}(v_{2}=\begin{pmatrix}
1 \\
-\sqrt{ t }
\end{pmatrix})
\end{cases}
$$
Or $\begin{vmatrix}1 & 1\cr\sqrt{ t } & -\sqrt{ t }\end{vmatrix}=-2\sqrt{ t }\not=0$, donc $\mathscr{B}=(v_{1},v_{2})$ est une base propre et
$$
\begin{cases}
A_{t}&=PDP^{-1} \\ \\
D&=\begin{pmatrix}
\frac{1+\sqrt{ t }}{2} & 0 \\
0 & \frac{1-\sqrt{ t }}{2}
\end{pmatrix} \\
P&=\begin{pmatrix}
1 & 1 \\
\sqrt{ t } & -\sqrt{ t }
\end{pmatrix}
\end{cases}
$$

---
### Q3.
Supposons $t<0$:
$$
\begin{align*}
\chi_{A_{t}}&=X^{2}-X+\frac{1-t}{4}&&\cr
&=\left( X-\frac{1+i\sqrt{ -t }}{2} \right)\left( X-\frac{1-i\sqrt{ -t }}{2} \right)&&\cr
\end{align*}
$$
De même que pour Q2.:
$$
\begin{cases}
E_{\frac{1+i\sqrt{ -t }}{2}}(A_{t})&=\mathrm{Ker}\begin{pmatrix}
-i\sqrt{ -t } & 1 \\
t & -i\sqrt{ -t }
\end{pmatrix}&=\mathrm{Vect}(\bar{v_{1}}=\begin{pmatrix}
1 \\
i\sqrt{ -t }
\end{pmatrix}) \\
E_{\frac{1-i\sqrt{ -t }}{2}}(A_{t})&=\mathrm{Ker}\begin{pmatrix}
i\sqrt{ -t } & 1 \\
t & i\sqrt{ -t }
\end{pmatrix}&=\mathrm{Vect}(\bar{v_{2}}=\begin{pmatrix}
1 \\
-i\sqrt{ -t }
\end{pmatrix})
\end{cases}
$$
Et donc, avec $\mathscr{\bar{B}}=(\bar{v_{1}},\bar{v_{2}})$ base propre:
$$
\begin{cases}
A_{t}&=PDP^{-1} \\
D&=\begin{pmatrix}
\frac{1+i\sqrt{ -t }}{2} & 0 \\
0 & \frac{1-i\sqrt{ -t }}{2}
\end{pmatrix} \\
P&=\begin{pmatrix}
1 & 1 \\
i\sqrt{ -t } & -i\sqrt{ -t }
\end{pmatrix}
\end{cases}
$$
Le polynôme caractéristique n'étant pas scindé sur $\mathbb{R}$, $A_{t}$ n'est pas trigonalisable sur $\mathbb{R}$.

---
### Q4.
$$
A_{0}=\frac{1}{2}\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$
Ainsi, $A_{0}$ est triangulaire supérieur, donc ses valeurs propres sont ses coefficients diagonaux.
$$
\mathrm{Sp}A_{0}=\mathrm{Set}\left(  \frac{1}{2}  \right).
$$
Et donc, si $A_{0}$ était diagonalisable, elle serait semblable à $\begin{pmatrix}\frac{1}{2} & 0\cr0 & \frac{1}{2}\end{pmatrix}$, donc égale à cette matrice, ce qui est absurde. Donc $A_{0}$ n'est pas diagonalisable, ni sur $\mathbb{R}$, ni sur $\mathbb{C}$.
En prenant $J=\begin{pmatrix}0 & 1\cr0 & 0\end{pmatrix}$, ça fonctionne.

Ainsi, sur $\mathbb{C}$, $A_{0}$ est diagonalisable pour $t\in \mathbb{R}^{\star}$, et triangulaire supérieur pour $t=0$.
Sur $\mathbb{R}$, $A_{0}$ est diagonalisable pour $t\in \mathbb{R}^{\star}_{+}$, n'est même pas trigonalisable pour $t\in \mathbb{R}^{\star}_{-}$, et est triangulaire supérieur pour $t=0$.

---
## Partie II
### Q5.
$$
\begin{align*}
A_{0}^{m}&=\left( \frac{1}{2}(I_{2}+J) \right)^{m}&&\cr
&=\frac{1}{2^{m}}\sum_{k=0}^{m}\binom{m}{k}J^{k}&&\cr
&=\frac{1}{2^{m}}(I_{2}+mJ)&&\cr
&\underset{ m }{ \to }0.&&\cr
\end{align*}
$$
Car $I_{2}$ et $J$ commutent.

---
## Partie III
# Problème 2

## Partie I

## Partie II

## Partie III

### Q24.
Tout élément de $\mathscr{P}$ a pour polynôme annulateur $P=X^{2}-X=X(X-1)$ qui est scindé à racine simple, donc est diagonalisable et a son spectre inclus dans $\mathrm{Set}( 0,1 )$.
Ainsi, $\forall P\in \mathscr{P},\;\mathrm{Tr}P\in \mathrm{Set}( 0,1,2 )$.

Introduisons $\phi:\begin{cases}\mathcal{M}_{2}(\mathbb{R})\to \mathbb{R}_{+}\cr M\to\|M^{2}-M\|\end{cases}$, est continue, alors $\mathscr{P}=\phi ^{-1}(\mathrm{Set}( 0 ))$, l'image réciproque d'un ensemble fermé par une application continue, donc un fermé.

---
### Q25.
$$
\forall s \in \mathbb{R},\;P_{s}^{2}=P_{s}\;\implies\;\forall s\in \mathbb{R},\;P_{s}\in \mathscr{P}.
$$
Or,
$$
\forall s\in \mathbb{R},\;\|P_{s}\|=1+|s|.
$$
Ainsi, $\mathscr{P}$ n'est pas borné.
Or, tout compact est bornée, donc $\mathscr{P}$ n'est pas un compact.

---
### Q26.
Soit $r\geq0$, alors:
- $\mathscr{P}_{r}$ est borné par définition
- $\mathscr{P}_{r}$ est un fermé car l'intersection de $\mathscr{P}$ et $\|\cdot\|^{-1}([-r, r])$, deux fermés.
Or, nous sommes en dimension finie, donc ces hypothèses suffisent: $\mathscr{P}_{r}$ est compact.

---
### Q27.
Soit $\psi:\begin{cases}\mathcal{M}_{2}(\mathbb{R})&\to \mathcal{M}_{2}(\mathbb{R})\cr M&\to M^{T}-M\end{cases}$.
Alors, $S=\mathscr{P}\cap \psi ^{-1}(\mathrm{Set}(0_{\mathcal{M}_{2}(\mathbb{R})}))$, est un fermé par intersection de fermé.

Soit
$$
s=\begin{pmatrix}
a & b \\
b & d
\end{pmatrix}\in S.
$$
Alors,
$$
S^{2}=S\;\implies\;\begin{pmatrix}
a^{2}+b^{2} & ab+bd \\
ab+bd & b^{2}+d^{2}
\end{pmatrix}=\begin{pmatrix}
a & b \\
b & d
\end{pmatrix}.
$$
- **Si $b\not=0$:**
On a $a+d=1$, donc $a^{2}+2ad+d^{2}=1=a^{2}+2b^{2}+d^{2}$, donc $ad=b^{2}$.
Ainsi:$\begin{cases}d=1-a\cr b=\pm\sqrt{ a(1-a) }\end{cases}$, et $a\in[0,1]$.
Ainsi, $s=\begin{pmatrix}a & \pm \sqrt{ a(1-a) } \\  \pm \sqrt{ a(1-a) } & 1-a\end{pmatrix}$, et $\|s\|\leq2$.
- **Si $b=0$:**
alors $(a,d)\in \mathrm{Set}( 0,1 )^{2}$, donc $\|s\|\leq1$.

Ainsi, $S$ est borné et fermé en dimension finie, donc $S$ est compact.

---














