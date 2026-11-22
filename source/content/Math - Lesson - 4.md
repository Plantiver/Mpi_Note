---
deck: math
---

<!-- basicblock-start oid="ObswXOcHnKazbNW6GiktrdzO" -->
Def. vecteur propre::
$$
\begin{cases}
\exists\lambda \in \mathbb{K},\;u(x)=\lambda x \\
\exists\lambda \in \mathbb{K},\;AX=\lambda X
\end{cases}
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObskxkDpg6ktHQtg1pzRHGeV" -->
Def. valeur propre::
$$
\begin{cases}
\exists x \in E^{\star},\;&u(x)=\lambda x \\
\exists X\in \mathcal{M}_{n,1}(\mathbb{K})^{\star},\;&AX=\lambda X
\end{cases}
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsOYlRhubnQn7KB4aJzzEo7" -->
Def. spectre d'un endomorphisme::
$$
\mathrm{Sp}u=\mathrm{Set}( \lambda \in \mathbb{K},\;\lambda\text{ valeur propre de u} ).
$$
<!-- basicblock-end -->

Théorème de diagonalisation 1.

<!-- basicblock-start oid="Obs5AjcIFelBxjSDP50Cv0kD" -->
Def. sous-espace propre associée à une valeur propre::
$$
\begin{cases}
E_{\lambda}(u)=\mathrm{Ker}(u-\lambda id) \\
E_{\lambda}(A)=\mathrm{Ker}(A-\lambda I_{n})
\end{cases}
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsaTzKFDv7kiLdc1k5zooRP" -->
Def. polynôme caractéristique::
$$
\begin{cases}
\chi_{u}=\det(Xid-u) \\
\chi_{A}=\det(XI_{n}-A)
\end{cases}
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsyK5dggszOAqO24BZ8IEUU" -->
Def. matrice diagonalisable::
$$
\exists (P,D)\in \mathcal{GL}_{n}(\mathbb{K})\times \mathcal{D}_{n}(\mathbb{K}),\;A=PDP^{-1}.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obsw9dmW1zX3KCldUgt3V7BU" -->
Th. spectrale 1/4::
$$
\mathcal{S}_{n}(\mathbb{R})\subset \mathcal{DZ}_{n}(\mathbb{K}).
$$
<!-- basicblock-end -->

Modification de la stabilité par commutativité pour inclure les SEP, voir [[Math - Lesson - 3]].

<!-- basicblock-start oid="Obs5DIdkVavHeNi0LSVKy7Y1" -->
Prop. particularité des SEP::
$$
\bigoplus_{\lambda \in \mathrm{Sp}u} E_{\lambda}(u).
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obs39KaHbOWKIxFevzHXOhwB" -->
Th. coefficient remarquable du polynôme caractéristique::
$$
\chi_{u}=X^{n}-\mathrm{tr}(u)X^{n-1}+\dots+(-1)^{n}\det(u).
$$
<!-- basicblock-end -->

Le théorème sur le polynôme d'un endomorphisme enduit

<!-- basicblock-start oid="Obsti0Vs8p8DTGnTNWdbB0C1" -->
Prop. dimension des SEP::
$$
1\leq \mathrm{dim}E_{\lambda}(u)\leq m(\lambda).
$$
<!-- basicblock-end -->
