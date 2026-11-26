
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
Is everything okay ??



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
Et en 0, on majore par 1 le $\cos$ et on conclut par Riemann.

---
# Chapitre 10
### 11
Soit
$$
I_{n}=\int_{0}^{+\infty}e^{-(x+1/2)^{n}}\mathrm{d}x.
$$
- $\forall x \in \mathbb{R}_{+},\;e^{-(x+1/2)^{n}}\underset{ n }{ \to }\begin{cases}1\text{ si }x< \frac{1}{2} \\  e^{-1}\text{ si }x=\frac{1}{2} \\  0\text{ si }x>\frac{1}{2}\end{cases}:=l(x)\in \mathcal{C}^{0}_{(m)}(\mathbb{R}_{+})$.
- $\forall n\in \mathbb{N}^{*},\;f_{n}\in \mathcal{C}^{0}_{(m)}(\mathbb{R}_{+})$
- $\forall n\in \mathbb{N}^{*},\;\forall x \in \mathbb{R}_{+},\;|e^{-(x+1/2)^{n}}|\leq \begin{cases}1\text{ si }x\leq \frac{1}{2} \\  e^{-(x+1/2)}\text{ sinon}\end{cases}:=\varphi(x)\in \mathcal{L}^{1}(\mathbb{R}_{+})$.
Ainsi par théorème de convergence dominée discret:
$$
\begin{align*}
\lim_{ n \to +\infty } I_{n}&=\int_{0}^{+\infty}l(x)\mathrm{d}x&&\cr
&=\frac{1}{2}.&&\cr
\end{align*}
$$
---
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

b)
C'est juste la même chose, donc bon...

c)
$$
\begin{align*}
I(a)&=\int_{0}^{a}\frac{x}{\sqrt{ (a^{2}-x^{2})(1+x^{2}) }}\mathrm{d}x&&\cr
&=\int_{0}^{1}\frac{au}{\sqrt{ (a^{2}-(au)^{2})(1+(au)^{2}) }}\frac{1}{a}\mathrm{d}u&&\cr
&=\int_{0}^{1}\frac{u}{a\sqrt{ (1-u^{2})(1+(au)^{2}) }}\mathrm{d}u&&\cr
&=\frac{1}{a}G(a)&&\cr
\end{align*}
$$








---
### 16
a)
Introduisons $f:(x,t)\to \frac{\ln(t)}{t^{2}+x}$.
- $\forall x \in \mathbb{R}_{+}^{*},\;f(x,\cdot)\in \mathcal{C}^{0}(\mathbb{R}_{+}^{*})$
Soit $x \in \mathbb{R}_{+}^{*}$, alors:
Problème en 0:
$$
\begin{align*}
f(x,t)&\underset{ t\to0 }{ \sim }-\frac{\ln(t)}{x}\in \mathcal{L}^{1}(]0;1])&&\cr
\end{align*}
$$
Problème en $+\infty$:
$$
f(x,t)\underset{ t\to+\infty }{ \sim }\frac{\ln(t)}{t^{2}}\in \mathcal{L}^{1}([1;+\infty[)
$$
Ainsi, $F(x)$ est licite.

**Continuité sous l'intégrale**
- $\forall t\in \mathbb{R}_{+},\;f(\cdot,t)\in \mathcal{C}^{0}(\mathbb{R}_{+}^{*})$
- $\forall x \in \mathbb{R}_{+}^{*},\;f(x,\cdot)\in \mathcal{C}^{0}(\mathbb{R}_{+})$
- $\forall(x,t)\in [a,b]\times \mathbb{R}_{+},\;|f(x,t)|\leq$

---

### 18
a)
Soit $x \in \mathbb{R}^{*}$, alors $f_{x}:t\to \frac{t^{-x}}{1+t}\in \mathcal{C}^{0}([1;+\infty[)$.
Problème en $+\infty$:
Par Riemann, $|f_{x}(t)|\sim\frac{1}{t^{1+x}}\in \mathcal{L}^{1}([1;+\infty[)$ ssi $x>0$.
Ainsi, $f$ est défini sur $\mathbb{R}_{+}^{*}$.

b)
Soit $h:(x,t)\to \frac{t^{-x}}{1+t}$.
Leibniz intégral:
- $\forall t\in \mathbb{R}_{+},\;h(\cdot,t)\in \mathcal{C}^{1}(\mathbb{R}_{+}^{*})$
- $\forall x \in \mathbb{R}_{+}^{*},\;h(x,\cdot)\in \mathcal{L}^{1}(\mathbb{R}_{+}),\;\frac{ \partial h }{ \partial x }=-\ln (t)h(x,t)\in \mathcal{L}^{1}(\mathbb{R}_{+})$
- Domination pour $x \in[a;b]\subset \mathbb{R}_{+}^{*}$:
$$
\forall t\in [1;+\infty[,\;|h(x,t)|\leq \frac{t^{-a}}{1+t}\in \mathcal{L}^{1}([1;+\infty[)
$$
Donc
$$
f\in \mathcal{C}^{1}(\mathbb{R}_{+}^{*})\text{ et }f'(x)=-\int_{1}^{+\infty}\ln(t) \frac{t^{-x}}{1+t}\mathrm{d}t.
$$
De plus, en tant qu'intégrale d'intégrande négative, $f'(x)$ est négative, donc $f\searrow$ sur $\mathbb{R}_{+}^{*}$.

c)
$$
\begin{align*}
f(x)+f(1+x)&=\int_{1}^{+\infty} \frac{t^{-x}}{1+t}+\frac{t^{-(x+1)}}{1+t}\mathrm{d}t&&\cr
&=\int_{1}^{+\infty} \frac{t^{-(x+1)}}{1+t}(t+1)\mathrm{d}t &&\cr
&=\int_{1}^{+\infty} t^{-(x+1)}\mathrm{d}t &&\cr
&=\left[ -\frac{1}{x}t^{-x} \right]_{1}^{t\to +\infty}&&\cr
&=\frac{1}{x}  &&\cr
\end{align*}
$$
d)
$$
\begin{align*}
f(x)&=\frac{1}{x}-f(x+1)&&\cr
&=\frac{1}{x}-\int_{1}^{+\infty} \frac{t^{-(x+1)}}{t+1}\mathrm{d}t &&\cr
&\sim_{0} \frac{1}{x}-\int_{1}^{+\infty} \frac{1}{t(t+1)}\mathrm{d}t &&\cr
&\sim \frac{1}{x}-\int_{1}^{+\infty} \frac{1}{t}-\frac{1}{t+1}\mathrm{d}t &&\cr
&\sim \frac{1}{x}-\left[ \ln t-\ln(t+1) \right]_{1}^{t\to +\infty}&&\cr
&\sim\frac{1}{x}+\ln2&&\cr
&\sim \frac{1}{x} &&\cr
\end{align*}
$$
Bon, pas besoin de calculer $f(1)$, on peut juste conclure en disant que c'est un nombre.

En $x\to +\infty$:
...

e)
Voir ci-dessus.

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
---

### 32
a)
Soit $h:(x,t)\to \frac{e^{-x(1+t^{2})}}{1+t^{2}}=e^{-x}\left( \frac{e^{-xt^{2}}}{1+t^{2}} \right)$.
Alors, $f: x\to \int_{0}^{+\infty}h(x,t)\mathrm{d}t$.
Si $x<0$, $f(x)$ est grossièrement divergente.
Si $x\geq 0$, $f(x)$ est ACV par majoration de l'exponentielle décroissante par 1, puis par Riemann.

b)
$$
\frac{ \partial h }{ \partial x } (x,t)=-e^{-x(1+t^{2})}
$$
**Th. Leibniz intégral**
- $\forall t\in \mathbb{R}_{+},\;h(\cdot,t)\in \mathcal{C}^{1}(\mathbb{R}_{+}^{*})$
- $\forall x \in \mathbb{R}_{+}^{*}, h(x,\cdot)\in \mathcal{L}^{1}(\mathbb{R}_{+}),\;\frac{ \partial h }{ \partial x }(x,\cdot)\in \mathcal{L}^{1}(\mathbb{R}_{+}^{*})$
- $\forall(x,t)\in [a,b]\times \mathbb{R}_{+},\;|\frac{ \partial h }{ \partial x }(x,t)|\leq e^{-a(1+t^{2})}\in \mathcal{L}^{1}(\mathbb{R}_{+})$
donc $f\in \mathcal{C}^{1}(\mathbb{R}_{+}^{*})$ et
$$
f'(x)=-\int_{0}^{+\infty}e^{-x(1+t^{2})}\mathrm{d}t=-e^{-x}\int_{0}^{+\infty}e^{-xt^{2}}\mathrm{d}t
$$
On pose $u=\sqrt{ x }t$, donc $\mathrm{d}u=\sqrt{ x }\mathrm{d}t$, donc
$$
f'(x)=-\frac{e^{-x}}{\sqrt{ x }}I.
$$
c)
Soit $A>0$, alors
$$
\begin{align*}
f(A)-f\left( \frac{1}{A} \right)&=\left[ f(t) \right]_{\frac{1}{A}}^{A}&&\cr
&=\int_{\frac{1}{A}}^{A}f'(t)\mathrm{d}t &&\cr
&=-I\int_{\frac{1}{A}}^{A} \frac{e^{-x}}{\sqrt{ x }}\mathrm{d}x&&\cr
&=-2I\int_{\frac{1}{\sqrt{ A }}}^{\sqrt{ A }}e^{-u^{2}}\mathrm{d}u &&\cr
\end{align*}
$$



---
### 33
$$
\begin{align*}
I(x)&=\int_{0}^{\pi/2} \frac{1}{\cos ^{2}t+x\sin ^{2}t}\mathrm{d}t &&\cr
&=\int_{0}^{\pi/2} \frac{1}{\cos ^{2}t}\cdot \frac{1}{1+x\tan ^{2}t}\mathrm{d}t &&\cr
&=\int_{0}^{+\infty} \frac{1}{1+xu^{2}}\mathrm{d}u&&\cr
&=\frac{1}{\sqrt{ x }}\int_{0}^{+\infty} \frac{\sqrt{ x }}{1+(\sqrt{ x }u)^{2}}\mathrm{d}u&&\cr
&=\left[ \frac{1}{\sqrt{ x }}\arctan(\sqrt{ x }u) \right]_{0}^{u\to+\infty}&&\cr
&=\frac{\pi}{2\sqrt{ x }} &&\cr
\end{align*}
$$
En posant $u=\tan t$, $\mathrm{d}u=\frac{1}{\cos ^{2}(t)}\mathrm{d}t$.

$$
\begin{align*}
J(x)&=\int_{0}^{\pi/2} \frac{\sin^{2}(t)}{(\cos ^{2}t+x\sin ^{2}t)^{2}}\mathrm{d}t &&\cr
&=\int_{0}^{\pi/2}\frac{\sin(t)}{\cos(t)} \frac{\cos(t)\sin(t)}{(\cos ^{2}t+x\sin ^{2}t)^{2}}\mathrm{d}t &&\cr
&=\left[\tan t\times \frac{1}{2(x-1)(\cos ^{2}t+x\sin ^{2}t)} \right]_{0}^{t\to \pi/2}-\int_{0}^{\pi/2}(1+\tan ^{2} t) \frac{1}{2(x-1)(\cos ^{2}t+x\sin ^{2}t)}\mathrm{d}t &&\cr
&= &&\cr
\end{align*}
$$

$$
f(t)=\frac{1}{\cos ^{2}t+x\sin ^{2}t}
$$
$$
f'(t)=-(2\cos t(-\sin t)+2x\sin t\cos t)f^{2}(t)=2(x-1)\cos t\sin tf^{2}(t)
$$
Pas d'idée... Ha si. Dommage, crochet impropre.

Montrons que $I\in \mathcal{C}^{1}(\mathbb{R}_{+}^{*})$, via Leibniz intégral:
Soit $f:(x,t)\to \frac{1}{\cos ^{2}t+x\sin ^{2}t}$, alors
- $\forall t\in [0;\frac{\pi}{2}], f(\cdot,t)\in \mathcal{C}^{1}(\mathbb{R}_{+}^{*})$
- 
- 


---
### 39
a)
Soit $a\in]1;+\infty[$, alors
Problème en $+\infty$:
$$
\frac{sh(x)}{x}e^{-ax}=\frac{1}{x^{2}}\cdot\left( x\frac{e^{(1-a)x}-e^{-(1+a)x}}{2} \right)\in \mathcal{L}^{1}([1;+\infty[)
$$
Problème en $0$:
$$
\frac{sh(x)}{x}e^{-ax}\sim_{0} \frac{x}{x}e^{-ax}\in \mathcal{L}^{1}([0;1])
$$
Donc $\forall a\in]1;+\infty[$, $I(a)$ existe.

b)
soit
$$
f: (a,x)\to  \frac{sh(x)}{x}e^{-ax}
$$
Théorème de convergence dominée:
- $\forall x \in \mathbb{R}_{+},\; \frac{sh(x)}{x}e^{-ax} \underset{ a }{ \to }0=l(x)\in \mathcal{L}^{1}$
- ...
- Domination sur $[42;+\infty[$:
$$
f(a,x)\leq \frac{sh(x)}{x}e^{-42x}\in \mathcal{L}^{1}(\mathbb{R}_{+})
$$
Donc l'intégrale de la limite existe et l'on peut les permuter:
$$
\lim_{ a \to +\infty } \int_{\mathbb{R}_{+}}f(a,x)\mathrm{d}x=0
$$
c)



---
### 42
a)
Soit $s\in]0;1[$, alors
Problème en 0, par Riemann:
$$
|u^{s-1}e^{iu}|=\frac{1}{u^{1-s}}\in \mathcal{L}^{1}([0;1])
$$
Problème en $+\infty$:
Par une IPP ne changeant pas la nature:
$$
\begin{align*}
\int_{1}^{+\infty}u^{s-1}e^{iu}\mathrm{d}u&=\left[ u^{s-1}e^{iu} \right] -\int_{1}^{+\infty}u^{s-2}e^{iu}\mathrm{d}u&&\cr
&=e^{i}-\int_{1}^{+\infty} \frac{1}{u^{2-s}}e^{iu}\mathrm{d}u&&\cr
\end{align*}
$$
Et donc, par Riemann, la deuxième est ACV, DLR.
(Bon, je me rends compte que mon IPP est pas bonne, mais ça fonctionne comme ça)

b)
Soit $x \in \mathbb{R}$, alors
Problème en 0, par Riemann:
$$
|t^{s-1}e^{(-1+ix)t}|\sim_{0} \frac{1}{t^{1-s}}\in \mathcal{L}^{1}([0;1])
$$
Problème en $+\infty$, par CC:
$$
|t^{s-1}e^{(-1+ix)t}|\sim_{+\infty} t^{s-1}e^{-t}\in \mathcal{L}^{1}([1;+\infty[).
$$
c)
Soit $g:(x,t)\to t^{s-1}e^{(-1+ix)t}$
Par Leibniz intégral:
- $\forall t\in \mathbb{R}_{+}, g(\cdot,t)\in \mathcal{C}^{1}(\mathbb{R})$, et $\frac{ \partial g }{ \partial x }(\cdot,t)=it^{s}e^{(-1+ix)t}$
- $\forall x \in \mathbb{R},\;g(x,\cdot)\in \mathcal{L}^{1}(\mathbb{R}_{+})$ et $\frac{ \partial g }{ \partial x }(x,\cdot)\in \mathcal{L}^{1}(\mathbb{R}_{+})$ par Riemann et CC
- Domination:
$$
\begin{align*}
|\frac{ \partial g }{ \partial x } (x,t)|&=t^{s}e^{-t}\in \mathcal{L}^{1}(\mathbb{R}_{+}).&&\cr
\end{align*}
$$
Donc
$$
f\in \mathcal{C}^{1}(\mathbb{R})\text{ et }f'(x)=\int_{0}^{+\infty}it^{s}e^{(-1+ix)t}\mathrm{d}t.
$$
Par IPP,
$$
\begin{align*}
f'(x)&=\left[ \frac{i}{-1+ix}t^{s}e^{(-1+ix)t} \right]_{0}^{+\infty}-\int_{0}^{+\infty} \frac{is}{-1+ix}t^{s-1}e^{(-1+ix)t}\mathrm{d}t &&\cr
&=\frac{is}{1-ix}f(x) &&\cr
\end{align*}
$$

d)


---
# [[Math - Lesson - 11|Chapitre 11]]

### 46
a)
Soit
$$
I_{n}=\int_{0}^{+\infty} \frac{1}{(1+t^{2})^{n}}\mathrm{d}t.
$$
Notons
$$
f_{n}:t\to \frac{1}{(1+t^{2})^{n}}\in \mathcal{C}^{0}([0;+\infty[).
$$
Problème en $+\infty$:
$$
f_{n}(t)\sim \frac{1}{t^{2n}}\in \mathcal{L}^{1}([1;+\infty[).
$$
Donc, $\forall n\in \mathbb{N}^{\star},\;I_{n}$ existe.

b)
Par le théorème de domination discret:
- $\forall t\in \mathbb{R}_{+}^{\star},\;f_{n}(t)\underset{n}{\to}0=l(t)\in \mathcal{L}^{1}(\mathbb{R}_{+})$
- $\forall n\in \mathbb{N},\;f_{n}\in \mathcal{C}^{0}_{(m)}(\mathbb{R}_{+})$
- Domination
$$
\begin{align*}
|f_{n}(t)|&= \frac{1}{(1+t^{2})^{n}}&&\cr
&\leq \frac{1}{1+t^{2}}\in \mathcal{L}^{1}(\mathbb{R}_{+}).&&\cr
\end{align*}
$$
Donc $\lim_{ n \to +\infty }I_{n}=0$.

c)
Par changement de variable, on pose $u=1+t^{2},\;t=\sqrt{ u-1 }$
Donc $\mathrm{d}u=2t\mathrm{d}t$
Ainsi
$$
\begin{align*}
I_{n}&=\int_{1}^{+\infty} \frac{1}{u^{n}2\sqrt{ u-1 }}\mathrm{d}u&&\cr
&=\left[ \frac{\sqrt{ u-1 }}{u^{n}} \right]_{1}^{u\to +\infty}+\int_{1}^{+\infty} \frac{\sqrt{ u-1 }}{u^{n+1}}\mathrm{d}u&&\cr
&=\int_{0}^{+\infty} \frac{v}{(v+1)^{2n+2}}2v\mathrm{d}v&&\cr
&=\int_{0}^{+\infty} \frac{2v^{2}}{(v+1)^{2n+2}}\mathrm{d}v&&\cr
\end{align*}
$$
Par SSA en fait, moi qui espérais l'éviter...
### 2

$$
\begin{align*}
\sum_{k=1}^{+\infty} \frac{1}{1+k^{2}}&=a_{n}+\sum_{k=1}^{n} \frac{1}{1+k^{2}}&&\cr
V&=a_{n}+\sum_{k=1}^{n}1-\frac{k^{2}}{1+k^{2}}&&\cr
&=a_{n}+n\times \frac{1}{n}\sum_{k=1}^{n}1-\frac{\left( \frac{k}{n} \right)^{2}}{1+\left( \frac{k}{n} \right)^{2}}&&\cr
&=a_{n}+n\int_{0}^{1}1-\frac{t^{2}}{1+t^{2}}\mathrm{d}t &&\cr
&=a_{n}+n\left[ \arctan t \right] _{0}^{1}&&\cr
&=a_{n}+n\frac{\pi}{2}&&\cr
\end{align*}
$$
Bon c'est faux.
Par contre, grâce au magnifique théorème du cours de ce matin
$$
\frac{1}{1+k^{2}}\sim \frac{1}{k^{2}}\geq 0.
$$
Donc, par convergence par Riemann et positivité
$$
a_{n}\sim \sum_{k=n}^{+\infty} \frac{1}{k^{2}}\sim \frac{1}{n}
$$


---
### 5
1. 
si $b_{n}\underset{n}{\to}l\in \mathbb{R}$, alors
$$
l=
$$

Alors, en inversant la relation, on trouve:
$$
a_{n}=b_{n}(b_{n+1}-b_{n})
$$
Or, $a_{n}\not=0$ par $b_{n}\not=b_{n+1}\not=0$, donc d'alembert:
$$
\begin{align*}
|\frac{a_{n+1}}{a_{n}}|&=\frac{b_{n+1}}{b_{n}}\frac{b_{n+2}-b_{n+1}}{b_{n+1}-b_{n}}&&\cr
&&&\cr
\end{align*}
$$
Bon, tout ce qu'il y a au-dessus n'est d'aucune utilité, je recommence.
a)
1. 
On sait que $b_{0}=1$, et $b_{n+1}=b_{n}+\frac{a_{n}}{b_{n}}>b_{n}$, donc si $(b_{n})$ converge, c'est vers $l\geq 1$.
2. 
???

b)
1. 
Par a) 1. on a $\forall n\in \mathbb{N},\;b_{n}\geq1\;\implies\;\frac{a_{n}}{b_{n}}\leq a_{n}$, ainsi par CV de $\sum a_{n}$, $\sum \frac{a_{n}}{b_{n}}$ CV.
2. 
$$
\forall n\in \mathbb{N},\;b_{n}=b_{0}+\sum_{k=0}^{n-1}\frac{a_{k}}{b_{k}}
$$
Et donc, par passage à la limite, $(b_{n})$ CV.

---
### 12
a)
Soit
$$
f_{n}:t\to e^{-t^{n}}\in \mathcal{C}^{0}([0;+\infty[).
$$
Soit $t \in[1;+\infty[$:
$$
\begin{align*}
1&\leq n&&\cr
t&\leq t^{n}&&\cr
-t&\geq-t^{n}&&\cr
e^{-t}&\geq e^{-t^{n}}&&\cr
e^{-t}&\geq|f_{n}(t)|&&\cr
\end{align*}
$$
Donc par $(t\to e^{-t})\in \mathcal{L}^{1}([1;+\infty[)$, $f_{n}\in \mathcal{L}^{1}([0;+\infty[)$.

b)
Par théorème de domination discret
- $\forall t\in \mathbb{R}_{+},\;f_{n}(t)\underset{n}{\to}\begin{cases}1\text{ si }t<1 \\  e^{-1}\text{ si }t=1 \\  0\text{ si }t>1\end{cases}:=l(t)\in \mathcal{L}^{1}([0;+\infty[)$
- $\forall n\in \mathbb{N}^{\star},\;f_{n}\in \mathcal{C}^{0}_{(m)}(\mathbb{R}_{+})$
- Domination
$$
\varphi(t)=\begin{cases}
1\text{ si }t\leq1 \\
e^{-t}\text{ sinon}
\end{cases}\in \mathcal{L}^{1}([0;+\infty[).
$$
Donc
$$
v_{n}\to \int_{0}^{+\infty}l(t)\mathrm{d}t=1.
$$
c)
On pose le changement de variable $u=t^{n}$, $\mathrm{d}t=\frac{1}{nu^{1-1/n}}\mathrm{d}u$
$$
\begin{align*}
u_{n}&=\int_{0}^{+\infty}e^{-t^{n}}\mathrm{d}t-1&&\cr
&=\int_{0}^{+\infty}e^{-u} \frac{1}{nu^{1-1/n}}\mathrm{d}u-1&&\cr
&=\frac{1}{n}\int_{0}^{+\infty}e^{-u}u^{1/n-1}\mathrm{d}u-\int_{0}^{+\infty}e^{-t}t^{0}\mathrm{d}t&&\cr
&=\frac{1}{n}\Gamma\left( \frac{1}{n} \right)-\Gamma(1).&&\cr
\end{align*}
$$
d)
Comment ?? Okay, apparemment Noah a trouvé quelque chose.

---
### 17
Soit
$$
u_{n}=\frac{1}{a_{n}} \sum_{k=1}^{n}a_{k}b_{k}.
$$


---
### 21
a)
Très simplement par les intégrales partielles, on découpe et on passe à la limite, et on obtient que c'est le double de la somme moins le terme initiale.

b)
Soit $u_{n}=(-1)^{n}$, alors $\sum u_{n+1}+u_{n}=0$ CV, mais pas $\sum u_{n}$.

c)
Soit $u_{n}\geq 0$, supposons $\sum u_{n+1}+u_{n}$ CV.
Introduisons $P_{n}=\sum_{k=0}^{n}u_{k+1}+u_{k}$ qui converge par hypothèse et $S_{n}=\sum_{k=0}^{n}u_{k}$ dont l'on va montrer la convergence.
(Ainsi, $\sum_{n=0}^{+\infty}P_{n+1}-P_{n}=\sum_{n=0}^{+\infty}a_{}$ CV... Hah. NON.)

Ainsi, par positivité de $u_{n}$, $S_{n}\nearrow$, et $\forall n\in \mathbb{N},\;0\leq S_{n}\leq P_{n}$.
Par passage à la limite, $S_{n}$ majorée et croissante, donc CV, donc $\sum u_{n}$ CV.

---
### 27
a)
$$
\begin{align*}
e^{(1/n)\sum_{k=1}^{n}\ln k}&\geq 1+\frac{1}{n}\sum_{k=1}^{n}\ln k&&\cr
&\geq&&\cr
\end{align*}
$$


---
### 34

Vu $\sum a_{n}$ CV, $\exists M,\;\forall n\in \mathbb{N},\;\sum ^{n}a_{k}\leq M$.

On a alors
$$
\begin{align*}
|\frac{\sum_{k=0}^{n}\lambda_{k}u_{k}}{\sum_{k=0}^{n}\lambda_{k}}|&\leq M| \frac{\sum_{k=0}^{n}\lambda_{k}}{\sum_{k=0}^{n}\lambda_{k}}|&&\cr
&\leq M&&\cr
\end{align*}
$$
Donc cette suite est majorée...
Mais ce n'est pas ce que je veux.



---
### 38
a)
$$
u_{n}=\sin(\pi(2-\sqrt{ 3 })^{n})
$$
On a
$$
0\leq i=2-\sqrt{ 3 }<1
$$
Donc
$$
i^{n}\underset{n}{\to}0
$$
Ainsi,
$$
\begin{align*}
u_{n}&\sim \pi i^{n}\geq 0&&\cr
\end{align*}
$$
Et donc $\sum u_{n}$ CV.

b)
$$
0=\sin(\pi((2-\sqrt{ 3 })^{n}+(2+\sqrt{ 3 }^{n})))=\cos(\pi(2-\sqrt{ 3 })^{n})\sin(\pi(2+\sqrt{ 3 })^{n})+\cos(\pi(2+\sqrt{ 3 })^{n})\sin(\pi(2-\sqrt{ 3 })^{n}).
$$

donc
$$
\begin{align*}
\sin(\pi(2+\sqrt{ 3 })^{n})&=-\frac{\cos(\pi(2+\sqrt{ 3 })^{n})}{\cos(\pi i^{n})}\sin(\pi i^{n})&&\cr
&\sim-\cos(\pi(2+\sqrt{ 3 })^{n})\pi i^{n}&&\cr
\end{align*}
$$
Or
$$
|-\cos(\pi(2+\sqrt{ 3 })^{n})\pi i^{n}|\leq \pi i^{n}\in \mathcal{L}^{1}(\mathbb{N}).
$$
Donc $\sum v_{n}$ CV.

---
### 39

$$
\begin{align*}
u_{n}&=\ln \left( \frac{n^{2}+2an+a^{2}}{n^{2}+(b+c)n+bc} \right)&&\cr
&=\ln \left( 1+ \frac{(2a-b-c)n+a^{2}-bc}{n^{2}+(b+c)n+bc}\right)&&\cr
&\sim \frac{(2a-b-c)n+a^{2}-bc}{n^{2}+(b+c)n+bc}  \text{ de signe constant}&&\cr
\end{align*}
$$
Donc $\sum u_{n}$ CV ssi $2a=b+c$.

Bon, par le SSA:
- $(-1)^{n}u_{n}$ est alterné APCR
- $|(-1)^{n}u_{n}|\underset{n}{\to} 0$ par l'équivalent trouvé
- $|(-1)^{n}u_{n}|\searrow$ par l'équivalent trouvé

Ainsi $\sum(-1)^{n}u_{n}$ CV.
Hah, en fait le SSA ne suffit pas, il faut faire un DL

---
### 50
g)
$$
\begin{align*}
u_{n}&=e^{\ln(n)/n^{2}}-1&&\cr
&\sim \frac{\ln(n)}{n^{2}}\geq0&&\cr
\end{align*}
$$
Et donc, par BeBert, $\sum u_{n}$ CV
i)
$$
\begin{align*}
u_{n}&=e(1-e^{n\ln(1+1/n)-1})&&\cr
&\sim e\left( n\ln\left( 1+\frac{1}{n} \right)-1 \right)&&\cr
&\sim e\left( n\left( \frac{1}{n}-\frac{1}{2n^{2}}+O\left( \frac{1}{n^{3}} \right) \right)-1 \right)&&\cr
&\sim \frac{e}{2}\cdot \frac{1}{n^{2}}\leq 0&&\cr
\end{align*}
$$
Et donc, par Riemann et équivalence de série, $\sum u_{n}$ CV.
o)
$\forall n\in \mathbb{N},\;u_{n}\not=0$, donc, par d'Alembert
$$
\begin{align*}
| \frac{u_{n+1}}{u_{n}}|&=|\frac{(-1)^{n+1}(2n+2)!}{(-1)^{n}(2n)!}\cdot \frac{4^{n}(n!)^{2}}{4^{n+1}((n+1)!)^{2}}|&&\cr
&=|(-1)(2n+2)(2n+1)\cdot \frac{1}{4(n+1)^{2}}|&&\cr
&=\frac{4n^{2}+3n+2}{4n^{2}+8n+4}&&\cr
&\to 1.&&\cr
\end{align*}
$$
Bon, d'Alembert donne rien.

Par SSA:
- $u_{n}$ est bien alterné
Att, mais est-ce que son terme général ne tend pas vers $+\infty$?
Je ne sais passssss
Il est tard...

Et bien, continuons le SSA
- Par ma tentative de d'Alembert, on voit $|u_{n}|\searrow$
- Pour le fait que ça tende vers 0, j'ai pas d'idée, tentons stirling

$$
\begin{align*}
|u_{n}|&\sim \frac{\frac{(2n)^{2n}}{e^{2n}}\sqrt{ 4\pi n }}{4^{n} \frac{n^{2n}}{e^{2n}}2\pi n}&&\cr
&\sim \frac{2^{2n}}{4^{n}\sqrt{ \pi n }}&&\cr
&\sim \frac{1}{\sqrt{ \pi n }}&&\cr
&\to0&&\cr
\end{align*}
$$
ça fonctionne.
Donc par SSA, $\sum u_{n}$ CV.


q)
$$
\begin{align*}
u_{n}&=\frac{(-1)^{n}(n+i)}{n^{2}-1}&&\cr
&=\frac{(-1)^{n}n}{n^{2}-1}+i\frac{(-1)^{n}}{n^{2}-1}&&\cr
\end{align*}
$$
Par SSA, les deux convergent, et l'on obtient la convergence coordonnée par coordonnée.

---

### 52
a)
par récurrence immédiate, $\forall n\in \mathbb{N},\;u_{n}\in \mathbb{R}_{+}^{\star}$.
De même, $(u_{n})\searrow$.
Ainsi, $\exists l\in [0;1],\;u_{n}\underset{n}{\to}l$.
Donc $l=le^{-l}$. Si par l'absurde, $l\not=0\;\implies\;l=0$, donc $l=0$.

b)
On a
$$
u_{n}= u_{n}\left( 1-u_{n}+\frac{u_{n}^{2}}{2}+O(u_{n}^{3}) \right)\;\implies\;u_{n}^{2}=\frac{u_{n}^{3}}{2}+O(u_{n}^{4})\;\implies\;u_{n}\sim \sqrt{ \frac{u_{n}^{3}}{2} }
$$
Heinn????
ça montre des choses bizarres...

---
### 54
a)
Soit
$$
(u_{n}):\begin{cases}
u_{0}\in \mathbb{R} \\
u_{n+1}=\frac{e^{-u_{n}}}{n+1}
\end{cases}
$$
On travaille sur $\mathbb{N}^{\star}$ afin d'avoir $u_{n}\geq 0$

Lemme: $u_{n}\underset{n}{\to} 0$
Démo: par $u_{n}\geq0$, $u_{n+1}\leq \frac{1}{n+1}$.

Ainsi
$$
\begin{align*}
u_{n}&\sim \frac{1}{n+1}&&\cr
&\sim \frac{1}{n}\geq0&&\cr
\end{align*}
$$
Donc $\sum u_{n}$ DV.

b)
Ainsi, $u_{n}^{2}\sim  \frac{1}{n^{2}}\geq0$ Donc $\sum u_{n}^{2}$ CV.

---

### 56

Soit
$$
f:\begin{cases}
E&\to \mathbb{N} \\
(p,q)&\to p+q
\end{cases}
$$
On note
$$
E_{n}=f^{-1}(\mathrm{Set}( n )).
$$
On a alors
$$
\begin{cases}
\#E_{n}=n-1 \\
a_{n}=\sum_{(p,q)\in E_{n}}a_{p,q}=\sum_{(p,q)\in E_{n}} \frac{1}{n^{2}-2pq}
\end{cases}
$$

$$
\forall(p,q)\in \mathbb{N}^{\star^{2}},\; p^{2}+q^{2}\geq2pq \;\implies\; \frac{1}{p^{2}+q^{2}}\leq \frac{1}{2pq}.
$$
Oui, mais ça, ça diverge directement.




---
### 58
On groupe selon des paquet de Cauchy, $n=p+q$.
Soit $r=|z|$, $\sum_{p,q}\binom{p+q}{q}z^{p+q}$ est sommable ssi $S=\sum_{n=0}^{+\infty}\sum_{k=0}^{n}\binom{n}{k}r^{n}$ CV

$$
\begin{align*}
S&=\sum_{n=0}^{+\infty}r^{n}\sum_{k=0}^{n}\binom{n}{k}&&\cr
&=\sum_{n=0}^{+\infty}r^{n}2^{n}&&\cr
&=\sum_{n=0}^{+\infty}(2r)^{n}&&\cr
\end{align*}
$$
 CV ssi $2r<1\iff r< \frac{1}{2}$
Donc $F$ est sommable ssi $|z|< \frac{1}{2}$.

---
### 59
a)

Soit $p\geq2$
$$
\forall n\geq 2,\;u_{n,p}=\left( \frac{z}{p} \right)^{n}
$$
Or $|\frac{z}{p}|<1$ donc
$$
\sum_{n\geq 2}u_{n,p}=\frac{z^{2}}{p^{2}-pz}.
$$
$$
S_{p}=\sum_{n\geq2}|\frac{z}{p}|^{n}=\frac{|z|^{2}}{p^{2}-p|z|}.
$$
b)

On a
$$
\sum_{p\geq 2}S_{p}\text{ CV par Riemann.}
$$
Donc, par Fubini, la famille est sommable.

c)

donc, par Fubini, on a
$$
\begin{align*}
\sum_{n\geq 2}\sum_{p\geq 2}u_{n,p}&=\sum_{p\geq 2}\sum_{n\geq2}u_{n,p}&&\cr
\sum_{n\geq 2}z^{n}\sum_{p\geq 2} \frac{1}{p^{n}}&=\sum_{p\geq 2} \frac{z^{2}}{p(p-z)}&&\cr
\sum_{n\geq 2}z^{n}(\zeta(n)-1)&=\sum_{p\geq 2}\frac{z^{2}}{p(p-z)}&&\cr
\end{align*}
$$
En prenant $z=1$, on obtient
$$
\begin{align*}
\sum_{n\geq 2}(\zeta(n)-1)&=\sum_{n\geq2} \frac{1}{p(p-1)}&&\cr
&=\sum_{n\geq 2}\left( \frac{1}{p}-\frac{1}{p-1} \right) &&\cr
&=\frac{1}{2-1}&&\cr
&=1.&&\cr
\end{align*}
$$


### 63
a)
$$
\begin{align*}
\sum_{n=0}\frac{z^{2n+1}}{1-z^{2n+1}}&=\sum_{n=0}\sum_{p=1}(z^{2n+1})^{p}&&\cr
&=\sum_{p=1}\sum_{n=0}(z^{p})^{2n+1}&&\cr
&=\sum_{p=1}z^{p}\sum_{n=0}(z^{2p})^{n}&&\cr
&=\sum_{p=1}z^{p}\cdot \frac{1}{1-z^{2p}}.&&\cr
\end{align*}
$$

# [[Math - Lesson - 12|Chapitre 12]]

### 3
a)
On a
$$
[H]_{i,j}=<x_{i}:o_{j}>.
$$
Ainsi
$$
\begin{align*}
[H^{T}\times H]_{i,j}&=\sum_{k=1}^{n}[H^{T}]_{i,k}[H]_{k,j}&&\cr
&=\sum_{k=1}^{n}<x_{k}:o_{i}>\cdot<x_{k}:o_{j}>&&\cr
&=\sum_{k=1}^{n}&&\cr
\end{align*}
$$

Comment montrez que ça vaut $<x_{i}: x_{j}>$ ?

---
### 6

On a toujours symétrie et bilinéarité.
Pour la définie positivité:
- Positivité
Soient $X$ et $A$, alors
$$
\begin{align*}
<X:X>&=X^{T}A^{T}AX&&\cr
&&&\cr
\end{align*}
$$
- Définition
Soient $X$ et $A$ tq
$$
\begin{align*}
0&=<X:X>&&\cr
&=X^{T}A^{T}AX&&\cr
\end{align*}
$$

Je ne cois pas savoir comment faire...

---

### 7
a)
Il n'y a pas la définition pour $X=\begin{pmatrix}0 \\  0 \\  1\end{pmatrix}$.
Donc ce n'est pas un produit scalaire
b)
Il le semble que tout est bon, vérifié assez facilement.
c)
De même, tout fonctionne.
d)
Par ### 6, ça fonctionne en dimension finie.
Maintenant, quand j'aurais trouvé le 6), je ferais celui là.

---
### 8
a)
$$
M^{2}=XX^{T}XX^{T}=X\cdot\|X\|^{2}\cdot X^{T}=\|X\|^{2}\cdot M.
$$
Ainsi
$$
P=X(X-\|X\|^{2})
$$
est un polynôme annulateur de $M$, et vu $M\not=0$, $P$ est son polynôme minimal.
Donc $\mathrm{Sp}M=\mathrm{Set}( 0,\|X\|^{2} )$.

b)
Vu $P$ SARS, $M$ DZ.
élément propre... Flemme

---
### 9
$$
\begin{align*}
\left( \sum_{k=1}^{n}a_{k}b_{k}c_{k} \right)^{2}&=\sum_{i=1}^{n}\sum_{j=1}^{n}a_{i}a_{j}b_{i}b_{j}c_{i}c_{j}&&\cr
\end{align*}
$$
$$
\begin{align*}
\left( \sum_{k=1}^{n}a_{k}^{2}c_{k} \right)\left( \sum_{k=1}^{n}b_{k}^{2}c_{k} \right)&=\sum_{i=1}^{n}\sum_{j=1}^{n}a_{i}^{2}b_{j}^{2}c_{i}c_{j}&&\cr
\end{align*}
$$

Comment je compare les deux ? Il y a une astuce avec des vecteurs j'imagine.
Okay, apparemment, il y a un truc, mais je n'arrive juste pas à le trouver...

---
### 10
a)
C'est la question 1. du cours
b)
C'est le Cauchy-Schwartz du pauvre! Hah, non
$$
\begin{align*}
|a+b|&=\sqrt{ a^{2}+2ab+b^{2} }&&\cr
&\leq\sqrt{ a^{2}+2|ab|+b^{2} }&&\cr
&\leq \sqrt{ a^{2}+2\left( \frac{1}{2}(a^{2}+b^{2}) \right)+b^{2} }&&\cr
&\leq \sqrt{ 2a^{2}+2b^{2} }&&\cr
&\leq \sqrt{ 2 }\sqrt{ a^{2}+b^{2} }.&&\cr
\end{align*}
$$

c)
Pas d'idée sur comment faire...
Par contre, une fois le résultat établie, en utilisant b) sur le membre de gauche, on obtient l'inégalité des normes voulues.

d)
Non, en prenant $f_{n}=\cos(n\cdot)$, le rapport explose.

---
### 11

Soient $X=\begin{pmatrix}x_{1} \\  \vdots \\  x_{n}\end{pmatrix}$et $\bar{X}=\begin{pmatrix}\frac{1}{x_{1}} \\  \vdots \\  \frac{1}{x_{n}}\end{pmatrix}$.
On veut montrer que $<X:\bar{X}>\geq n^{2}$.
Par Cauchy-Schwartz
$$
\begin{align*}
<X:\bar{X}>&\leq\|X\|\cdot\|\bar{X}\|&&\cr
&\leq\left( \sum_{k=1}^{n}x_{k}^{2} \right)\left( \sum_{k=1}^{n} \frac{1}{x_{k}^{2}} \right)&&\cr
&\leq \sum_{i=1}^{n}\sum_{j=1}^{n} \left( \frac{x_{i}}{x_{j}} \right)^{2}&&\cr
&\leq \sum_{i=1}^{n}1^{2}+\sum_{1\leq i<j\leq n}\left( \left( \frac{x_{i}}{x_{j}} \right)^{2}+\left( \frac{x_{j}}{x_{i}} \right)^{2} \right)&&\cr
&\leq n+\sum_{1\leq i<j\leq n}2&&\cr
&\leq n+\frac{n(n-1)}{2}\cdot2&&\cr
&\leq n^{2}&&\cr
\end{align*}
$$

Okay, pourquoi je trouve l'inverse ??? Okay, il y a pas mal d'erreurs dans mon raisonnement (saurez vous les trouver?).

---

### 13
a)
$a$ et $b$ sont non colinéaire par hypothèse (liberté de la famille), donc on a pas l'égalité dans l'inégalité de Cauchy-Schwarz.
b)
On reconnait la distance entre $c$ et $\mathrm{Vect}(a,b)$. Calculons la projections orthogonale de $c$ sur $\mathrm{Vect}(a,b)$.
On a
$$
p(c)=\lambda a+\mu b.
$$
Et
$$
\begin{cases}
<c-p(c):a> =0 \\
<c-p(c):b> =0
\end{cases}
$$
On a donc
$$
\begin{cases}
<c:a> =\lambda\|a\|+\mu<a:b> \\
<c:b> =\lambda<a:b>+\mu\|b\|.
\end{cases}
$$


### 15
a)
Soit $(\lambda_{i})$ tq
$$
x=\sum_{i=1}^{n}\lambda_{i}e_{i}=0.
$$
Alors, $\|x\|=0$, d'où
$$
\forall i\in[1;n],\;<\sum_{j=1}^{n}\lambda_{j}e_{j};e_{i}>=0\;\implies\;\sum_{j=1}^{n}\lambda_{j}<e_{j};e_{i}> =0
$$
Sauf que l'on ne sait pas comment sont ces produits scalaires, on a pas assez d'information. Ou en tout cas, je n'ai pas assez pour faire.

b)
Soit $x \in X^{\bot}$, alors
$\forall i\in[1;p],\;<x;e_{i}> =0$
Ainsi, par la propriété de l'hypothèse, $x=0$.
Ainsi, $X=\mathrm{Set}( 0 )^{\bot}=E$.
Donc $(e_{i})$ étant libre (par a) et génératrice, c'est une base.
De plus, pour tout $e_{i}\not=e_{j}, <e_{i};e_{j}> =0$ par propriété de base.
Ainsi, par hypothèse, $(e_{i})$ est une base orthonormée.

---

### 19
a)
$$
\begin{align*}
\left( \int_{0}^{1}f(t)\mathrm{d}t \right)^{2}&\leq\left( \int_{0}^{1}|f(t)|\mathrm{d}t \right)^{2}&&\cr
&\leq&&\cr
\end{align*}
$$

Pas d'idée.
Je cherche une propriété du type $<f;g> \leq$
Okay, je l'ai
Par
$$
|<f;g>|^{2}\leq\|f\|^{2}\cdot\|g\|^{2}
$$
Ou quelque chose comme ça, il y en a trop des inégalités dans ce cours.
J'écrirais tout ça bien demain, une fois reposée.

---
### Suite
