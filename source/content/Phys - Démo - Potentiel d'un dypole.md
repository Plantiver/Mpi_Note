**Énoncé:**
Soit $P$ et $N$ deux particules de charge respective $+q$ et $-q$. On place L'origine du repère en $O$ à mi-chemin entre $P$ et $N$.
Ainsi, $P$ et $N$ forme le dipole $\overrightarrow{p}=q\overrightarrow{NP}$.
On s'intéresse au potentiel électrique en $M$, un point placé à une distance $r$ de $O$.
De plus, on note $\theta$ l'angle entre $\overrightarrow{OP}$ et $\overrightarrow{OM}$.
Enfin, on considère $r$ grand devant la taille du système.

**Idée:**
On divise le calcul sur chaque particule, puis avec un peu de géométrie et un développement limité, on obtient le résultat voulu.

**Démo:**
On notera $a=\|\overrightarrow{OP}\|=\|\overrightarrow{ON}\|$.
$$
\begin{align*}
V(M)&\underset{ \text{superposition} }{ = } V_{P}(M)+V_{N}(M)&&\cr
&\underset{ V }{ \hat{=} }\frac{q}{4\pi\varepsilon_{0}}\left( \frac{1}{\|\overrightarrow{PM}\|}-\frac{1}{\|\overrightarrow{NM}\|} \right)&&\cr
&=\frac{q}{4\pi\varepsilon_{0}}((\|\overrightarrow{PM}\|^{2})^{-1/2}-(\|\overrightarrow{NM}\|^{2})^{-1/2})&&\cr
&\underset{ \text{Al Kashi} }{ = }\frac{q}{4\pi\varepsilon_{0}}((r^{2}+a^{2}-2ar\cos\theta)^{-1/2}-(r^{2}+a^{2}+2ar\cos\theta)^{-1/2})&&\cr
&=\frac{q}{4\pi\varepsilon_{0}r}\left( \left( 1+\left( \frac{a}{r} \right)^{2}-2\left( \frac{a}{r} \right)\cos\theta \right)^{-1/2}-\left( 1+\left( \frac{a}{r} \right)^{2}+2\left( \frac{a}{r} \right)\cos\theta \right)^{-1/2} \right)&&\cr
&\underset{ DL_{1}\left( \frac{a}{r} \right) }{ = }\frac{q}{4\pi\varepsilon_{0}r}\left( \left( 1+\left( \frac{a}{r} \right)\cos\theta \right)-\left( 1-\left( \frac{a}{r}\cos\theta \right) \right) \right)&&\cr
&=\frac{q}{4\pi\varepsilon_{0}r}\cdot\left( \frac{a}{r} \right)\cos\theta.&&\cr
\end{align*}
$$

**Conséquence:**
Ainsi, on observe bien que pour une distance suffisante, un dipôle peut être considéré comme une masse sans charges.
Cela permet de ne pas avoir à considérer le potentiel électrique de la matière si l'on s'en éloigne suffisament.