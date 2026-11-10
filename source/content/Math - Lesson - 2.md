---
deck: math
---
<!-- basicblock-start oid="ObsVKcLtvlrO4Xz6VLk1Jnhk" -->
Def. espace vectoriel::
- $(E,+,\cdot)$ est un $\mathbb{K}$-EV ssi
- $(E,+)$ est un groupe abélien
- $\cdot$ est distributive sur $+$
- Le produit de $\mathbb{K}$ est compatible avec $\cdot$
- $\forall e\in E,\;1\cdot e=e$.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObslljoNKxihYjN6TnPeC63s" -->
Def. famille libre::
$$
\forall(\lambda_{i})\in \mathbb{K}^{n},\;\sum_{k=1}^{n}\lambda_{k}f_{k}=0\;\implies\;(\lambda_{i})=0.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsuRtkMUICClIsOVKamV1YB" -->
Def. famille génératrice::
$$
\forall e\in E,\;\exists(\lambda_{i})\in \mathbb{K}^{n},\;\sum_{k=1}^{n}\lambda_{k}f_{k}=e.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsLqN4HzZoLiw7dr3uBmHG9" -->
Def. dimension d'un espace vectoriel::
- Nombre d'élément de l'une de ses bases.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObslxJkAMfETk8EzbIIQoUkA" -->
Prop. tailles des familles d'un espace vectoriel::
- Si $\mathscr{F}$ est génératrice, $\# \mathscr{F}\geq \mathrm{dim}E$
- Si $\mathscr{F}$ est libre, $\# \mathscr{F}\leq\mathrm{dim}E$.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsetftanUULWderRSEYI32Q" -->
Def. rang d'une famille::
$$
\mathrm{rg}\mathscr{F}=\mathrm{dim}\mathrm{Vect}(\mathscr{F}).
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obs0DeLF5XOQsX9ZRrpaGM3M" -->
Prop. estimation du rang d'une famille::
- $\mathrm{rg}\mathscr{F}\leq \mathrm{dim}E$, avec égalité ssi $\mathscr{F}$ est génératrice
- $\mathrm{rg}\mathscr{F}\leq\#\mathscr{F}$, avec égalité ssi $\mathscr{F}$ est libre.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsTCGBKsUPhxj0OHerQ5MKj" -->
Th. de la base incomplète::
- Toute famille libre peut être complétée en une base
- De toute famille génératrice peut être extraite une base.
<!-- basicblock-end -->

prop. dim d'un produit d'espace vectoriel::
$$
\mathrm{dim}E\times F=\mathrm{dim}E+\mathrm{dim}F.
$$

<!-- basicblock-start oid="ObslhuIs8G6zAPel5Oi4NjE7" -->
Prop. matrice d'une application linéaire dans une base::
$$
\mathcal{Mat}_{\mathscr{B},\mathscr{B}'}(u)=\left( u(\mathscr{B}_{1}) \;\middle|\; \vdots \;\middle|\;u(\mathscr{B}_{n}) \right) .
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. sous-espace vectoriel::
- $0\in F\subset E$
- $\forall(x,y,\lambda,\mu)\in F^{2}\times \mathbb{K}^{2},\;\lambda x+\mu y\in F$.
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. caractérisation des sommes directes::
- $\forall(e_{i})\in \prod E_{i},\;\sum e_{i}=0\;\implies\;(e_{i})=0$
- $\mathrm{dim}\left( \sum E_{i} \right)=\sum\mathrm{dim}(E_{i})$ en dimension finie
- $E_{1}\cap E_{2}=\mathrm{Set}( 0 )$ en dimension 2.
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. espace supplémentaire::
$$
E=\bigoplus E_{i}.
$$
<!-- basicblock-end -->















