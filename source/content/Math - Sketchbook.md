TD MPI. 6, 10, 16, 19


# 6
a) ? parce qu'elle est intégrable, mais pour quoi exactement ?
b)
Soit $l\in \mathbb{R},\;\lim_{ x \to +\infty }f(x)=l$. Alors, $\exists A\in \mathbb{R}^{+},\;\forall x\geq A,\;f(x)\in\left[ \frac{l}{2};\frac{3l}{2} \right]$. et l'on a $\int_{\mathbb{R}^{+}}f\simeq \int_{A}^{+\infty}f$, avec $f$ alors de signe constant $\mathrm{si}(l)$. Si par l'absurde $l\not=0$, alors cette intégrale diverge, ce qui contredis l'énoncé.
c)
Par IPP:
$$
\begin{align*}
\int_{0}^{+\infty}f(t)\sin(xt)\mathrm{d}t&=\left[ -\frac{f(t)\cos(xt)}{x} \right]_{0}^{+\infty}-\int_{0}^{+\infty}f'(t)\times\left( -\frac{\cos(xt)}{x} \right)\mathrm{d}t&&\cr
&=\frac{f(0)}{x}+\frac{1}{x}\int_{0}^{+\infty}f'(t)\cos(xt)\mathrm{d}t &&\cr
\end{align*}
$$
Avec le crochet licite par $|\cos x|\leq 1$ et $f$ intégrable.
d)
On a, par une deuxième IPP, qui se justifie comme la première:
$$
\begin{align*}
\int_{0}^{+\infty}f'(t)\cos(xt)\mathrm{d}t&=\left[ \frac{f'(t)\sin(xt)}{x} \right]_{0}^{+\infty}-\int_{0}^{+\infty}\frac{f''(t)\sin(xt)}{x}\mathrm{d}t &&\cr
&=-\frac{f'(0)}{x}-\frac{1}{x}\int_{0}^{+\infty}f''(t)\sin(xt)\mathrm{d}t&&\cr
&=-\frac{1}{x}\left( f'(0)+\int_{0}^{+\infty}f''(t)\sin(xt)\mathrm{d}t \right)&&\cr
&=-\frac{1}{x}\lambda&&\cr
\end{align*}
$$
Donc:
$$
I= \frac{f(0)}{x}-\frac{1}{x}\left( \frac{1}{x}\lambda \right)=\frac{f(0)}{x}+o\left( \frac{1}{x} \right).
$$
Et donc, si $f(0)\not=0$:
$$
I\underset{ +\infty }{ \sim } \frac{f(0)}{x}
$$
---
# 10
Soit
$$
I=\int_{0}^{+\infty}\frac{t^{x-1}}{1+t}\mathrm{d}t
$$
Notons $f:t\to \frac{t^{x-1}}{1+t}\in \mathcal{C}^{0}(]0;+\infty[)$.
On observe que $\lim_{ t \to 0^{+} }f(t)=0$ pour $x\not=1$, et l'on décide de prolonger $f$ par continuité en $t=0$.

En $t\to+ \infty$, par positivité de $f$:
$$
\begin{align*}
\int_{42}^{+ \infty}\frac{t^{x-1}}{1+t}\mathrm{d}t&\simeq \int_{42}^{+ \infty}t^{x-2}\mathrm{d}t&&\cr
\end{align*}
$$
Par critère de Riemann, $I$ converge pour $x \in \mathbb{R}_{-}^{\star}$.
De plus:
$$
\begin{align*}
I&=\int_{0}^{1}\frac{t^{x-1}}{1+t}\mathrm{d}t+\int_{1}^{+\infty}\frac{t^{x-1}}{1+t}\mathrm{d}t&&\cr
&=\int_{0}^{1}\frac{t^{x-1}}{1+t}\mathrm{d}t+\int_{1}^{0}\left( \frac{u^{1-x}}{1+\frac{1}{u}} \right)\left( -\frac{1}{u^{2}} \right)\mathrm{d}u&&\cr
&=\int_{0}^{1}\frac{t^{x-1}}{1+t}\mathrm{d}t+\int_{0}^{1}\frac{u^{-x}}{1+u}\mathrm{d}u&&\cr
&=\int_{0}^{1}\frac{t^{x-1}+t^{-x}}{1+t}\mathrm{d}t&&\cr
\end{align*}
$$
En posant $u=\frac{1}{t}$.

---
# 16

---
# 19

























