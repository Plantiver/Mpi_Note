**Énoncé:**
On s'intéresse à une sphère chargée uniformément, de centre $O$, de rayon $R$, et de densité de charge $\rho_{0}$.
On place un point $M(r,\theta,\varphi)$, et l'on cherche l'expression de $\overrightarrow{E}(M,t)$ ainsi que de $V(M,t)$.

**Idée:**
On applique la méthode et on l'apprends

**Démo:**
1. Invariance et symétrie
- Toute translation de $t$ laisse $\overrightarrow{E}(M,t)$ inchangé
- Toute rotation de $\theta$ laisse $\overrightarrow{E}(M,t)$ inchangé
- Toute rotation de $\varphi$ laisse $\overrightarrow{E}(M,t)$ inchangé
Donc: $\overrightarrow{E}(M,t)=\overrightarrow{E}(r)$.
- Tout plan contenant $\overrightarrow{OM}$ est un plan de symétrie
- Ainsi, $\overrightarrow{E}\in(OM)$
Finalement: $\overrightarrow{E}(M,t)=E(r)\overrightarrow{e_{r} }.$


2. Choix de la surface de Gauss
On prend la sphère de centre $O$ et de rayon $r$.
Ainsi:
$$
\begin{align*}
\phi&=\oint \int_{S}\overrightarrow{E}\cdot \overrightarrow{\mathrm{d}S}&&\cr
&=\iint_{S}E(r)\mathrm{d}S&&\cr
&=E(r)\iint_{S}\mathrm{d}S&&\cr
&=E(r)4\pi r^{2}&&\cr
\end{align*}
$$

3. Application du théorème de Gauss
$$
\phi=\frac{Q_{\text{int} } }{\varepsilon_{0} }
$$
- Si $r<R$:
$$
\begin{align*}
Q_{\text{int} }&=\iiint_{V}\rho_{0}\mathrm{d}V&&\cr
&=\frac{4}{3}\pi r^{3}\rho_{0}&&\cr
\end{align*}
$$
D'où:
$$
\begin{align*}
E(r)4\pi r^{2}=&\frac{4}{3}\pi r^{3}\frac{\rho_{0} }{\varepsilon_{0} }&&\cr
\;\implies\;E(r)=&\frac{r\rho_{0} }{3\varepsilon_{0} }&&\cr
\end{align*}
$$

- Si $r>R$:
$$
\begin{align*}
Q_{\text{int} }&=\iiint_{V}\rho_{0}\mathrm{d}V&&\cr
&=\frac{4}{3}\pi R^{3}\rho_{0}&&\cr
&=Q_{\text{total} }&&\cr
\end{align*}
$$
D'où:
$$
\begin{align*}
E(r)4\pi r^{2}&=\frac{Q_{\text{total} } }{\varepsilon_{0} }&&\cr
\;\implies\;E(r)&=\frac{Q_{\text{total} } }{4\pi\varepsilon_{0}r^{2} }&&\cr
\end{align*}
$$
4. Calcul du potentiel
Par définition:
$$
\overrightarrow{E}=-\overrightarrow{ \mathrm{grad} }V
$$
Donc, ici:
$$
E(r)\overrightarrow{e_{r} }=-\frac{\mathrm{d}V}{\mathrm{d}r}\overrightarrow{e_{r} }
$$

- Si $r<R$:
$$
\begin{align*}
\frac{r\rho_{0} }{3\varepsilon_{0} }&=-\frac{\mathrm{d}V}{\mathrm{d}r}&&\cr
V(r)&=-\frac{\rho_{0}r^{2} }{6\varepsilon_{0} }+K_{1}&&\cr
\end{align*}
$$
- Si $r>R$:
$$
\begin{align*}
\frac{Q_{\text{total} } }{4\pi\varepsilon_{0}r^{2} }&=-\frac{\mathrm{d}V}{\mathrm{d}r}&&\cr
V(r)&=\frac{Q_{\text{total} } }{4\pi\varepsilon_{0}r}+K_{2}&&\cr
\end{align*}
$$
En choisissant l'origine des potentiels à l'$\infty$, ainsi $K_{2}=0$.
De plus, par continuité de $V$, on a:
$$
\begin{align*}
V(R)=-\frac{\rho_{0}R^{2} }{6\varepsilon_{0} }+K_{1}&=\frac{Q_{\text{total} } }{4\pi\varepsilon_{0}R}&&\cr
K_{1}&=\frac{4\pi R^{3}\rho_{0} }{4\pi\varepsilon_{0}R}+\frac{\rho_{0}R^{2} }{6\varepsilon_{0} }&&\cr
K_{1}&=\frac{7}{6}\cdot \frac{R^{2}\rho_{0} }{\varepsilon_{0} }&&\cr
\end{align*}
$$

**Conséquence:**
Si l'on se place à l'extérieur de la sphère, on obtient la même chose que pour une particule.
Ainsi, toute les "approximations" faites en première année, de considérer des objets comme des particules n'en sont pas pour l'expression des forces électrique et gravitationnelle.




