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
a)
Soit $f:t\to \ln \sin t\in \mathcal{C}^{0}(]0;\pi/2])$.
On a $f(t)\underset{ 0 }{ \sim } \ln(t)$ de signe constant, donc $\int_{0}^{1}f(t)\mathrm{d}t\simeq \int_{0}^{1}\ln t\mathrm{d}t$, qui converge par Bertrand.
Ainsi, $I$ converge.
Or, par le changement de variable $u=\frac{\pi}{2}-t$ dans I, on obtient $I=J$.
Ensuite, par changement de variable $u=\frac{\pi}{2}+t$ dans $J$, on obtient via Chasles $K=I+J$.

b)
$$
\begin{align*}
I+J&=\int_{0}^{\pi/2}\ln(\sin ^{2} t)\mathrm{d}t &&\cr
&=\int_{0}^{1}\ln(u^{2})\cos u\mathrm{d}u&&\cr
I&=&&\cr
\end{align*}
$$
En posant $u=\arcsin t,\;\mathrm{d}u=\frac{1}{\sqrt{ 1-t^{2} }}\mathrm{d}t\;\implies\;\mathrm{d}t=\cos u\mathrm{d}u$
c)
...

---
# 19
a)
$f:t\to P(t)e^{t}\in \mathcal{C}^{0}(\mathbb{R})$.
En $t\to-\infty$, $P(t)\sim a_{d}t^{d}$ et donc $|f|\sim\left( \frac{1}{t^{2}} \right)(|a_{d}t^{d+2}|e^{t})=o\left( \frac{1}{t^{2}} \right)$. Et, donc $\int_{-\infty}^{x}f(t)\mathrm{d}t$ CV $\forall x \in \mathbb{R}$.
b)
$$
\begin{align*}
L(\mu_{k+1})&: x\to e^{-x}\int_{-\infty}^{x}t^{k+1}e^{t}\mathrm{d}t&&\cr
&: x\to e^{-x}\left( \left[ t^{k+1}e^{t} \right]_{-\infty}^{x}-\int_{-\infty}^{x}(k+1)t^{k}e^{t}\mathrm{d}t  \right)&&\cr
&: x\to t^{k+1}-(k+1)e^{-x}\int_{-\infty}^{x}t^{k}e^{t}\mathrm{d}t &&\cr
&=\mu_{k+1}-(k+1)L(\mu_{k})&&\cr
\end{align*}
$$
Or $L(\mu_{0})=1$, donc par récurrence:
$$
L(\mu_{k})=(-1)^{k}k!\sum_{j=0}^{k}\frac{(-1)^{j}}{j!}\mu_{j}.
$$
c)
La matrice de $L$ est trig sup, donc les valeurs propres de $L$ sont $1$, mais $L$ n'est pas l'identité, donc $L$ n'est pas DZ.






---
# DM
# Exercice 1
### 1
$$
\boxed{\lim_{ n \to \infty } P_{n}=X^{3}+1}
$$
$$
\boxed{\mathrm{Rac}_{\mathbb{C}}P=\mathrm{Set}( 1,j,\bar{j} )}
$$
---
### 2
Non, $P_{n}\in \mathbb{R}[X]$, donc ses racines complexes sont deux à deux conjugués. Or, c'est un polynôme d'ordre 3, donc il ne peut pas avoir plus de deux racines non réelles. Ainsi, elles sont forcément distinctes.

---
### 3
- Par imparité du degré de $P_{n}$, $P_{n}$ possède au moins une racine réelle.
- Or, $P_{n}'=3X^{2}+\frac{1}{n}$ ne s'annule pas sur $\mathbb{R}$, donc $P_{n}$ est strictement monotone, et ne possède donc au plus une racine réelle.
Donc, $\exists!x_{n}\in \mathbb{R},\;P_{n}(x_{n})=0$.
![[Math - Sketchbook 2026-11-08 22.30.26.excalidraw.svg]]

---
### 4
- $P_{n}(0)=-1<0$
- $P_{n}(1)=\frac{1}{n}>0$
Par le Théorème des valeurs intermédiaire (TVI), $x_{n}\in[0;1]$.

---
### 5
On a:
$$
\begin{align*}
P_{n}\left( 1-\frac{1}{n} \right)&=\left( 1-\frac{1}{n} \right)^{3}+\frac{1}{n}\left( 1-\frac{1}{n} \right)-1&&\cr
&=1-\frac{3}{n}+\frac{3}{n^{2}}-\frac{1}{n^{3}}+\frac{1}{n}-\frac{1}{n^{2}}-1&&\cr
&=-\frac{2}{n}+\frac{2}{n^{2}}-\frac{1}{n^{3}}&&\cr
&=-\frac{2}{n}\left( 1-\frac{1}{n} \right)-\frac{1}{n^{3}}&&\cr
&\leq 0&&\cr
\end{align*}
$$
Et donc, par TVI, $x_{n}\in [1-\frac{1}{n};1]$.
Et donc par le théorème des gendarmes sur cette inégalité, on obtient:
$$
\boxed{\lim_{ n \to \infty } x_{n}=1}
$$
---
### 6
a)
$P_{n}$ est un polynôme scindé à racine simple sur $\mathbb{C}$ (par 2), et un polynôme annulateur de A, donc $A$ est diagonalisable, et son spectre complexe est inclus dans $\mathrm{Rac}_{\mathbb{C}}(P_{n})$.

b)
Considérons $\chi_{A}=(X-x_{n})^{p-2k}\left[ (X-\lambda_{n})(X-\bar{\lambda_{n}}) \right]^{k}$.
Alors, $\det A=(-1)^{p}(-x_{n})^{p-2k}(\lambda_{n} \bar{\lambda_{n}})^{k}=x_{n}^{p-2k}(\lambda_{n} \bar{\lambda_{n}})^{k}\underset{ n\geq 2 }{ > }0$.

---
### 7















