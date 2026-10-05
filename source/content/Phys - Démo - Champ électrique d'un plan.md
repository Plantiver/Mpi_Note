**Énoncé:**
On s'intéresse au plan $(O,\overrightarrow{e_{x} }, \overrightarrow{e_{y} })$ de charge surfacique uniforme $\sigma_{0}$.
On place un point $M=(x,y,z)$, et l'on cherche à exprimer $\overrightarrow{E}(M,t)$ et $V(M,t)$.

**Idée:**
On applique la méthode et on l'apprends.

**Démo:**
1. Invariance et symétrie
- Toute translation de $t$ laisse $\overrightarrow{E}(M,t)$ inchangé
- Toute translation de $x$ laisse $\overrightarrow{E}(M,t)$ inchangé
- Toute translation de $y$ laisse $\overrightarrow{E}(M,t)$ inchangé
Donc $\overrightarrow{E}(M,t)=\overrightarrow{E}(z)$.
- Tout plan contenant $\overrightarrow{MM'}$ est un plan de symétrie (avec $M'$ le projeté orthogonal de $M$ sur le plan)
- Ainsi, $\overrightarrow{E}\in(MM')$.
Finalement: $\overrightarrow{E}(M,t)=E(z)\overrightarrow{e_{z} }$.
De plus, il y a une symétrie globale par le plan considéré.
Donc $E(-z)=-E(z)$.


2. Choix de la surface de Gauss
On prends un cylindre orientée selon $\overrightarrow{e_{z} }$, de hauteur $2z$, et coupée en son milieu par notre surface.
$$
\begin{align*}
\phi_{S}&=\oint \int_{S}\overrightarrow{E}\cdot \overrightarrow{\mathrm{d}S}&&\cr
&=\iint_{S,\text{Haut} }\overrightarrow{E}\cdot \overrightarrow{\mathrm{d}S}+\iint_{S,\text{Bas} }\overrightarrow{E}\cdot \overrightarrow{\mathrm{d}S}+\iint_{S,\text{Side} }\overrightarrow{E}\cdot \overrightarrow{\mathrm{d}S}&&\cr
&=\iint_{S,\text{Haut} }E\mathrm{d}S+\iint_{S,\text{Bas} }-E\mathrm{d}S&&\cr
&=E(z)2\pi R^{2}-E(-z)2\pi R^{2}&&\cr
&=E(z)4\pi R^{2}&&\cr
\end{align*}
$$


3. Application du théorème
D'après le théorème de Gauss
$$
\phi_{S}=\frac{Q_{\text{int} } }{\varepsilon_{0} }.
$$
Or, $Q_{\text{int} }=\sigma_{0}2\pi R^{2}$.
D'où:
$$
\begin{align*}
E(z)4\pi R^{2}&=\frac{\sigma_{02}\pi R^{2} }{\varepsilon_{0} }&&\cr
E(z)&=\frac{\sigma_{0} }{2\varepsilon_{0} }.&&\cr
\end{align*}
$$
On retrouve que:
$$
\overrightarrow{E} = \begin{cases}
\frac{\sigma_{0} }{2\varepsilon_{0} }\overrightarrow{e_{z} }&\text{ si }z>0 \cr
-\frac{\sigma_{0} }{2\varepsilon_{0} }\overrightarrow{e_{z} }&\text{ si }z<0
\end{cases}
$$

4. Calcul du potentiel
On a:
$$
\begin{align*}
\overrightarrow{E}&=-\overrightarrow{ \mathrm{grad} }V&&\cr
&-\frac{\mathrm{d}V}{\mathrm{d}z}\overrightarrow{e_{z} }.&&\cr
\end{align*}
$$
- Si $z<0$:
$$
V(z) = \frac{\sigma_{0}z}{2\varepsilon_{0} }+K_{+}
$$
- Si $z>0$:
$$
V(z)=-\frac{\sigma_{0}z}{2\varepsilon_{0} }+K_{-}
$$
En prenant l'origine des potentielles sur le plan, on trouve:
$$
V(z) = \mathrm{si}(z)\cdot\frac{\sigma_{0}z}{2\varepsilon_{0} }.
$$

**Conséquence:**
Voir le modèle du condensateur plan.