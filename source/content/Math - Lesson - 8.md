---
deck: math
---
<!-- basicblock-start -->
Def. Dérivabilité en un point::
$$
f(x_{0}+h)=f(x_{0})+L(h)+o(h).
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. Classe de régularité::
$$
f\in \mathcal{C}^{k}(D,E)\iff \begin{cases}
f\in \mathcal{D}^{k}(D,E) \cr
f^{(k)}\in \mathcal{C}^{0}(D,E)
\end{cases}
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. Chain rule::
$$
(f\circ g)'=g'\times f'\circ g.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. Structures des classes de régularités::
- $\mathcal{C}^{k}(D,E)$ est un $\mathbb{K}$-EV
- $\mathcal{C}^{k}(D)$ est une $\mathbb{K}$-Algèbre.
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. de Leibniz::
$$
\left[ \hat{b}(f,g) \right] ^{(n)}=\sum_{k=0}^{n}\begin{pmatrix}
n \cr
k
\end{pmatrix}\hat{b}(f^{(k)},g^{(n-k)})
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. de Rolle::
$$
\begin{cases}
f\in \mathcal{C}^{0}([a,b]) \cr
f\in \mathcal{D}^{0}(]a,b[) \cr
f(a)=f(b)
\end{cases}\;\implies\;\exists c\in]a,b[,\;f'(c)=0.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. accroissement fini::
$$
\begin{cases}
f\in \mathcal{C}^{0}([a,b]) \cr
f\in \mathcal{D}^{0}(]a,b[)
\end{cases}\;\implies\;\exists c\in]a,b[,\;f(b)-f(a)=f'(c)(b-a).
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. des bijections::
$$
\begin{cases}
f\in \mathcal{C}^{0}([a,b]) \cr
f\nearrow\nearrow\text{ ou }f\searrow\searrow
\end{cases}\;\implies\;\begin{cases}
f:[a,b]\leftrightsquigarrow [\lim_{ a } f,\lim_{ b } f] \cr
f:^{-1}\in \mathcal{C}^{0}
\end{cases}
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. Dérivée d'une réciproque::
$$
(f^{-1})' = \frac{1}{f'\circ f^{-1}}.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. des accroissement finis::
$$
f\in \mathcal{C}^{0}(I,E),\;\left( \exists M\in \mathbb{R},\;\forall x \in I,\;\|f'(x)\|\leq M \right) \;\implies\;f\text{ est }M\text{-lispschitzienne}.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. fonction continue par morceaux::
$$
\exists(a_{k})_{k=0}^{N},\;a=a_{0}<\dots<a_{N}=b,\;\forall i\in[0,N-1],\;f_{|]a_{i},a_{i+1}[}\in \mathcal{C}^{0}(]a_{i},a_{i+1}[).
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. somme de Riemann::
$$
S_{n}=\frac{b-a}{n}\sum_{k=0}^{n-1}f\left( a+k\frac{b-a}{n} \right).
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. convergence des sommes de Riemann::
$$
S_{n}(f)\underset{ n }{ \to }\int_{a}^{b}f(t)\mathrm{d}t.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. primitive d'une fonction::
$$
F,\;F'=f.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. fondamentale de l'analyse::
- $F(x)=\int_{a}^{x}f(t)\mathrm{d}t\;\implies\;\begin{cases}F(a)=0\cr F'=f\end{cases}$
- $F'=f\;\implies\;\int_{a}^{b}f=F(b)-F(a)$.
<!-- basicblock-end -->


<!-- basicblock-start -->
Th. développement de Taylor::
$$
f(x)=\sum_{k=0}^{p}\frac{f^{(k)}(a)}{k!}(x-a)^{k}+o((x-a)^{p}).
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. développement de Taylor reste intégral::
$$
f(x)=\sum_{k=0}^{p}\frac{f^{(k)}(a)}{k!}(x-a)^{k}+\int_{a}^{x}\frac{f^{(p+1)}(t)}{p!}(x-t)^{p}\mathrm{d}t.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. Majoration du reste intégral::
$$
\int_{a}^{x}\frac{f^{(p+1)}(t)}{p!}(x-t)^{p}\mathrm{d}t\leq\frac{|x-a|^{p+1}}{(p+1)!}\cdot max_{[a,x]}\|f^{(p+1)}\|.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. développement de Taylor usuel::
$$
f(a+h)=\sum_{k=0}^{p}\frac{f^{(k)}(a)}{k!}h^{k}+o(h^{p}).
$$
<!-- basicblock-end -->

On peut intégrer un DL.
De même, on peut dériver un DL.


