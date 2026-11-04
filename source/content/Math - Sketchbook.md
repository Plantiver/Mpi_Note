19, 22 a,b, 27, 31

# 19
a)
$f$ est $\mathcal{C}^{1}$ donc $f'$ est $\mathcal{C}^{0}$, et donc par le th. des bornes atteintes, est bornée et atteint ses bornes. Donc $supA$ est licite et atteint.
$\varphi:\begin{cases}X^{2}&\to \mathbb{R} \\  (x,y)&\to \begin{cases}|\frac{f(x)-f(y)}{x-y}|\text{ si }x\not=y \\  |f'(x)|\text{ sinon}\end{cases}\end{cases}$ est continue et défini sur un compact. Donc $\varphi(X^{2})$ est un compact, donc borné, et donc $B\subset\varphi(X^{2})$ est borné.

b)
hein???

# 22
a)
$$
f:t\to \frac{\sin t-t}{t\sin t}
$$
$$
\begin{align*}
f&\sim- \frac{t^{3}}{6t^{2}}&&\cr
&\sim- \frac{t}{6}&&\cr
\end{align*}
$$
Ainsi$f$ qui est $\mathcal{C}^{1}$ partout ailleurs qu'en $0$, et est $\mathcal{C}^{0}$ partout en posant $f(0)=0$, On a que $f$ est $\mathcal{C}^{1}$.

b)
$f:t\to \arctan e^{-t^{2}}$
$$
\begin{align*}
f(t)&=\arctan\left( 1-t^{2}+\frac{t^{4}}{2}+o(t^{5}) \right)&&\cr
&=&&\cr
\end{align*}
$$

# 27
a)
$$
\begin{align*}
u_{n}&=\frac{1}{n}\sum_{k=1}^{n}\ln\left( 1+\frac{k}{n} \right)&&\cr
&\to \int_{1}^{2}\ln(t)\mathrm{d}t&&\cr
&\to2\ln 2-1&&\cr
\end{align*}
$$
b)
$$
\begin{align*}
\ln(v_{n})&=\frac{1}{n}\left( \sum_{k=1}^{2n}\ln(k)-\sum_{k=1}^{n}\ln(k)-n\ln(n) \right)&&\cr
&=\frac{1}{n}\left( \sum_{k=n+1}^{2n}\ln(k)-n\ln n \right)&&\cr
&=\frac{1}{n}\left( \sum_{i=1}^{n}\ln\left( 1+\frac{i}{n} \right) \right)&&\cr
v_{n}&=e^{\sigma/n}&&\cr
&\to e&&\cr
\end{align*}
$$

# 31
a)
Bon, ça se fait rapidement, flemme

b)
Soit $P=\sum_{k=0}^{n}a_{k}X^{k}\in\mathrm{Ker}\theta$.
Alors, par linéarité:
$$
\begin{align*}
\sum_{k=0}^{n}a_{k}\theta_{k}(P)&=0&&\cr
&=\int_{0}^{1}\sum_{k=0}^{n}a_{k}t^{k}P(t)\mathrm{d}t&&\cr
&=\int_{0}^{1}P^{2}(t)\mathrm{d}t&&\cr
\end{align*}
$$

c)
Or, $P^{2}$ est continue et positive, donc la question précédente signifie que $P^{2}=0\;\implies\;P=0$, donc $\mathrm{Ker}\theta=\mathrm{Set}( 0 )$, et donc $\theta$ est injective.
Or, ce sont deux espaces de même dim, donc $\theta$ est bijective, un isomorphisme.






































