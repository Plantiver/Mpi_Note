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
\mathcal{P}_{2}\text{ décidable}\;&\implies\;\mathcal{P}_{1}\text{ décidable} \\
\mathcal{P}_{1}\text{ indécidable} \;& \implies\;\mathcal{P}_{2}\text{ indécidable}
\end{cases}
$$
<!-- basicblock-end -->

Toute les définitions sur la complexité, bon...

<!-- basicblock-start -->
Def. problème de la classe $\textbf{P}$::
$$
\exists<A>_{\mathcal{P}},\;|A(e)|=O(P(|e|)).
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsLy1Zgwo6ivGAxufSD95ym" -->
Def. réduction polynomiale d'un problème en un autre::
$$
(\mathcal{P_{1}},E_{1})\leq_{\textbf{P}}(\mathcal{P}_{2},E_{2})\iff \exists tr\in E_{2}^{E_{1}},\;\begin{cases}
e\in \mathcal{P_{1}}^{+}\iff tr(e)\in \mathcal{P}_{2}^{+} \\
tr\text{ calculable et polynômiale}
\end{cases}
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obs6mi5r1a2Sec5Hi3vYQ0ix" -->
Th. classe polynomiale par réduction::
$$
\mathcal{P}_{1}\leq_{\textbf{P}} \mathcal{P}_{2}\;\implies\;\begin{cases}
\mathcal{P}_{2}\in \textbf{P}\;&\implies\;\mathcal{P}_{1}\in\textbf{P} \\
\mathcal{P}_{1}\not\in \textbf{P} \;& \implies\;\mathcal{P}_{2}\not\in \textbf{P}
\end{cases}
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. problème de la classe $\textbf{NP}$::
$$
\exists C,\;\exists g\in \mathrm{Set}( \top,\bot )^{E\times C},\;\begin{cases}
e\in \mathcal{P}^{+}\iff \exists c\in C,\;\begin{cases}
|c|&=O(P(|e|)) \\
g(e,c)&=\top
\end{cases} \\
\mathcal{P}_{g}\in \textbf{P}
\end{cases}
$$
<!-- basicblock-end -->

Théorème d'inclusion de $\textbf{P}$ dans $\textbf{NP}$, je ne le mets pas par manque d'intérêt.

<!-- basicblock-start -->
Def. problème $\textbf{NP}$-dur::
$$
\forall \mathcal{P}'\in \textbf{NP},\;\mathcal{P}\leq_{\textbf{P}}\mathcal{P}'.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. problème $\textbf{NP}$-complet::
- $\mathcal{P}$ est $\textbf{NP}$-dur
- $\mathcal{P}\in \textbf{NP}$.
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. de Cook::
$$
\textbf{SAT}\in \textbf{NP}.
$$
<!-- basicblock-end -->

> [!note]- Démo FNC SAT dans NP
> ![[Info - Démo - FNC SAT dans NP]]

<!-- basicblock-start -->
Th. condition d'égalité $\textbf{P}=\textbf{NP}$::
$$
\exists \mathcal{P}\;\textbf{NP}\text{-complet},\;\mathcal{P}\in \textbf{P}.
$$
<!-- basicblock-end -->