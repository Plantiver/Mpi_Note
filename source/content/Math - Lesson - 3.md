---
deck: math
---
<!-- basicblock-start -->
Th. formule cœur (matrice)::
$$
[A\times B]_{i,j}=\sum_{k=1}^{p}[A]_{i,k}[B]_{k,j}.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. transposée d'une matrice::
$$
\cdot^{T}:M=(m_{i,j})\to(m_{j,i}).
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. transposée::
- $\cdot^{T}\in \mathcal{L}(\mathcal{M}_{n}(\mathbb{K}))$
- $(A\times B)^{T}=B^{T}\times A^{T}$
- $(\cdot^{T})^{2}=id$
- $\cdot^{T}\circ\cdot^{-1}=\cdot^{-1}\circ\cdot^{T}$
- Invariance de la trace, du rang, du déterminant, et du polynôme caractéristique par $\cdot^{T}$.
<!-- basicblock-end -->

Pratique
<!-- basicblock-start -->
Prop. produit de matrices élémentaires::
$$
E_{i,j}\times E_{k,l}=\delta_{j,k}E_{i,l}.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. matrices diagonales::
$$
\mathcal{D}_{n}(\mathbb{K})=\mathrm{Vect}((E_{i,i})).
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. matrices symétriques/antisymétriques::
- $\mathcal{S}_{n}(\mathbb{K})=\mathrm{Vect}((E_{i,j}+E_{j,i}))$
- $\mathcal{A}_{n}(\mathbb{K})=\mathrm{Vect}((E_{i,j}-E_{j,i}))$.
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. matrices triangulaires supérieurs::
$$
\mathcal{T}_{n}^{+}(\mathbb{K})=\mathrm{Vect}((E_{i,j})_{j\geq i}).
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. trace d'une matrice::
$$
\mathrm{Tr}A=\sum_{k=1}^{n}[A]_{k,k}
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. trace::
- $\mathrm{Tr}(AB)=\mathrm{Tr}(BA)$
- $\mathrm{Tr}p=\mathrm{rg}p$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. determinant d'une matrice::
$$
\det A=\sum_{\sigma \in \mathfrak{S}_{n}}\varepsilon(\sigma)\prod_{i=1}^{n}a_{i,\sigma(i)}
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. determinant d'une matrice::
- $\det(A\times B)=\det A\times \det B$
- $\det(\lambda\cdot A)=\lambda ^{n}\cdot\det A$
- forme $n$-linéaire alternée avec $\det I_{n}=1$
- $\det A=0\iff A\notin \mathcal{GL}_{n}(\mathbb{K})$.
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. déterminant d'une matrice diagonale par bloc::
$$
\det \begin{pmatrix}
A_{1} & * & \dots & * \\
0 & A_{2} & \ddots & \vdots \\
\vdots & \ddots & \ddots & * \\
0 & \dots & 0 & A_{p}
\end{pmatrix}=\prod_{k=1}^{p}\det A_{k}.
$$
<!-- basicblock-end -->

définition déterminant mineur, cofacteur, comatrice... (voir copain comme cochon).

<!-- basicblock-start -->
Th. développement suivant une colonne/ligne::
$$
\det A=\sum_{i=1}^{n}a_{i,j}\Delta_{i,j}.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. relation comaticre::
$$
A\times (\mathrm{comat}A)^{T}=(\det A)I_{n}.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. déterminant de Vandermonde::
$$
V(x_{1},\dots, x_{n})=\begin{vmatrix}
1 & x_{1} & \dots & x_{1}^{n-1} \\
\vdots & \vdots & \vdots & \vdots \\
1 & x_{n} & \dots & x_{n}^{n-1}
\end{vmatrix}=\prod_{1\leq i<j\leq n}(x_{j}-x_{i}).
$$
<!-- basicblock-end -->

Tout les trucs de définition de changement de base.

<!-- basicblock-start -->
Def. matrices semblables::
$$
A\sim B\iff \exists P\in \mathcal{GL}_{n}(\mathbb{K}),\;A=PBP^{-1}.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. matrices équivalentes::
$$
A\simeq B\iff \exists(P,Q)\in \mathcal{GL}_{n}(\mathbb{K})^{2},\;A=PBQ.
$$
<!-- basicblock-end -->

Théorème de caractérisation du rang, à savoir, mais bon, pas tant.

<!-- basicblock-start -->
Def. endomorphisme induit::
$$
u:\begin{cases}
F&\to &F \\
x&\to&u(x)
\end{cases},\;u(F)\subset F\subset E.
$$
<!-- basicblock-end -->

Rajout de la stabilité des espaces propres, par le chapitre 4.
<!-- basicblock-start -->
Th. stabilité déduite des applications commutantes::
$$
u\circ v=v\circ u\;\implies\;\begin{cases}
v(\mathrm{Ker}u)\subset\mathrm{Ker}u \\
v(\mathrm{Im}u)\subset\mathrm{Im}u \\
v(E_{\lambda}(u))\subset E_{\lambda}(u)
\end{cases}
$$
<!-- basicblock-end -->

Okay, on suppose que les théorèmes restant sont négligeable devant mon envie de dormir. Donc, par moi, je vais dodo.