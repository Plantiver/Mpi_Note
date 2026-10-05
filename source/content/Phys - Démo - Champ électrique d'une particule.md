**Énoncé:**
On s'intéresse à une particule de charge $q$ placée en $O$.
On place un point $M(r,\theta,\varphi)$, et l'on cherche l'expression de $\overrightarrow{E}(M,t)$ ainsi que de $V(M,t)$.

**Idée:**
On applique la méthode et on l'apprends.

**Démo:**
1. Invariance et symétrie
- Toute translation de $t$ laisse $\overrightarrow{E}(M,t)$ inchangé
- Toute rotation de $\theta$ laisse $\overrightarrow{E}(M,t)$ inchangé
- Toute rotation de $\varphi$ laisse $\overrightarrow{E}(M,t)$ inchangé
Donc: $\overrightarrow{E}(M,t)=\overrightarrow{E}(r)$.
- Tout plan contenant $\overrightarrow{OM}$ est un plan de symétrie
- Ainsi, $\overrightarrow{E}\in(OM)$
Finalement: $\overrightarrow{E}(M,t)=E(r)\overrightarrow{e_{r}}.$


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
\phi=\frac{Q_{\text{int}}}{\varepsilon_{0}}
$$
Ici, $Q_{\text{int}}=q$.
D'où:
$$
\begin{align*}
E(r)4\pi r^{2}&=\frac{q}{\varepsilon_{0}}&&\cr
E(r)&=\frac{q}{4\pi\varepsilon_{0}r^{2}}&&\cr
\end{align*}
$$
4. Calcul du potentiel
Par définition:
$$
\overrightarrow{E}=-\overrightarrow{ \mathrm{grad}}V
$$
Donc, ici:
$$
E(r)\overrightarrow{e_{r}}=-\frac{\mathrm{d}V}{\mathrm{d}r}\overrightarrow{e_{r}}
$$
D'où:
$$
\begin{align*}
E(r)&=-\frac{\mathrm{d}V}{\mathrm{d}r}&&\cr
V(r)&=\frac{q}{4\pi \varepsilon_{0}r}+K&&\cr
\end{align*}
$$
En choisissant l'origine des potentiels à l'$\infty$, on a $K=0$.

**Conséquence:**
Par superposition, on pourra donc calculer le champs de tout ensemble de particules.
Pratique.