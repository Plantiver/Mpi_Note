# Exo 1
### a)
On observe que
$$
A\in S_{n}(\mathbb{R}).
$$
Donc, par le théorème spectrale:
$$
\exists P,D\in \mathcal{GL}_{2n}(\mathbb{R})\times\mathrm{diag}(\mathbb{R}^{2n}),\; A=PDP^{-1}.
$$
### b)
De même que pour a), $M_{\lambda}$ est diagonalisable.

### c)
###### (i)
Par hypothèse, on a:
$$
\forall i\in[1,n] \begin{cases}
u(e_{i})&=\lambda_{i}e_{i}+\lambda_{i}^{2}e_{i+n} \\
u(e_{i+n})&=\lambda_{i}^{2}e_{i}-\lambda_{i}e_{i+n}
\end{cases}
$$
Ainsi, dans la base $B'$:
$$
B=\mathcal{Mat}_{B'}(u) = \begin{pmatrix}
M_{\lambda_{1}}&&(0) \\
&\ddots& \\
(0) & & M_{\lambda_{n}}
\end{pmatrix}.
$$
###### (ii)
D'après b), $M_{\lambda}$ est diagonalisable, notons:
$$
M_{\lambda}=P_{\lambda}D_{\lambda}P_{\lambda}^{-1}.
$$
Ainsi, on introduit:
$$
\begin{cases}
\tilde{P}=\mathrm{diag}((P_{\lambda_{i}})_{i\in[1,n]}) \\
\tilde{D}=\mathrm{diag}((D_{\lambda_{i}})_{i\in[1,n]}).
\end{cases}
$$
On vérifie que:
$$
\mathrm{diag}((P_{\lambda_{i}^{-1}})_{i\in[1,n]})\times \tilde{P}=I_{2n}.
$$
D'où:
$$
B=\tilde{P}\tilde{D}\tilde{P}^{-1}
$$
Or $\tilde{D}$ est diagonale, donc:
$$
\mathrm{Sp}B = \bigcup_{i\in[1,n]}\mathrm{Sp}M_{\lambda_{i}}=\mathrm{Set}( \pm\lambda_{i}\sqrt{ 1+\lambda_{i}^{2} },\;i\in[1,n] ).
$$
Or $B$ est la matrice de l'endomorphisme canoniquement associé à $A$ dans une autre base, donc $A\sim B$.
Et donc, $A$ est diagonalisable
Et $\mathrm{Sp}A=\mathrm{Sp}B$.

# Exo 2

On notera $\|\cdot\|$ sans distinction les différentes normes, pour une meilleur lisibilité.
### a)
Supposons par l'absurde que $A\not\in \mathcal{GL}_{n}(\mathbb{R})$.
Alors,
$$
\begin{align*}
\exists X\in \mathcal{M}_{n,1}(\mathbb{R})^{\star},\quad&&&\cr
0&=AX&&\cr
X&=-CX&&\cr
\|X\|&=\|CX\|&&\cr
\|X\|&\leq\|C\|\cdot\|X\|&&\cr
1&\leq\|C\|.&&\cr
\end{align*}
$$
Absurde, contredis l'hypothèse de départ.

Ainsi, $\boxed{A\in \mathcal{GL}_{n}(\mathbb{R})}$.

### b)
Soit $\lambda \in \mathrm{Sp}C$.
Alors:
$$
\exists X\in \mathcal{M}_{n,1}(\mathbb{R})^{\star},\;CX=\lambda X.
$$
Ainsi, en composant par les normes:
$$
\begin{align*}
\|CX\|&=\|\lambda X\|&&\cr
\|C\|\cdot\|X\|&\geq|\lambda|\cdot\|X\|&&\cr
\|C\|&\geq|\lambda|.&&\cr
\end{align*}
$$
D'où:
$$
\boxed{|\lambda|<1}.
$$
### c)
$$
\begin{align*}
AX&=Y&&\cr
\underset{A^{-1}\times\dots}{\implies\quad\quad}X&=A^{-1}Y.&&\cr
\end{align*}
$$
Par bijectivité de $A$, $(E)$ possède une unique solution:
$$
\boxed{X_{S}=A^{-1}Y}.
$$


### d)
Soit $X\in \mathcal{M}_{n,1}(\mathbb{R})$.
Alors,
$$
\begin{align*}
\|F(X)\|&=\|CX-Y\|&&\cr
&\leq\|CX\|+\|Y\|&&\cr
&\leq\|CX\|&&\cr
&\leq\|C\|\cdot\|X\|.&&\cr
\end{align*}
$$
Donc $F$ est $\|C\|$-lipschitzienne.
Ainsi, $F$ est continue.
Ainsi, si $X$ est solution de $(E)$, alors
$$
F(X)=Y-CX = Y-AX+X=X.
$$
Réciproquement, satisfaire $F(X)=X$ implique que $X$ est solution de $(E)$.

### e)
Soit $P(p):\|X_{p}-X_{s}\|\leq\|C\|^{p}\cdot\|X_{0}-X_{s}\|$.
Montrons $P(p)$ par récurrence avec $p \in \mathbb{N}$.
**Initialisation:** Trivialement $\|X_{0}-X_{s}\|\leq 1\cdot\|X_{0}-X_{s}\|$.
**Hérédité:** Supposons $P(p)$, montrons $P(p+1)$.
$$
\begin{align*}
CX_{p}-CX_{s}&=C(X_{p}-X_{s})&&\cr
CX_{p}-Y+X_{s}&=C(X_{p}-X_{s})&&\cr
-X_{p+1}+X_{s}&=C(X_{p}-X_{s})&&\cr
\|X_{p+1}-X_{s}\|&\leq\|C(X_{p}-X_{s})\|&&\cr
&\leq\|C\|\cdot\|X_{p}-X_{s}\|&&\cr
&\leq\|C\|^{p+1}\cdot\|X_{0}-X_{s}\|.&&\cr
\end{align*}
$$
Ainsi, la proposition est vraie par récurrence.

Ainsi, la suite des $(X_{p})_{p \in \mathbb{N}}$ converge vers $X_{s}$ (par $\|C\|<1$).
### f)
On a donc:
$$
\begin{align*}
\|X_{0}-X_{s}\|&=\|X_{0}-A^{-1}Y\|&&\cr
&\leq\|X_{0}\|+\|A^{-1}Y\|&&\cr
&\leq\|X_{0}\|+\|A^{-1}\|\cdot\|Y\|.&&\cr
\end{align*}
$$
CQFD.

### g)
Pour $p\geq10$, $\|X_{0}-X_{s}\|\leq \frac{1}{1024}$.

### h)
Par équivalence des normes en dimensions finies, 
Il existe $C\in \mathbb{R},\;\forall X\in \mathcal{M}_{n,1}(\mathbb{R}),\;\|X\|\leq C\mathcal{N}(X)$.
Alors $\gamma=C\mathcal{N}(X_{0})+C\|A^{-1}\|\cdot \mathcal{N}(Y)$ convient.




