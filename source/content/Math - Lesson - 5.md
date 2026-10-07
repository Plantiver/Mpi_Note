---
deck: math
---
<!-- basicblock-start oid="Obs2sdIh0iYtL9R4pCbxuX9k" -->
Def. Segment $[A,B]$::
$$
\mathrm{Set}( \lambda A+(1-\lambda)B,\;\lambda \in[0,1] ).
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsUncOt210Yt6sXIfqqan9i" -->
Def. Ensemble convexe::
$$
\forall x,y \in E,\;[x,y]\subset E.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsBSlVVv4VirJXfp4tWdvFo" -->
Def. $f:I\to \mathbb{R}$ convexe::
$$
\forall(\lambda,x,y)\in[0,1]\times I^{2},\;f(\lambda x+(1-\lambda)y)\leq \lambda f(x)+(1-\lambda)f(y)
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsJqYic1upb8Sp5RXO84ZD8" -->
Th. (Jensen) $f:I\to \mathbb{R}$ convexe::
$$
\phantom{`}(\lambda_{i})\text{ stochastiques}\;\implies\;f\left( \sum_{i=1}^{n}\lambda_{i}x_{i} \right)\leq \sum_{i=1}^{n}\lambda_{i}f(x_{i}).\phantom{`}
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsRFY85YA6MCp6Q349r5Skb" -->
Th. (Trois pentes) $f:I\to \mathbb{R}$ convexe::
$$
\forall(a,b,c)\in I^{3},\;(a<b<c)\;\implies\;\frac{f(b)-f(a)}{b-a}\leq \frac{f(c)-f(a)}{c-a}\leq \frac{f(c)-f(b)}{c-b}.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsKqcInk3Bq9Mvyc1qtlaTn" -->
Prop. Convexité de $f\in D^{2}(I,\mathbb{R})$::
- $f'$ croissante sur $I$
- $f''\geq0$ sur $I$.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsNWACrRa5x0o8DdzfkYT7m" -->
Prop. Fonctions usuelles et leur tangente::
- $e^{x}\geq 1+x$
- $\ln(1+x)\leq x$
- $|\sin(x)|\leq|x|$.
<!-- basicblock-end -->


<!-- basicblock-start -->
Def. Norme::
- $\|\cdot\|:E\to \mathbb{R}$
- $\forall (\lambda,x)\in \mathbb{K}\times E,\;\|\lambda x\|=|\lambda|\|x\|$
- $\|x\|=0\;\implies\;x=0_{E}$
- $\forall x \in E,\;\|x\|\geq 0$
- $\forall(x,y)\in E^{2},\;\|x+y\|\leq\|x\|+\|y\|$.
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. EVN::
$$
(E,+,\cdot,\|\cdot\|),\;\begin{cases}
(E,+,\cdot)\text{ est un }\mathbb{K}\text{-EV} \cr
\|\cdot\|\text{ est une norme sur }E.
\end{cases}
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. Distance associée à une norme::
$$
\forall(x,y)\in E^{2},\;\mathrm{d}(x,y)=\|x-y\|.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. Inégalité triangulaire sur les distances::
$$
\forall(x,y,z)\in E^{3},\;d(x,z)\leq d(x,y)+d(y,z).
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. Seconde inégalité triangulaire::
$$
\forall(x,y)\in E^{2},\;|\|x\|-\|y\||\leq\|x-y\|.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. Norme associée à un produit scalaire::
$$
\forall x \in E,\;\|x\|=\sqrt{ <x|x> }.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. Partie Bornée::
$$
\exists M\in \mathbb{R},\;\forall x \in X,\;\|x\|\leq M.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. Fonction bornée::
$$
\exists M\in \mathbb{R},\;\forall x \in X,\;\|f(x)\|\leq M.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. Ensemble des fonctions bornées::
$$
\mathscr{B}(X,E)=\mathrm{Set}( f\in \mathscr{F}(X,E),\;\exists M\in \mathbb{R},\;\|f\|\leq M ).
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. Boule fermée::
$$
\overline{B}(x,\varepsilon)=\mathrm{Set}( y\in E,\;\|x-y\|\leq\varepsilon ).
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. Boule ouverte::
$$
\dot{B}(x,\varepsilon)=\mathrm{Set}( y\in E,\;\|x-y\|<\varepsilon ).
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. Boules::
- Toujours convexe
- Toujours bornée
- Contient toujours une boule de l'autre type.
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. Normes usuelles::
- $\|\cdot\|_{1}: x\to \sum|x_{i}|$
- $\|\cdot\|_{2}: x\to \sqrt{\sum|x_{i}|}$
- $\|\cdot\|_{1}: x\to \sum|x_{i}|$
<!-- basicblock-end -->















