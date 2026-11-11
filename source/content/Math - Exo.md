
# Chapitre 9
### 6
a)
Par $f'$ intégrable et le TFI, on obtient que $f$ est l'intégrale des restes, qui tends donc vers 0.
b)
Soit $l\in \mathbb{R},\;\lim_{ x \to +\infty }f(x)=l$. Alors, $\exists A\in \mathbb{R}^{+},\;\forall x\geq A,\;f(x)\in\left[ \frac{l}{2};\frac{3l}{2} \right]$. et l'on a $\int_{\mathbb{R}^{+}}f\simeq \int_{A}^{+\infty}f$, avec $f$ alors de signe constant $\mathrm{si}(l)$. Si par l'absurde $l\not=0$, alors cette intégrale diverge, ce qui contredis l'énoncé.
c)
!! Ne pas oublier la CV !! -> se fait par ACV en majorant $\sin$ par $1$.
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
&=-\frac{1}{x}\lambda(x)&&\cr
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
### 10
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
### 13
Soit $h: x\to \frac{g^{2}(x)}{x^{2}}\in \mathcal{C}^{0}(]0;+\infty[)$.

Problème en 0:
Prenons $F$ primitive de $f^{2}$, alors $\lim_{ x \to 0 }\frac{g^{2}(x)}{x^{2}}=\lim_{ x \to 0 }\left( \frac{F(x)-F(0)}{x-0} \right)^{2}=F'^{2}(0)=f^{2}(0)>0$, on peut donc prolonger par continuité en cette valeur et pouf plus de problème.

Problème en $+\infty$:
Par $f^{2}$ intégrable, $\exists l\in \mathbb{R},\;g(x)\underset{ x\to+\infty }{ \to }l$
Ainsi, $g^{2}(x)\sim_{+\infty}l^{2}\geq 0$, et donc $\frac{g^{2}(x)}{x^{2}}\sim_{+\infty}\frac{l^{2}}{x^{2}}\in \mathcal{L}^{1}([1;+\infty[)$

Donc $h\in \mathcal{L}^{1}(]1;+\infty[)$.

---
### 16
a)
Soit $f:t\to \ln \sin t\in \mathcal{C}^{0}(]0;\pi/2])$.
On a $f(t)\underset{ 0 }{ \sim } \ln(t)$ de signe constant, donc $\int_{0}^{1}f(t)\mathrm{d}t\simeq \int_{0}^{1}\ln t\mathrm{d}t$, qui converge par Bertrand.
Ainsi, $I$ converge.
Or, par le changement de variable $u=\frac{\pi}{2}-t$ dans I, on obtient $I=J$.
Ensuite, par changement de variable $u=\frac{\pi}{2}+t$ dans $J$, on obtient via Chasles $K=I+J$.

b)
$$
\begin{align*}
I+J&=\int_{0}^{\pi/2}\ln(\sin t\cos t)\mathrm{d}t &&\cr
&=\int_{0}^{\pi/2}\ln\left( \frac{1}{2}\sin(2t) \right)\mathrm{d}t &&\cr
&=\frac{\pi}{2}\ln\left( \frac{1}{2} \right)+\int_{0}^{\pi/2}\ln(\sin2t)\mathrm{d}t &&\cr
&=-\frac{\pi}{2}\ln2+\frac{1}{2}\int_{0}^{\pi}\ln \sin u \mathrm{d}u&&\cr
&=-\frac{\pi}{2}\ln2+I&&\cr
\end{align*}
$$
c)
Via les bonnes IPP.

---
### 19
a)
$f:t\to P(t)e^{t}\in \mathcal{C}^{0}(\mathbb{R})$.
En $t\to-\infty$, $P(t)\sim a_{d}t^{d}$ et donc $|f|\sim\left( \frac{1}{t^{2}} \right)(|a_{d}t^{d+2}|e^{t})=o\left( \frac{1}{t^{2}} \right)$. Et, donc $\int_{-\infty}^{x}f(t)\mathrm{d}t$ CV $\forall x \in \mathbb{R}$.
b)
$$
\begin{align*}
L(\mu_{k+1})&: x\to e^{-x}\int_{-\infty}^{x}t^{k+1}e^{t}\mathrm{d}t&&\cr
&: x\to e^{-x}\left( \left[ t^{k+1}e^{t} \right]_{t\to-\infty}^{x}-\int_{-\infty}^{x}(k+1)t^{k}e^{t}\mathrm{d}t  \right)&&\cr
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
$$
\mathcal{Mat}_{\mathscr{C}}(L)=\begin{pmatrix}
1  &  \dots & (-1)^{n}n! \\
 & \ddots & \vdots \\
 (0)&  & 1 
\end{pmatrix}
$$
---
### 25
e)
Soit $f: t\to \frac{\mathrm{ch}t-\cos t}{t^{5/2}}\in \mathcal{C}^{0}(]0;1])$
Par DL en 0:
$$
\begin{align*}
f(x)&=\frac{1+\frac{x^{2}}{2}-\left( 1-\frac{x^{2}}{2} \right)+o(x^{2})}{x^{5/2}}&&\cr
&=\frac{1}{\sqrt{ x }}+o\left( \frac{1}{\sqrt{ x }} \right)\in \mathcal{L}^{1}(]0;1])&&\cr
\end{align*}
$$
Par Riemann.
m)
Soit $f:t\to \tan^{a}t\in \mathcal{C}^{0}\left( ]0;\frac{\pi}{2}[ \right)$ pour $a\in \mathbb{R}^{\star}$.
Problème en 0:
$$
\begin{align*}
f(t)&\sim t^{a}&&\cr
\end{align*}
$$
de signe constant, intégrable par Riemann pour $a>-1$.
Problème en $\frac{\pi}{2}$:
$$
\begin{align*}
f\left( t-\frac{\pi}{2} \right)&=\frac{\sin^{a}\left( t-\frac{\pi}{2} \right)}{\cos^{a}\left( t-\frac{\pi}{2} \right)}&&\cr
&=-\frac{\cos^{a} t}{\sin^{a} t}&&\cr
&\sim_{0}-\frac{1}{t^{a}}&&\cr
\end{align*}
$$
de signe constant, intégrable par Riemann pour $a<1$.
n)
$$
\begin{align*}
I&=\int_{\mathbb{R}^{+}}t-\lfloor t \rfloor \mathrm{d}t &&\cr
&=\sum_{i=0}^{+\infty}\int_{0}^{1}t\mathrm{d}t &&\cr
&=\frac{1}{2}\sum_{i=0}^{n}1&&\cr
&=+\infty&&\cr
\end{align*}
$$
o)
$$
f:t\to \sqrt{ t-\sin t }-\sqrt{ t }\in \mathcal{C}^{0}([1;+\infty[)
$$
$$
\begin{align*}
\sqrt{ t-\sin t }-\sqrt{ t }&=\frac{t-\sin t-t}{\sqrt{ t-\sin t }+\sqrt{ t }}&&\cr
&=-\frac{\sin(t)}{\sqrt{ t }\left( \sqrt{ 1-\frac{\sin t}{t} }+1 \right)}&&\cr
&=-\frac{\sin(t)}{2\sqrt{ t }\left( 1+\frac{1}{4}\frac{\sin(t)}{t}+o\left( \frac{\sin(t)}{t} \right) \right)}&&\cr
&=-\frac{\sin(t)}{2\sqrt{ t }}\left( 1+\frac{1}{4}\frac{\sin(t)}{t}+o\left( \frac{\sin(t)}{t} \right) \right)&&\cr
\end{align*}
$$
Concentrons nous sur la convergence de $I=\int_{\pi}^{+\infty}\frac{\sin(t)}{\sqrt{ t }}\mathrm{d}t$, le reste convergeant par majoration puis critère de Riemann.

Changement de variable, posons $u=\sqrt{ t }$, alors $\mathrm{d}u=\frac{1}{2\sqrt{ t }}\mathrm{d}t\;\implies\;\mathrm{d}t=2u\mathrm{d}u$.
On a donc:
$$
\begin{align*}
I&=\int_{\pi}^{+\infty}\frac{\sin(u^{2})}{u}2u\mathrm{d}u&&\cr
&=2\int_{\pi}^{+\infty}\sin(u^{2})\mathrm{d}u&&\cr
\end{align*}
$$
D'après une rapide recherche sur [internet](https://en.wikipedia.org/wiki/Fresnel_integral), j'apprends que cette intégrale converge.
La preuve et le calcul directe se fond par des procédés que nous n'avons malheureusement pas encore vu (et je crois malheureusement que nous ne nous y attellerons pas), mais je tacherais néanmoins d'en donner une idée.
On s'intéresse à l'intégrale de $f:z\to e^{-z^{2}}$ holomorphe sur un contour fermé $\gamma:[0;1]\to \mathbb{C}$, autant dire une quantité nulle. En décomposant ensuite le contour en plusieurs chemins, on calcule l'intégral sur chacun de ces chemins, et l'on trouve pour l'un d'entre eux la moitié de l'intégral de Gauss (dont je ne détaillerais pas le calcul), une quantité que l'on fait tendre vers 0, et une quantité qui contient notre inconnue.
En résolvant, on trouve:
$$
\int_{0}^{+\infty}\sin(u^{2})\mathrm{d}u=\sqrt{ \frac{\pi}{8} }.
$$
Bon, ce ne nous donne pas la valeur de l'intégrale de départ, mais ça nous assure la convergence.

Le prof m'a également signalé que par une IPP en dérivant la racine, on prouve la convergence.

---
### 27
a)
Converge par $f(t)\sim\frac{1}{t^{3}}>0$, critère de Riemann.
$$
\begin{align*}
I&=\int_{1}^{+\infty}\frac{1}{t(t+1)(t+2)}\mathrm{d}t &&\cr
&=\int_{1}^{+\infty}\frac{1}{2t}-\frac{1}{t+1}+\frac{1}{2(t+2)}\mathrm{d}t&&\cr
&=\left[ \frac{1}{2}\ln t-\ln(t+1)+\frac{1}{2}\ln(t+2) \right]_{1}^{t\to+\infty}&&\cr
&=\lim_{ t \to +\infty } \frac{1}{2}\ln\left( \frac{t(t+2)}{(t+1)^{2}} \right)-\ln\left( \frac{\sqrt{ 3 }}{2} \right) &&\cr
&=-\ln \frac{\sqrt{ 3 }}{2}&&\cr
\end{align*}
$$
---
### 38
Voir [[Math - Exo#25]], o).

# Chapitre 10
### 15
a)
Soit $f_{a}:\begin{cases}\mathbb{R}_{+}^{\star}&\to \mathbb{K} \\  x&\to \frac{x}{a\sqrt{ (a^{2}-x^{2})(x^{2}+1) }}\end{cases}$
- $\forall a\in \mathbb{R}_{+}^{\star},\;f_{a}\in \mathcal{C}^{0}([0,a[)$
$$
\begin{align*}
|f(x)|&=\frac{x}{a\sqrt{ (a+x)(x^{2}+1) }}\cdot\frac{1}{\sqrt{ a-x }}&&\cr
&=\frac{x}{a\sqrt{ (a+x)(x^{2}+1) }}\cdot \frac{1}{\sqrt{ a }}&&\cr
\end{align*}
$$







---
### 19
a)
$$
\forall n\in \mathbb{N},\;f_{n}\in \mathcal{C}^{0}([0;+\infty[)
$$

$$
\begin{align*}
|f_{n}(t)|&=o_{+\infty}\left( \frac{1}{t^{2}} \right)\in \mathcal{L}^{1}(\mathbb{R}_{+})&&\cr
\end{align*}
$$
Donc, $\forall n\in \mathbb{N},\;f_{n}\in \mathcal{L}^{1}(\mathbb{R}_{+})$.
b)
- $\forall t\in \mathbb{R}_{+},\;\lim_{ n \to +\infty }f_{n}(t)=\frac{1}{1+t^{2}}$
- $\forall n\in \mathbb{N},\;f_{n}(t)\leq \frac{1}{t^{2}}\in \mathcal{L}^{1}(\mathbb{R}_{+})$
Par le théorème de convergence dominée discret:
$$
I_{n}=\int_{0}^{+\infty}\frac{1}{1+t^{2}}\mathrm{d}t=[\arctan t]_{0}^{t\to +\infty}=\frac{\pi}{2}
$$



