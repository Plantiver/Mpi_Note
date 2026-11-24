---
deck: math
---

<!-- basicblock-start -->
Def. colinéaire::
$$
x=0\text{ ou }y=\lambda x.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. produit scalaire::
- $<x;y>$:
- Symétrique: $<x;y>=<y;x>$
- Bilinéaire: ...
- Positive: $<x;x> \geq0$
- Définie: $<x;x> =0\;\implies\;x=0$.
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. norme associée à un produit scalaire::
$$
\|\cdot\|:x\to \sqrt{ <x;x> }.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. espace préhilbertien::
$$
(E,<\cdot;\cdot>).
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. espace euclidien::
$$
(E,<\cdot;\cdot>),\;\mathrm{dim}E<+\infty.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. Cauchy-Schwartz::
$$
|<x;y>|\leq\|x\|\cdot\|y\|.
$$
<!-- basicblock-end -->

> [!note]- Démo Cauchy-Schwartz
> ![[Math - Démo - Inégalité de Cauchy-Schwartz]]

<!-- basicblock-start -->
Prop. égalité de Minkowski::
$$
\|x+y\|=\|x\|+\|y\|\iff \exists\lambda \in \mathbb{R}_{+},\;x=\lambda y\text{ ou }y=\lambda x.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. produit scalaire usuels::
- $<X;Y>=X^{T}Y$
- $<A;B>=\mathrm{Tr}(A^{T}B)$
- $<f;g>=\int_{a}^{b}fg$.
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. Cauchy-Schwartz du produit scalaire des fonctions continues::
$$
|\int_{a}^{b}fg|\leq \sqrt{ \int_{a}^{b}f^{2} }\cdot \sqrt{ \int_{a}^{b}g^{2} }.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. famille orthogonale::
$$
\forall (e_{i},e_{j})\in \mathscr{F}^{2},\;i\not=j\;\implies\;<e_{i};e_{j}> =0.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. famille orthonormé::
$$
\forall(e_{i},e_{j})\in \mathscr{F}^{2},\;<e_{i};e_{j}> =\delta_{i}^{j}.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. famille orthonormé sans vecteurs nul::
$$
\mathscr{F}\text{ est libre}.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. Pythagore pour une famille orthogonale::
$$
\|\sum_{i=1}^{n}e_{i}\|^{2}=\sum_{i=1}^{n}\|e_{i}\|^{2}.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. Riesz::
$$
\exists!a\in E,\;f=(x\to<x;a>).
$$
<!-- basicblock-end -->

Th. Interprétation matricielle du ps en BON... Flemme #todo parce qu'important apperement.

<!-- basicblock-start -->
Def. ensembles orthogonaux::
$$
X\bot Y\iff \forall(x,y)\in X\times Y,\;<x;y>=0.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. orthogonal d'un ensemble::
$$
X^{\bot}=\mathrm{Set}( y\in E,\;\forall x \in X,\;<x;y>=0 ).
$$
<!-- basicblock-end -->






