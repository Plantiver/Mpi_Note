---
deck: math
---
<!-- basicblock-start oid="Obs2bj85bpGMtggr2c81a3YA" -->
Def. intervalle impropre::
$$
\int_{]a,b]}f(t)\mathrm{d}t,\;f\text{ DV en }a.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsVAopmTMKvdxqTU852dG39" -->
Prop. calcul d'une intégral impropre::
- $\int_{]a,b]}f(t)\mathrm{d}t=\lim_{ x \to a }\int_{[x,b]}f(t)\mathrm{d}t$
- 
<!-- basicblock-end -->

<!-- basicblock-start oid="Obs8lcGlWTKfwWkCj0RImxiE" -->
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

<!-- basicblock-start oid="Obsh5PC36GzD5xppnCwKTjWZ" -->
Def. fonction absolument convergente::
$$
f,\;\int_{I}|f(t)|\mathrm{d}t\text{ CV}
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




<!-- basicblock-start oid="ObseVE4PeT6PBZfQxru4c1XR" -->
Th. convergence usuelle::
- $\ln \in \mathcal{L}^{1}(]0,1])$
- $(t\to e^{-at})\in \mathcal{L}^{1}([0,+\infty[)\iff a>0$
- $\left( t\to \frac{1}{t^{a}} \right)\in \mathcal{L}^{1}([1,+\infty])\iff a>1$
- $\left( t\to\frac{1}{t^{a}} \right)\in \mathcal{L}^{1}(]0,1])\iff a<1$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsIsswKymPdv3KerUayQ6T6" -->
Th. nature d'une intégrale::
- Convergente
- Divergente
<!-- basicblock-end -->

Dans la suite, deux intégrale de même natures seront notées avec $\simeq$.

<!-- basicblock-start oid="ObsL9AKIpmuUrgRzioh191Hp" -->
Th. intégrale tronqué::
$$
\int_{[a,b[}f(t)\mathrm{d}t\simeq \int_{[c>a,b[}f(t)\mathrm{d}t.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsEdBnZ3SHkjy6qVUor51kt" -->
Prop. changement de variable pour une intégrale impropre::
- $\mathcal{C}^{1}$
- $\leftrightsquigarrow$
- $\nearrow\nearrow$ ou $\searrow\searrow$.
<!-- basicblock-end -->


# 11
Par l'absurde, supposons la convergence de $\int_{I}f+g$.
Alors, par stabilité, $\int_{I}f+g-\int_{I}f=\int_{I}g$ CV, absurde.


#todo : th about domination et équivalence de fonction

# 13
a)
$$
\begin{align*}
\int_{0}^{+\infty}f(t)\mathrm{d}t&\simeq \int_{0}^{+\infty}\lambda \mathrm{d}tnl&&\cr
\end{align*}
$$
Donc, diverge car $\lambda \in \mathbb{R}^{\star}$

b)
$$
\begin{align*}
\int_{0}^{+\infty}\frac{\sin ^{2}t}{t^{2}}\mathrm{d}t&= \int_{0}^{1}\frac{\sin^{2}t}{t^{2}}\mathrm{d}t+\int_{1}^{+\infty}\frac{\sin ^{2}t}{t^{2}}\mathrm{d}t &&\cr
&\simeq \int_{0}^{1}1\mathrm{d}t+\int_{1}^{+\infty}\frac{1}{t^{2}}\mathrm{d}t&&\cr
\end{align*}
$$
par positivité de $\frac{\sin ^{2}t}{t^{2}}$, et équivalence en $0$ avec $t$, et par majoration par $1$.
Donc, converge par sommes de telles intégrales.

c)
$$
\begin{align*}
\int_{0}^{+\infty}\frac{t^{2}}{1+t^{4}}e^{-t}\mathrm{d}t&\simeq \int_{42}^{+\infty}\frac{1}{t^{2}e^{t}}\mathrm{d}t&&\cr
&\leq \int_{42}^{+\infty}\frac{1}{t^{2}}\mathrm{d}t &&\cr
\end{align*}
$$
donc converge par riemman.

d)
$$
\begin{align*}
\int_{0}^{+\infty}\ln te^{-\sqrt{ t }}\mathrm{d}t&=\int_{0}^{1}\ln te^{-\sqrt{ t }}\mathrm{d}t+\int_{1}^{+\infty}\ln te^{-\sqrt{ t }}\mathrm{d}t&&\cr
&\simeq \int_{0}^{1}\ln t\mathrm{d}t+\int_{0}^{+\infty}&&\cr
\end{align*}
$$


f)
...
g)
voir les photos du profs...



#todo : do it properly
<!-- basicblock-start oid="ObslZURWyWHVnyfWpmtxl8T3" -->
Th. ipp d'intégrale impropre::
- L’IPP sur des fonctions C 1 conserve la nature/valeur des intégrales impropres si l’on signale/justifie qu’il y a des limites finies aux crochets impropre.
<!-- basicblock-end -->



---

Questions à poser:
- Peut-on passer des applications linéaires dans des intégrales impropres?
- Sur la méthode de calcul, est-ce qu'on sépare toujours, ou, est-ce qu'on peut faire tendre les deux bornes? à ce moment est-ce qu'on peut faire tendre comme on veut, ou pas?
- théorème de réarrangement de Riemann sur les intégrales?































