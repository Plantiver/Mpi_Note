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


<!-- basicblock-start oid="ObsB0656x9MJxdHL1JjkjO4U" -->
Def. Norme::
- $\|\cdot\|:E\to \mathbb{R}$
- $\forall (\lambda,x)\in \mathbb{K}\times E,\;\|\lambda x\|=|\lambda|\|x\|$
- $\|x\|=0\;\implies\;x=0_{E}$
- $\forall x \in E,\;\|x\|\geq 0$
- $\forall(x,y)\in E^{2},\;\|x+y\|\leq\|x\|+\|y\|$.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsixZlxEFd4PBgWLiHMD8By" -->
Def. EVN::
$$
(E,+,\cdot,\|\cdot\|),\;\begin{cases}
(E,+,\cdot)\text{ est un }\mathbb{K}\text{-EV} \cr
\|\cdot\|\text{ est une norme sur }E.
\end{cases}
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsokbUBEwoNoTqP2QjJ9Lse" -->
Def. Distance associée à une norme::
$$
\forall(x,y)\in E^{2},\;\mathrm{d}(x,y)=\|x-y\|.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsXJDFkGDPSeD5FlodDqVMM" -->
Prop. Inégalité triangulaire sur les distances::
$$
\forall(x,y,z)\in E^{3},\;d(x,z)\leq d(x,y)+d(y,z).
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsY17NQu8gLTNBxPAaWX1I7" -->
Def. Seconde inégalité triangulaire::
$$
\forall(x,y)\in E^{2},\;|\|x\|-\|y\||\leq\|x-y\|.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsLmHZqUzHWpNeVmx9rIyzi" -->
Def. Norme associée à un produit scalaire::
$$
\forall x \in E,\;\|x\|=\sqrt{ <x|x> }.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obsu5YAyRNzHOcWuWK5QIAo2" -->
Def. Partie Bornée::
$$
\exists M\in \mathbb{R},\;\forall x \in X,\;\|x\|\leq M.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsHeKftOI6An390IqH8vMwk" -->
Def. Fonction bornée::
$$
\exists M\in \mathbb{R},\;\forall x \in X,\;\|f(x)\|\leq M.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsZBXYKd3rrvR96YJfzB2Oz" -->
Def. Ensemble des fonctions bornées::
$$
\mathscr{B}(X,E)=\mathrm{Set}( f\in \mathscr{F}(X,E),\;\exists M\in \mathbb{R},\;\|f\|\leq M ).
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obsf1VbFx5ruQWeIPaXmzUcO" -->
Def. Boule fermée::
$$
\overline{B}(x,\varepsilon)=\mathrm{Set}( y\in E,\;\|x-y\|\leq\varepsilon ).
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsbQ1JeFy4K743DqMwA5uAE" -->
Def. Boule ouverte::
$$
\dot{B}(x,\varepsilon)=\mathrm{Set}( y\in E,\;\|x-y\|<\varepsilon ).
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsTHsX8BnwkTO3gip56zitC" -->
Prop. Boules::
- Toujours convexe
- Toujours bornée
- Contient toujours une boule de l'autre type.
<!-- basicblock-end -->

<!-- basicblock-start oid="Obsddc8ELyPQnUWUn61Aq0EO" -->
Def. Normes usuelles de $\mathbb{K}^{n}$::
- $\|\cdot\|_{1}: x\to \sum|x_{i}|$
- $\|\cdot\|_{2}: x\to \sqrt{\sum|x_{i}|}$
- $\|\cdot\|_{\infty}: x\to \sup|x_{i}|$.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsXCbPV6a230HMPTWyB7KBh" -->
Def. Normes usuelles de $\mathscr{C}_{0}([a,b],\mathbb{K})$::
- $\|\cdot\|_{1}: f\to \int_{a}^{b}|f(t)|\mathrm{d}t$
- $\|\cdot\|_{2}: f\to \sqrt{\int_{a}^{b}|f(t)|^{2}\mathrm{d}t}$
- $\|\cdot\|_{\infty}: f\to \sup_{[a,b]}|f|$.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsyGx87Pvltcpf88Q7wqvKY" -->
Def. Normes équivalentes::
$$
\mathscr{N}_{1}\sim \mathscr{N}_{2}\iff \exists(C_{1},C_{2})\in R_{+}^{\star^{2}},\;\forall x \in E,\;C_{1}\mathscr{N}_{1}(x)\leq \mathscr{N}_{2}(x)\leq C_{2}\mathscr{N}_{1}(x).
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsEk33GdkJuzwTUP0bVyUdX" -->
Th. Equivalence de Norme::
- Si $E$ est de dimension finie, Alors toutes les normes sont équivalentes.
<!-- basicblock-end -->

<!-- basicblock-start oid="Obsi7nveab9eOfZFcVYBH2og" -->
Def. Notion topologique::
$$
\mathscr{P}\text{ est topologique}\iff \left[ (\mathscr{N}\implies \mathscr{P})\implies(\forall \mathscr{N'}\sim \mathscr{N},\;\mathscr{N'}\implies \mathscr{P}) \right].
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsDFBU7TgxOipi7DHfqAsNM" -->
Def. Convergence::
$$
(u_{n})\underset{ n }{ \to }l\iff \forall\varepsilon>0,\;\exists n_{0}\in \mathbb{N},\;\forall n\geq n_{0},\;\|u_{n}-l\|<\varepsilon.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsPN9NseQAoXR7M3vAiijrM" -->
Th. Convergence et borne::
- Si $u_{n}$ converge, alors la suite $(u_{n})$ est bornée.
<!-- basicblock-end -->

<!-- basicblock-start oid="Obs5EA9vg8rpOox52xqNxtHh" -->
Th. Convergence coordonnée par coordonnée::
$$
u_{n}=\sum_{i=1}^{N}u_{i_{n}}e_{i}\underset{ n }{ \to }l=\sum_{i}l_{i}e_{i}\iff \forall i,\;u_{i_{n}}\underset{ n }{ \to }l_{i}.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obsr3V8fobWuJ9ZYXxvSglF6" -->
Th. Convergence par monotonie::
$$
(u_{n})\nearrow\;\implies\;(u_{n})\underset{ n }{ \to }l\in \mathbb{R}\cup \mathrm{Set}( +\infty ).
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. suite adjacente::
$$
\begin{cases}
(u_{n})\searrow \\
(v_{n})\nearrow \\
|u_{n}-v_{n}|\underset{ n }{ \to }0
\end{cases}\;\implies\;\begin{cases}
u_{n}\underset{ n }{ \to }l\in \mathbb{R} \\
v_{n}\underset{ n }{ \to }l\in \mathbb{R}
\end{cases}
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. des points fixes::
$$
\begin{cases}
f\in \mathcal{C}^{0}(\mathbb{R}) \\
u_{n+1}=f(u_{n})
\end{cases}\;\implies\;\left( u_{n}\underset{n}{\to}l\;\implies\;l=f(l) \right). 
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. extractrice::
$$
\begin{cases}
\varphi:\mathbb{N}\to \mathbb{N} \\
\varphi\nearrow\nearrow
\end{cases}
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. suite extraite::
$$
u_{\varphi(_{n})}.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. comportement d'une suite extraite de suite convergente::
$$
u_{n}\underset{n}{\to}l\in \bar{\mathbb{R}}\;\implies\;u_{\varphi(n)}\underset{n}{\to}l.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. valeur d'adhérence d'une suite::
$$
u_{\varphi(n)}\to l\in E.
$$
<!-- basicblock-end -->

Bon, une suite qui converge a une unique valeur d'adhérence... Cela découle directement du fait que toute suite extraite tend vers cette limite, et donc il n'y a que cette valeur d'adhérence.

<!-- basicblock-start -->
Th. caractérisation epsilonesque de valeur d'adhérence::
$$
\forall\varepsilon>0,\;\forall n_{0}\in \mathbb{N},\;\exists n\geq n_{0},\;u_{n}\in B(a,\varepsilon).
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. voisinage d'un point::
$$
X,\;\exists\varepsilon>0,\;B(a,\varepsilon)\subset X.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. point adhérent à un ensemble::
$$
\forall\varepsilon>0,\;B(a,\varepsilon)\cap X\not=\emptyset.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. adhérence d'un ensemble::
$$
\bar{X}=\mathrm{Set}( \text{point adhérant à }X ).
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. point intérieur à un ensemble::
$$
\forall\varepsilon>0,\;B(a,\varepsilon)\subset X.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. intérieur d'un ensemble::
$$
\mathring{X}=\mathrm{Set}( \text{point intérieur à }X ).
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. frontière d'un ensemble::
$$
\delta X=\bar{X}\setminus \mathring{X}.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. caractérisation séquentielle de point adhérent::
$$
\exists(x_{n})\in X^{\mathbb{N}},\;x_{n}\underset{n}{\to}a.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. densité d'un ensemble dans un autre::
$$
X\subset E,\;\bar{X}=E.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. caractérisation par les voisinages de densité::
$$
\forall e\in E,\;\forall\varepsilon>0,\;B(e,\varepsilon)\cap X\not=\emptyset.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. caractérisation séquentielle de densité::
$$
\forall e\in E,\;\exists(x_{n})\in X^{\mathbb{N}},\;x_{n}\underset{n}{\to}e.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. ensemble ouvert::
$$
X=\mathring{X}.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. ensemble fermé::
$$
C_{X}^{E}\in \mathscr{U}(E).
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. caractérisation séquentielle des fermés::
$$
\forall(x_{n})\in X^{\mathbb{N}},\;\left( x_{n}\underset{n}{\to}x\;\implies\;x \in X \right) .
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. ensemble fermé::
- un produit de fermé est fermé
- un sev de dim finie est fermé
- stable par intersection quelconque
- stable par union finie.
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. ensemble ouvert::
- un produit d'ouvert est ouvert
- stable par union quelconque
- stable par intersection finie.
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. fermé relatif d'un ensemble::
$$
X\cap F
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. ouvert relatif d'un ensemble::
$$
X\cap U.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. ensemble compacte::
$$
\forall(x_{n})\in X^{\mathbb{N}},\;\exists\varphi ,\;x_{\varphi(n)}\underset{n}{\to}l\in X.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. ensemble compacte::
- un produit de compact est un compact
- est fermé et borné
- tout fermé relatif est un compact.
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. caractérisation des compacts en dim finies::
- fermé
- borné.
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. de Bolzano-Weierstrass dans un EVN::
$$
\forall(u_{n})\in E^{\mathbb{N}},\;(\exists M,\;\forall n\in \mathbb{N},\;|u_{n}|\leq M\;\implies\;\exists l\in E,\;\exists\varphi ,\;u_{\varphi(n)}\underset{n}{\to}l).
$$
<!-- basicblock-end -->
