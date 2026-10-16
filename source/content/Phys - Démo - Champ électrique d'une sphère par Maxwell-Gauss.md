#todo : do the thing
**Énoncé:**

**Idée:**

**Démo:**


**Autres méthode:** calcul direct par Maxwell-Gauss.
En sphérique:
![[Phys - Math#Divergence en sphérique]]

Or $\overrightarrow{E}=E(r)\overrightarrow{e_{r} }$
$\implies \mathrm{div}\overrightarrow{E}=\frac{1}{r^{2} }\frac{ \partial r^{2}E_{r} }{ \partial r }$

En symétrie sphérique, calculons le flux sortant d'une coquille sphérique de rayon $r$ et d'épaisseur $\mathrm{d}r$.

Flux entrant en $r$: $\phi(r)=4\pi r^{2}E(r)$
Flux sortant en $r+\mathrm{d}r$: $\phi(r+\mathrm{d}r)=4\pi(r+\mathrm{d}r)^{2}E(r+\mathrm{d}r)$.

En posant: $f(r)=r^{2}E(r)$:
$\implies d\phi=4\pi \frac{df}{dr}dr$
Mais $d\phi=(\mathrm{div}\overrightarrow{E})dV$.
$dV=4\pi r^{2}dr$.

Mais
$$
d\phi=4\pi \frac{d}{dr} (r^{2}R)dr
$$
et
$$
d\phi=\mathrm{div}\overrightarrow{E}dV=\mathrm{div}\overrightarrow{E}4\pi r^{2}dr
$$
Donc:
$$
\mathrm{div}\overrightarrow{E}=\frac{1}{r^{2} }\frac{ \partial  }{ \partial r } (r^{2}E)
$$
*D'après Maxwell-Gauss:*
$$
\mathrm{div}\overrightarrow{E}=\frac{\rho(r)}{\varepsilon_{0} }
$$
- Si $r<R$:
$\rho(r)=\rho_{0}$
$$
\begin{align*}
\frac{1}{r^{2} }\frac{ \partial  }{ \partial r } (r^{2}E)=&\frac{\rho_{0} }{\varepsilon_{0} }&&\cr
\frac{ \partial  }{ \partial r } (r^{2}E)=&\frac{\rho_{0}r^{2} }{\varepsilon_{0} }&&\cr
r^{2}E=&\frac{\rho_{0}r^{3} }{3\varepsilon_{0} }+K_{1}&&\cr
\end{align*}
$$
En $r=0$, $\overrightarrow{E}$ appartient à tout les plans de symétrie, donc $\overrightarrow{E(0)}=\overrightarrow{0}$.
Donc $K_{1}=0$.
D'où, si $r<R$:
$$
E(r)=\frac{\rho r}{3\varepsilon_{0} }
$$
- Si $r>R$:
$$
\begin{align*}
\rho(r)=&0&&\cr
\mathrm{div}\overrightarrow{E}=&0&&\cr
\frac{ \partial  }{ \partial r } (r^{2}E)=&0&&\cr
E=&\frac{K_{2} }{r^{2} }&&\cr
\end{align*}
$$
$E$ est continue, étant solution d'une équation différentielle:
$E(R^{+})=E(R^{-})$
$$
K_{2}=\frac{\rho_{0}R^{3} }{3\varepsilon_{0} }
$$
$$
\begin{align*}
E(r)=&\frac{1}{r^{2} }\int_{0}^{r}\frac{\rho(u)u^{2} }{\varepsilon_{0} }du&&\cr
\end{align*}
$$
**Calcul du potentiel électrostatique**
$$
\overrightarrow{E}=-\overrightarrow{ \mathrm{grad} }V=-\frac{dV}{dr}\overrightarrow{e_{r} }
$$

- Si $r<R$:
$$
\begin{align*}
E=&\frac{r\rho_{0} }{3\varepsilon_{0} }&&\cr
\implies \frac{dV}{dr}=&-\frac{r\rho_{0} }{3\varepsilon_{0} }&&\cr
\implies V(r)=&-\frac{\rho_{0}r^{2} }{6\varepsilon_{0} }+K_{3}&&\cr
\end{align*}
$$
- Si $r>R$:
$$
V(r)=\frac{\rho_{0}R^{3} }{3\varepsilon_{0}r}+K_{4}
$$
On CHOISIT de prendre l'origine des potentiels en $+\infty$.
Donc $K_{4}=0$
... calculs
$K_{2}=\frac{1}{2}\frac{\rho_{0}R^{2} }{\varepsilon_{0} }$
... schémas



**Conséquence:**
