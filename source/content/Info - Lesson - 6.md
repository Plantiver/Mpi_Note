---
deck: info
---
# Calculabilité

<!-- basicblock-start oid="ObstHkJl8YnP2v0ETbiFZMWG" -->
Def. problème algorithmique::
$$
\mathcal{P}\subset E\times S
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obs6v0po7rU22fVT14neSMDJ" -->
Def. problème de décision::
$$
\mathcal{P}\in \mathrm{Set}( \top,\bot )^{E}.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsWm5fwZlCXVD3eMxzGJmxK" -->
Def. instance positive d'un problème de décision::
$$
\mathcal{P}^{+}=\mathrm{Set}( e \in E,\;\mathcal{P}(e)=\top)
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obs6ydimASmijOZVffO4C9sD" -->
Prop. problème d'optimisation::
$$
(\mathcal{P}_{c},\mathcal{P},c):\begin{cases}
\mathcal{P}_{c}\subset\mathcal{P}\subset E\times S \\
c:S\to \mathbb{R}_{+} \\
\forall (e,s)\in \mathcal{P}_{c},\;\forall(e',s')\in \mathcal{P},\;(e=e'\;\implies\;c(s)\leq c(s'))
\end{cases}
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsDomYQIUt9QHTEn1DypqvV" -->
Meth. transformer un problème d'optimisation en problème de décision::
$$
(\mathcal{P}_{c},\mathcal{P},c)\to \mathcal{P}'=\mathrm{Set}( ((e,k),s)\in(E\times \mathbb{R}_{+})\times S,\;(e,s)\in \mathcal{P},\;c(s)\leq k).
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsCH4zUQZL18k74qjfqMHD7" -->
Def. fonction calculable::
$$
\exists <A>,\;\forall e\in E,\;\begin{cases}
A(e)\text{ termine} \\
A(e)=f(e)
\end{cases}
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obsx7BlW5yjtaIsYp6WkUaWY" -->
Def. problème décidable::
$$
\exists<A>,\;\forall e\in E,\;\begin{cases}
A(e)\text{ termine} \\
A(e)=\top \iff e\in \mathcal{P}^{+}
\end{cases}
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsAc3x56lfx00VEVPccFrND" -->
Def. machine universelle::
$$
\mathcal{M}_{u}(<A>,e)=A(e).
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsmP59bzTQqIkmSKSMesg7a" -->
Def. problème de l'arrêt::
- Entrée: le code source d'un algorithme $A$, une entrée $e$ de $A$.
-  Sortie: vrai si l'appel $A(e)$ termine, faux sinon.
<!-- basicblock-end -->

> [!note]- Démo problème de l'arrêt
> ![[Info - Démo - Problème de l'arrêt]]

<!-- basicblock-start oid="ObsLy1Zgwo6ivGAxufSD95ym" -->
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

<!-- basicblock-start oid="Obs6mi5r1a2Sec5Hi3vYQ0ix" -->
Th. décidabilité par réduction::
$$
\mathcal{P}_{1}\leq \mathcal{P}_{2}\;\implies\;\begin{cases}

\end{cases}
$$
<!-- basicblock-end -->

