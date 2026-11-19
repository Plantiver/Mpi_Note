---
deck: info
---
# Calculabilité

<!-- basicblock-start -->
Def. problème algorithmique::
$$
\mathcal{P}\subset E\times S
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. problème de décision::
$$
\mathcal{P}\in \mathrm{Set}( \top,\bot )^{E}.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. instance positive d'un problème de décision::
$$
\mathcal{P}^{+}=\mathrm{Set}( e \in E,\;\mathcal{P}(e)=\top)
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. problème d'optimisation::
$$
(\mathcal{P}_{c},\mathcal{P},c):\begin{cases}
\mathcal{P}_{c}\subset\mathcal{P}\subset E\times S \\
c:S\to \mathbb{R}_{+} \\
\forall (e,s)\in \mathcal{P}_{c},\;\forall(e',s')\in \mathcal{P},\;(e=e'\;\implies\;c(s)\leq c(s'))
\end{cases}
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Meth. transformer un problème d'optimisation en problème de décision::
$$
(\mathcal{P}_{c},\mathcal{P},c)\to \mathcal{P}'=\mathrm{Set}( ((e,k),s)\in(E\times \mathbb{R}_{+})\times S,\;(e,s)\in \mathcal{P},\;c(s)\leq k).
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. fonction calculable::
$$
\exists <A>,\;\forall e\in E,\;\begin{cases}
A(e)\text{ termine} \\
A(e)=f(e)
\end{cases}
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. problème décidable::
$$
\exists<A>,\;\forall e\in E,\;\begin{cases}
A(e)\text{ termine} \\
A(e)=\top \iff e\in \mathcal{P}^{+}
\end{cases}
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. machine universelle::
$$
\mathcal{M}_{u}(<A>,e)=A(e).
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. problème de l'arrêt::
- Entrée: le code source d'un algorithme $A$, une entrée $e$ de $A$.
-  Sortie: vrai si l'appel $A(e)$ termine, faux sinon.
<!-- basicblock-end -->

> [!note]- Démo problème de l'arrêt
> ![[Info - Démo - Problème de l'arrêt]]

<!-- basicblock-start -->
Def. réduction d'un problème en un autre::
$$
(\mathcal{P_{1}},E_{1})\leq(\mathcal{P}_{2},E_{2})\iff \exists tr\in E_{2}^{E_{1}},\;\begin{cases}
e\in \mathcal{P_{1}}^{+}\iff tr(e)\in \mathcal{P}_{2}^{+} \\
tr\text{ calculable}
\end{cases}
$$
<!-- basicblock-end -->

> [!note]- Méthode de réduction
> ![[Info - Meth - Réduction d'un algorithme en un autre]]

<!-- basicblock-start -->
Th. décidabilité par réduction::
$$
\mathcal{P}_{1}\leq \mathcal{P}_{2}\;\implies\;\begin{cases}

\end{cases}
$$
<!-- basicblock-end -->

