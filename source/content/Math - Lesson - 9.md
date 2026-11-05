---
deck: math
---
<!-- basicblock-start -->
Def. intervalle impropre::
$$
\int_{]a,b]}f(t)\mathrm{d}t,\;f\text{ DV en }a.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. calcul d'une intégral impropre::
- $\int_{]a,b]}f(t)\mathrm{d}t=\lim_{ x \to a }\int_{[x,b]}f(t)\mathrm{d}t$
- 
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. convergence d'une intégral impropre::
$$
\int_{[a,b[}f(t)\mathrm{d}t\text{ CV}\iff \exists M,\;\forall x \in[a,b[,\;\int_{[a,x]}f(t)\mathrm{d}t\leq M
$$
<!-- basicblock-end -->

# Exo 2
$$
\begin{align*}
f(t)&=\frac{1+t-(1+2t)+o(t)}{t}&&\cr
&=-1+o(1)&&\cr
&\underset{ 0 }{ \to }-1&&\cr
\end{align*}
$$
Donc cette intégrale est faussement impropre, prolongeable par continuité en 0.

# Exo 3
a)
Idée, DV sauf si f=0:
Soit $x>0$:
$$
\begin{align*}
\int_{[0,x]}c\mathrm{d}t&=cx&&\cr
&\underset{ x\to + \infty }{ \to }\begin{cases}
+\infty\text{ si }c\not=0 \\
0\text{ sinon}
\end{cases}&&\cr
\end{align*}
$$
Donc, ça confirme l'hypothèse.

b)
$f\in \mathcal{C}^{0}([1,+\infty[)$, alors, soit $x>0$
$$
\begin{align*}
\int_{[1,x]}\frac{1}{t^{2}}\mathrm{d}t&=\left[ -\frac{1}{t} \right]_{0}^{x}&&\cr
&=1-\frac{1}{x}&&\cr
&\underset{ x\to +\infty }{ \to }1&&\cr
\end{align*}
$$
Donc l'intégrale converge par convergence des intégrales partielles.

c)
$f\in \mathcal{C}^{0}([1,+\infty[)$, alors, soit $x>0$
$$
\begin{align*}
\int_{[1,x]}\frac{1}{t^{2}}\mathrm{d}t&=\left[ \ln(t) \right]_{0}^{x}&&\cr
&=\ln(x)&&\cr
&\underset{ x\to +\infty }{ \to }+\infty&&\cr
\end{align*}
$$
Donc divergence par divergence des intégrales partielles.

d)
Ici, on va séparer l'intégrale en une partie avec $x$ positif et une avec $x$ négatif.
- Soit $x\geq0$:
$$
\begin{align*}
\int_{[0,x]}\frac{1}{1+t^{2}}\mathrm{d}t&=[\arctan t]_{0}^{x}&&\cr
&=\arctan x&&\cr
&\to \frac{\pi}{2}&&\cr
\end{align*}
$$
- Soit $x\leq0$:
same...

e)
$f\in \mathcal{C}^{0}(]-\infty , -2])$, alors, soit $x\leq2$:
$$
\begin{align*}
\int_{[x,-2]}\frac{1}{t(t^{2}-1)}\mathrm{d}t&=\int_{[x,-2]}\frac{1}{t}+\frac{1}{2}\left[ \frac{1}{t-1}+\frac{1}{t+1} \right]&&\cr
&=\left[ -\ln|t|+\frac{1}{2}(\ln|t-1|+\ln|t+1|) \right]_{x}^{-2}&&\cr
&=\left[ \ln \frac{\sqrt{ |t-1|\cdot|t+1| }}{|t} \right]_{x}^{-2}&&\cr
&=\ln \frac{\sqrt{ 3 }}{2}-\ln \frac{\sqrt{ |x^{2}-1| }}{|x|}&&\cr
&\to \ln \frac{\sqrt{ 3 }}{2}-0&&\cr
\end{align*}
$$
La décomposition en élément simple à la première ligne se fait à part bien sûr
Donc, ça converge par convergence des intégrales partielles.

<!-- basicblock-start -->
Def. fonction absolument convergente::
$$
\int_{I}|f(t)|\mathrm{d}t\text{ CV}
$$
<!-- basicblock-end -->

# 5
a)
bon, les dessin, pas trop mon truc

b)
Soit $f\in \mathcal{L}^{1}(J)$, et $I\subset J$, alors:
$$
\begin{align*}
\int_{I}|f(t)|\mathrm{d}t&\leq \int_{I}|f(t)|\mathrm{d}t+\int_{J\setminus I}|f(t)|\mathrm{d}t&&\cr
&\leq \int_{J}|f(t)|\mathrm{d}t&&\cr
\end{align*}
$$
Par hypothèse, ceci est majorée, donc, par positivité de $|f|$, et notre CNS, $|f|$ est absolument convergente, donc $f\in \mathcal{L}^{1}(I)$.






















































