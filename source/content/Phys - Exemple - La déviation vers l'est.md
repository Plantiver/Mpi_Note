Voir le contexte dans [[Phys - M1 - Compléments de mécanique#4 - Dynamique dans le référentiel terrestre]].

On se place en coordonnée cartésiennes
On lâche une balle sans vitesse initiale en chute libre.
La force d'inertie d'entrainement est intégrée au poids.
$$
m\overrightarrow{a}=m\overrightarrow{g}+\overrightarrow{F_{ic}}
$$
avec $\overrightarrow{F}_{ic}=-m\overrightarrow{a_{c}}=-2m\overrightarrow{\Omega}\wedge \overrightarrow{v_{r}}$.

Schema de la situation avec $\lambda$ la colongitude.

Rappel:
$$
\begin{align*}
g&\sim 10m\cdot s^{-2}&&\cr
\Omega&\sim 7\times 10^{-5}rad\cdot s^{-1}&&\cr
\end{align*}
$$
Donc, pour avoir:
$$
\begin{align*}
2\Omega v&\sim g&&\cr
v&\sim 10^{5}m\cdot s^{-1}&&\cr
\end{align*}
$$
Ainsi, $\overrightarrow{F_{ic}}$ est négligeable devant le poids pour des vitesses faibles.
Ainsi,
$$
\begin{align*}
m\overrightarrow{a}&=m\overrightarrow{g}&&\cr
\overrightarrow{v}&=-gt\overrightarrow{e_{x}}&&\cr
\end{align*}
$$
Donc on peut calculer Coriolis avec cette expression:
$$
\begin{align*}
\overrightarrow{\Omega}&=\Omega_{T}(-\cos\lambda \overrightarrow{e_{x}}+\sin\lambda \overrightarrow{e_{z}})&&\cr
\overrightarrow{\Omega}\wedge \overrightarrow{v}&=\Omega_{T}(-\cos\lambda \overrightarrow{e_{x}}+\sin\lambda \overrightarrow{e_{z}})\wedge(-gt\overrightarrow{e_{z}})&&\cr
&=\Omega_{T}\cos\lambda gt\overrightarrow{e_{x}}\wedge \overrightarrow{e_{z}}&&\cr
&=-\Omega_{T}\cos\lambda gt\overrightarrow{e_{y}}&&\cr
\end{align*}
$$
Donc
$$
\overrightarrow{F_{ic}}=2m\Omega_{T}\cos\lambda gt\overrightarrow{e_{y}}.
$$
Donc, la deuxième loi de Newton devient
$$
m\overrightarrow{a}=-g\overrightarrow{e_{z}}+2m\Omega_{T}\cos\lambda gt\overrightarrow{e_{y}}
$$
Projection sur $\overrightarrow{e_{y}}$:
$$
\begin{align*}
\ddot{y}&=2\Omega_{T}\cos\lambda gt &&\cr
\dot{y}&=2\Omega_{T}\cos\lambda g\frac{t^{2}}{2}+\dot{y_{0}}&&\cr
y&=\Omega_{T}\cos\lambda g\frac{t^{3}}{3}+y_{0}&&\cr
\end{align*}
$$

### Hors programme, calcul explicite
#hp 
$$
\begin{align*}
m\overrightarrow{a}&=-mg\overrightarrow{e_{z}}+\overrightarrow{F_{ic}}&&\cr
\overrightarrow{\Omega}&=\Omega_{T}(-\cos\lambda \overrightarrow{e_{x}}+\sin\lambda \overrightarrow{e_{z}})&&\cr
\overrightarrow{v}&=\dot{x}\overrightarrow{e_{x}}+\dot{y}\overrightarrow{e_{y}}+z\overrightarrow{e_{z}}&&\cr
\overrightarrow{\Omega}\wedge \overrightarrow{v}&=&&\cr
xyzxy&=\Omega_{T}(-\cos\lambda(\dot{y}\overrightarrow{e_{z}}-\dot{z}\overrightarrow{e_{y}})+\sin\lambda(\dot{x}\overrightarrow{e_{y}}-\dot{y}\overrightarrow{e_{x}}))&&\cr
\end{align*}
$$
Donc
$$
\begin{align*}
\overrightarrow{F_{ic}}&=-2m\overrightarrow{\Omega}\wedge \overrightarrow{v}&&\cr
&=-2m\Omega_{T}\begin{pmatrix}
-\dot{y}\sin\lambda \\
\dot{z}\cos\lambda+\dot{x}\sin\lambda \\
-\dot{y}\cos\lambda
\end{pmatrix}&&\cr
\end{align*}
$$
La deuxième loi de Newton nous donne:
$$
\begin{align*}
m\begin{pmatrix}
\ddot{x} \\
\ddot{y} \\
\ddot{z}
\end{pmatrix}&=-m\begin{pmatrix}
0 \\
0 \\
g
\end{pmatrix}-2m\Omega_{T}\begin{pmatrix}
-\dot{y}\sin\lambda \\
\dot{z}\cos\lambda+\dot{x}\sin\lambda \\
-\dot{y}\cos\lambda
\end{pmatrix}&&\cr
\end{align*}
$$
Dérivons l'équation en $y$:
$$
\begin{align*}
\ddot{y}&=-2\Omega_{T}(\cos\lambda \dot{z}+\sin\lambda \dot{x})&&\cr
\ddot{\dot{y}}&=-2\Omega_{T}(\cos\lambda \ddot{z}+\sin\lambda \ddot{x})&&\cr
&=-2\Omega_{T}\left[ \cos\lambda(-g+2\Omega_{T}\cos\lambda \dot{y})+\sin\lambda2\Omega_{T}\sin\lambda \dot{y} \right] &&\cr
&=2\Omega_{T}\cos\lambda g-4\Omega_{T}^{2}(\cos ^{2}\lambda+\sin ^{2}\lambda)\dot{y}&&\cr
\dot{\ddot{y}}+4\Omega_{T}^{2}\dot{y}&=2\Omega_{T}\cos\lambda g&&\cr
\end{align*}
$$
Un oscillateur harmonique:
$$
\begin{align*}
\dot{y}(t)&=A\cos(2\Omega_{T}t)+B\sin(2\Omega_{T}t)+\frac{\cos\lambda g}{2\Omega t}&&\cr
&=\frac{\cos\lambda g}{2\Omega_{T}}(1-\cos(2\Omega_{T}t))&&\cr
y(t)&=\frac{\cos\lambda g}{2\Omega_{T}}\left( t-\frac{1}{2\Omega_{T}}\sin(2\Omega_{T}t) \right)+y_{0}&&\cr
\end{align*}
$$
En faisant un DL3, on retrouve l'expression de tout à l'heure.

Bon... Merci Robin...