
Jolie schéma #todo 

Pour simplifier, on suppose que la tige est à température uniforme à $x$ fixée ($T(x,r,t)=T(x,t)$).

On se place en régime stationnaire et on cherche $T(x)$.

On réalise un bilan de puissance sur une portion de tige entre $x$ et $x+\mathrm{d}x$.

Joli schéma des flux à travers une portion de tige infinitésimal.

$$
\begin{align*}
\phi(x)&=j_{\text{th}}(x)S&&\cr
\phi(x+\mathrm{d}x)&=j_{\text{th}}(x+\mathrm{d}x)S&&\cr
\phi_{\text{latéral}}&=j_{\text{cc}}S_{\text{latéral}}&&\cr
\end{align*}
$$
avec
- $S=\pi R^{2}$ où $R$ est le rayon de la tige
- $S_{\text{latéral}}=2\pi R\mathrm{d}x$ la surface du tour de la portion de tige.
- $j_{\text{cc}}=h(T(x)-T(x+\mathrm{d}x))$

En stationnaire
$$
\begin{align*}
\phi(x)&=\phi(x+\mathrm{d}x)+\phi_{\text{latéral}}&&\cr
(j_{\text{th}}(x)-j_{\text{th}}(x+\mathrm{d}x))\pi R^{2}&=j_{\text{cc}}2\pi R\mathrm{d}x&&\cr
-\frac{\mathrm{d}j_{\text{th}}}{\mathrm{d}x}\pi R^{2}\mathrm{d}x&=h(T(x)-T_{\text{air}})2\pi R\mathrm{d}x&&\cr
\lambda \frac{d^{2}T}{\mathrm{d}x^{2}}&=\frac{h}{R}(T-T_{\text{air}})&&\cr
\frac{\mathrm{d}^{2}T}{\mathrm{d}x^{2}}-\frac{2h}{\lambda R}T&=-\frac{2h}{\lambda R}T_{\text{air}}&&\cr
\end{align*}
$$

**Conditions aux limites:**
- $T(x=0)=T_{0}$
- Au bout de la tige, avec $L$ la longueur de la tige
$$
\begin{align*}
\phi(L^{-})&=\phi(L^{+})&&\cr
\phi(L^{-})&=j_{\text{th}}(L^{-})\pi R^{2}&&\cr
\phi(L^{+})&=j_{\text{cc}}\pi R^{2}&&\cr
j_{\text{th}}(L^{-})&=j_{\text{cc}}&&\cr
-\frac{\lambda \mathrm{d}T}{\mathrm{d}x}(L)&=h(T(L)-T_{\text{air}})&&\cr
\end{align*}
$$

Résolution, on pose
$$
\delta=\sqrt{ \frac{\lambda R}{2h} }
$$
Et on obtient
$$
\frac{\mathrm{d}^{2}T}{\mathrm{d}x^{2}}-\frac{1}{\delta^{2}}T=-\frac{1}{\delta^{2}}T_{\text{air}}
$$
Solution de l'équation caractéristique
$$
\begin{align*}
r^{2}-\frac{1}{\delta^{2}}r&=0&&\cr
r&=\pm\frac{1}{\delta}&&\cr
\end{align*}
$$
$$
\begin{align*}
T_{hom}&=Ae^{x/\delta}+Be^{-x/\delta}&&\cr
T_{par}&=T_{\text{air}}.&&\cr
\end{align*}
$$
Solution générale
$$
T(x)=Ae^{x/\delta}+Be^{-x/\delta}+T_{\text{air}}.
$$

**Résolution grâce aux conditions aux limites:**
$$
\begin{align*}
T(x=0)&=A+B+T_{\text{air}}=T_{0}&&\cr
-\lambda\left( \frac{A}{\delta}e^{L/\delta}-\frac{B}{\delta}e^{-L/\delta} \right)&=h(Ae^{L/\delta}+Be^{-L/\delta})&&\cr
\end{align*}
$$
Souvent, on a $L/\delta>>1$
Donc
$$
\begin{align*}
-\frac{\lambda}{\delta}Ae^{L/\delta}&=hAe^{L/\delta}&&\cr
A&=0&&\cr
\end{align*}
$$
Alors
$$
T(x)=(T_{0}-T_{\text{air}})e^{-x/\delta}+T_{\text{air}}.
$$


