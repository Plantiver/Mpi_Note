---
deck: math
---

<!-- basicblock-start oid="ObsLIBfgMQK2U7NUHwkwKkht" -->
Th. Localisation du spectre::
$$
P(A)=0\;\implies\;\mathrm{\mathrm{Sp} }_{\mathbb{K} }A\subset \mathrm{Rac}_{\mathbb{K} }(P).
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsxjoyfAU2QlJOGP7hw88IA" -->
Th. Cayley-Hamilton::
$$
\chi_{A}(A)=0.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsEaLqTrPdwaXReAlSwDwag" -->
Def. Polynôme minimal::
$$
\pi_{A}=\mathrm{min}_{|deg}(\mathrm{Set}( P\in \mathbb{K}[X],\;P(A)=0 ))
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. Base de $\mathbb{K}[U]$::
$$
\mathbb{K}[u] = \mathrm{Vect}\left[ (u^{k})_{k\in[0,\mathrm{deg}\pi_{u}-1]} \right].
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. Racine du polynôme minimal::
$$
\mathrm{Rac}_{\mathbb{K}}u=\mathrm{Sp}_{\mathbb{K}}u.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. Encadrement du polynôme minimal::
$$
\prod_{\mu \in \mathrm{Sp}u}(X-\mu)\;|\;\pi_{u}\;|\;\chi_{u}.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. Décomposition des noyaux::
$$
P=\prod P_{i},\;\forall i\not=j,\;P_{i}\wedge P_{j}=1 \;\implies\;\mathrm{Ker}P(u) = \bigoplus\mathrm{Ker}P_{i}(u). 
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. 5 CNS de DZ::
- $E=\bigoplus_{\mu \in \mathrm{Sp}u}E_{\mu}(u)$
- $\mathrm{dim}E=\sum_{\mu \in \mathrm{Sp}u}\mathrm{dim}E_{\mu}(u)$
- $\chi_{u}=\prod_{\mu \in \mathrm{Sp}u}(X-\mu)^{m_{\mu}}$ et $\forall \mu \in \mathrm{Sp}u,\;\mathrm{dim}E_{\mu}u=m_{\mu}$
- $\pi_{u}=\prod_{\mu \in \mathrm{Sp}u}(X-\mu)\in \mathbb{K}[X]$
- $\exists P\in \mathbb{K}[X],\;\begin{cases}P(u)=0\cr P=\prod(X-\lambda_{i}),\;(i\not=j\implies\lambda_{i}\not=\lambda_{j})\end{cases}$
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. DZ d'un induit::
- Soit $v$ induite de $u$
- $\pi_{v} | \pi_{u}$
- $u$ DZ $\;\implies\;v$ DZ.
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. TZ::
- u est TZ ssi $\exists B,\;\mathcal{Mat}_{B}(u)\in \mathcal{T}_{n}^{+}(\mathbb{K})$.
- $M$ TZ ssi $M\sim B\in \mathcal{T}_{n}^{+}(\mathbb{K})$.
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. 3 CNS de TZ::
- $\chi_{u}$ scindé sur $\mathbb{K}$
- $\pi_{u}$ scindé sur $\mathbb{K}$
- $\exists P\in \mathbb{K}[X],\;P(u)=0,\;P$ scindé sur $\mathbb{K}$.
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. TZ d'une matrice nilpotente::
$$
\exists n\in \mathbb{N},\;M^{n}=0\iff M\sim \begin{pmatrix}
0&&(\star)\cr
&\ddots& \cr
(0)&&0  
\end{pmatrix}
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
$$
\chi_{u}\text{ scindé}\iff \exists B,\;\mathcal{Mat}_{B}(u)=D+N,\;D=\mathrm{Diag}(\lambda _{i}), N^{n}=0.
$$
<!-- basicblock-end -->

#hp 
Def. Matrice de Jordan
Th. Réduction de Jordan
