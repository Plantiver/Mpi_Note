---
deck: math
---
<!-- basicblock-start oid="Obs2bj85bpGMtggr2c81a3YA" -->
Def. intégrale impropre::
$$
\int_{[a,b[}f(t)\mathrm{d}t.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. convergence d'une intégrale impropre::
$$
\int_{[a;b[}f(t)\mathrm{d}t\text{ CV}\iff \lim_{ x \to b }\int_{[a;x[}f(t) \mathrm{d}t \text{ CV}.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obs8lcGlWTKfwWkCj0RImxiE" -->
Th. caractérisation de la convergence d'une intégrale impropre::
$$
\int_{[a,b[}f(t)\mathrm{d}t\text{ CV}\iff \exists M,\;\forall x \in[a,b[,\;\int_{[a,x]}f(t)\mathrm{d}t\leq M
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obsh5PC36GzD5xppnCwKTjWZ" -->
Def. fonction absolument convergente::
$$
\int_{I}|f(t)|\mathrm{d}t\text{ CV}
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. espace de Lebesgue::
$$
\mathcal{L}^{p}=\mathrm{Set}\left(  f,\;\|f\|_{p}\in[0;+\infty[  \right).
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObseVE4PeT6PBZfQxru4c1XR" -->
Th. convergence usuelle::
- $\ln \in \mathcal{L}^{1}(]0,1])$
- $(t\to e^{-at})\in \mathcal{L}^{1}([0,+\infty[)\iff a>0$
- $\left( t\to \frac{1}{t^{a}} \right)\in \mathcal{L}^{1}([1,+\infty])\iff a>1$
- $\left( t\to\frac{1}{t^{a}} \right)\in \mathcal{L}^{1}(]0,1])\iff a<1$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsIsswKymPdv3KerUayQ6T6" -->
Def. nature d'une intégrale::
- Convergente
- Divergente
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsL9AKIpmuUrgRzioh191Hp" -->
Th. intégrale tronqué::
$$
\int_{[a,b[}f(t)\mathrm{d}t\simeq \int_{[c>a,b[}f(t)\mathrm{d}t.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsEdBnZ3SHkjy6qVUor51kt" -->
Prop. condition de changement de variable::
- $\mathcal{C}^{1}$
- $\leftrightsquigarrow$
- $\nearrow\nearrow$ ou $\searrow\searrow$.
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. convergence de fonctions positives::
- si $f=O(g)$, alors $\begin{cases}\int_{a}^{b}g\text{ CV}&\;\implies\;\int_{a}^{b}f\text{ CV} \\  \int_{a}^{b}f\text{ DV}&\;\implies\;\int_{a}^{b}g\text{ DV}\end{cases}$
- si $f\sim_{b} g$, alors $\int_{a}^{b}f\simeq \int_{a}^{b}g$.
<!-- basicblock-end -->

Bon, le théorème qui dis que ACV implique CV, c'est évident pour les espaces dans lesquelles on travaille (complet), mais cette notion est hors programme, donc autant laisser les gens assumez que c'est vrai partout.

<!-- basicblock-start -->
Th. ipp d'intégrale impropre::
- licite ssi tout converge
- nature/valeur inchangées.
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. intégration des relations de comparaison::
$$
\begin{cases}
g\geq 0 \\
f=\mathscr{R}(g)
\end{cases}\;\implies\;\begin{cases}
\int_{a}^{b}g\text{ CV}\;\implies\;\int_{x}^{b}f=\mathscr{R}\left( \int_{x}^{b}g \right) \\
\int_{a}^{b}g\text{ DV}\;\implies\;\int_{a}^{x}f=\mathscr{R}\left( \int_{a}^{x}g \right)
\end{cases}
$$
<!-- basicblock-end -->