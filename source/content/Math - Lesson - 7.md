---
deck: math
---

<!-- basicblock-start oid="ObstVfN4mo70B831cVmtxUvF" -->
Def. critère générale d'une limite::
$$
(f(x)\underset{ x\to x_{0} }{ \to }l)\iff\left[\forall \mathcal{V}_{l},\;\exists \mathcal{V}_{x_{0}},\;\forall x \in D,\;(x \in \mathcal{V}_{x_{0}}\;\implies\;f(x)\in \mathcal{V}_{l})\right].
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsNgzQhyOQ3Zmo5ptch8QIt" -->
Def. fonction continue en un point::
$$
f\in \mathcal{C}^{0}_{x_{0}}(D,A)\iff \forall(u_{n})\in D^{\mathbb{N}},\;u_{n}\underset{ n }{ \to }x_{0}\;\implies\;f(u_{n})\underset{ n }{ \to }f(x_{0}).
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObseFjgY3jSe0SdBMQWYTdYC" -->
Def. fonction lipshitziannité::
$$
\exists k\in \mathbb{R}_{+},\; \forall(x,y)\in E^{2},\;\|f(x)-f(y)\|_{F}\leq k\|x-y\|_{E}.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obs4Of860nHRNlQjla4hLlaE" -->
Th. critère de continuité d'application linéaire::
$$
\exists k\in R^{+},\;\forall x \in E,\;\|u(x)\|_{F}\leq k\cdot\|x\|_{E}.
$$
<!-- basicblock-end -->

#todo finish this one
<!-- basicblock-start oid="Obs3CYoS8T0oPEj5eT2wpPTP" -->
Th. continuité d'application linéaire en dimension finie::
$$
\mathcal{L}_{c}(E,F)=\mathcal{L}(E,F).
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obsgmaai35BVboTgjhrWbqgf" -->
Th. CS de continuité d'une application::
- Lipschitzienne
- Les composantes sont polynomiales en les coordonnées.
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. propriété vraie à un voisinage::
$$
\exists \mathcal{V},\;P(\mathcal{V})\text{ est vraie}.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. conséquence de limite finie en un point::
$$
f(x)\underset{ x\to a }{ \to } l\;\implies\;\exists \mathcal{V},\;\forall x \in \mathcal{V},\;\exists M,\;|f(x)|\leq M.
$$
<!-- basicblock-end -->

Plein de choses sur les équivalents... ça ne sert à rien évidement (faux, le ds va me détruire)

<!-- basicblock-start -->
Th. caractérisation topologique des applications continue::
$$
\forall U\in \mathscr{U}(F),\;f^{-1}(U)\in \mathscr{U}(E).
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. chemin d'un ensemble::
$$
\gamma:[a,b]\to X\in \mathcal{C}^{0}.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. composantes fortement connexes::
$$
C\subset X,\;\forall(a,b)\in C,\;\exists\gamma \in C^{[0;1]},\;\begin{cases}
\gamma (0)&=a \\
\gamma(1)&=b
\end{cases}
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. ensemble connexe par arc::
$$
\forall(a,b)\in X,\;\exists\gamma \in C^{[0;1]},\;\begin{cases}
\gamma(0)&=a \\
\gamma(1)&=b
\end{cases}
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. ensemble CPA usuels::
- les ensembles convexes
- les ensembles étoilés.
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. image par une fonction continue::
- CPA
- intervalle
- compact.
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. TVI::
$$
\begin{cases}
f\in \mathcal{C}^{0}(I,\mathbb{R}) \\
I=[a,b]
\end{cases}\;\implies\;\forall y\in[f(a);f(b)],\;\exists x \in[a;b],\;f(x)=y.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. des bornes::
- Toute fonction continue sur un compact est bornée et atteint ses bornes.
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. fonction multilinéaire::
$$
\forall i\in[1,n],\;f(x_{1},\dots,x_{i-1},\cdot,x_{i+1},\dots,x_{n})\in \mathcal{L}(E,F).
$$
<!-- basicblock-end -->


















<!-- basicblock-start oid="ObsRwqwvCqnHgDU2yjtY37un" -->
Form. de Stirling::
$$
n! \sim \sqrt{ 2\pi n }\left( \frac{n}{e} \right)^{n}.
$$
<!-- basicblock-end -->

