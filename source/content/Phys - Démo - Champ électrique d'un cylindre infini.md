#todo : do the thing
**Énoncé:**

**Idée:**

**Démo:**
En coordonnée cylindrique:
$$
\rho(r)=\begin{cases}
\rho_{0}\text{ si }r<R \cr
0 \text{ sinon}
\end{cases}
$$
1. Symétries et invariances:
invariant:
- translation d'axe $z$
- translation dans le temps
- rotation d'angle $\theta$.
symétrie:
- Le plan de $\overrightarrow{OM}$ et $\overrightarrow{O_{z} }$.
- Le plan de $(M,\overrightarrow{e_{r} },\overrightarrow{e_{\theta} })$
Donc: $\overrightarrow{E(r)}=E(r)\overrightarrow{e_{r} }$.
1. Choix de la surface de Gauss
On choisit la surface du cylindre centrée en $O_{z}$, passant par $M$, de hauteur $H$.
$$
\begin{align*}
\oint \int_{S}\overrightarrow{E}\cdot \overrightarrow{dS}&=\iint_{\text{Haut} }\overrightarrow{E}\cdot \overrightarrow{dS}+\iint_{\text{Bas} }\overrightarrow{E}\cdot \overrightarrow{dS}+\iint_{\text{side} }\overrightarrow{E}\cdot \overrightarrow{dS}&&\cr
&=\iint_{\text{side} } E\times dS&&\cr
&=E(r)2\pi rH&&\cr
\end{align*}
$$
2. Application du th.
$$
\oint \int_{S}\overrightarrow{E}\cdot \overrightarrow{dS}=\frac{Q_{\text{int} } }{\varepsilon_{0} }
$$
- Si $r<R$:
$$
Q_{\text{int} }=\rho_{0}V=\rho_{0}\pi r^{2}H
$$
Donc:
$$
\begin{align*}
E(r)2\pi rH=&\frac{\rho_{0} \pi r^{2}H}{\varepsilon_{0} }&&\cr
\implies E(r)=&\frac{\rho_{0}r}{Z\varepsilon_{0} }&&\cr
\end{align*}
$$
- Si $r>R$:
$$
Q_{\text{int} }=\rho_{0}\pi R^{2}H
$$
Donc:
$$
\begin{align*}
E(r)2\pi rH=&\frac{\rho_{0}\pi R^{2}H}{\varepsilon_{0} }&&\cr
\implies E(r)=&\frac{\rho_{0}R^{2} }{2\varepsilon_{0}r}&&\cr
\end{align*}
$$

4. Calcul direct par Maxwell-Gauss
$$
\mathrm{div}\overrightarrow{E}=\frac{1}{r}\frac{ \partial  }{ \partial r } (rE(r))
$$
rq: $d\phi=\phi(r+dr)-\phi(r)$.
$\phi(r)=E(r)2\pi rH$
$\phi(r+dr)=E(r+dr)2\pi(r+dr)H$
$d\phi=2\pi \frac{d}{dr}(rE(r))H=(\mathrm{div}\overrightarrow{E})dV$
avec
$dV=2\pi rdrH=\pi(r+dr)^{2}H-\pi r^{2}H$
$\implies \mathrm{div}\overrightarrow{E}=\frac{1}{r}\frac{ \partial  }{ \partial r }(rE)$
Ensuite, on raisonne de même que précédemment, et on obtient des valeurs similaire, on choisit  notre origine des potentielles, et c'est tout bon...
(Je ne vais pas tout écrire, surtout si le prof dis que c'est pas tant obligatoire.)

5. Calcul du potentiel
$$
\overrightarrow{E}=-\overrightarrow{ \mathrm{grad} }V=-\frac{dV}{dr}\overrightarrow{e_{r} }
$$
- $r<R$:
$V(r)=-\frac{\rho_{0}r^{2} }{4\varepsilon_{0} }+K_{3}$
- $r>R$:
$V(r)=-\frac{\rho_{0}R^{3} }{2\varepsilon_{0} }+K_{4}$

Choix de l'origine des potentiels:
Dans le poly, $V(0)=0$
Ici, on choisit $V(r=R)=0$. Le choix n'a pas d'importance tant que ce n'est pas l'infini, qui diverge.
- $r<R$:
$-\frac{\rho_{0}R^{2} }{4\varepsilon_{0} }+K_{3}=0\implies V(r)=\frac{\rho_{0} }{4\varepsilon_{0} }(R^{2}-r^{2})$
- $r>R$:
$V(r)=-\frac{\rho_{0}R^{2} }{2\varepsilon_{0} }\ln\left( \frac{r}{R} \right)$

**Conséquence:**
