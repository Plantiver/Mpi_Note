# Énoncé
On considère une surface plane en $x=0$ et l'on considère cette plaque chauffée de manière régulière, ainsi on a
$$
T(x=0,t)=T_{0}+a\cos(\omega t).
$$
On cherche a exprimer $T(x,t)$ pour tout $x<0$.

schéma #todo 
# Idée

# Démo
On se place en cartésien

On doit résoudre 
$$
\frac{ \partial T }{ \partial t } =D \frac{ \partial^{2}T }{ \partial x^{2} } .
$$
On cherche une solution de la forme 
$$
T(x,t)=T_{0}+\mathrm{Re}(af(x)e^{j\omega t}).
$$
Cette forme est cohérente avec
- la donnée initiale sinusoïdale
- apparition d'un retard de propagation de l'ordre thermique.

On pose
$$
\underline{T}(x,t)=a \underline{f}(x)e^{j\omega t}.
$$
On a donc
$$
\begin{align*}
\frac{ \partial \underline{T} }{ \partial t } &j\omega a \underline{f}e^{j\omega t}&&\cr
\frac{ \partial^{2} \underline{T} }{ \partial x^{2} } &=a \underline{f}''e^{j\omega t}&&\cr
\end{align*}
$$
On applique l'équation de la chaleur
$$
\begin{align*}
j\omega a \underline{f}e^{j\omega t}&Da \underline{f}''e^{j\omega t}&&\cr
\underline{f}''-j \frac{\omega}{D} \underline{f}&=0&&\cr
\end{align*}
$$
On résout par l'équation caractéristique
$$
\begin{align*}
r^{2}-j \frac{\omega}{D}r&=0&&\cr
r^{2}&=j \frac{\omega}{D}&&\cr
r&=\pm \sqrt{ \frac{\omega}{D} }e^{j \pi/4}&&\cr
r&=\pm(1+j)\sqrt{ \frac{\omega}{2D} }&&\cr
\end{align*}
$$
Donc
$$
\begin{align*}
\underline{f}(x)&=\underline{A}e^{(1+j)\sqrt{ \omega/2D }x}+\underline{B}e^{-(1+j)\sqrt{ \omega/2D }x}&&\cr
\end{align*}
$$
En $x=0$, on a $\underline{f}(x)=1$, donc
$$
\underline{A}+\underline{B}=1
$$
Et, on a nécessairement $\underline{A}=0$, sinon lorsqu'on s'enfonce dans le sol ($x\nearrow$) la température augmenterais (ce qui est impossible physiquement).

Donc
$$
\underline{f}(x)=e^{-(1+j)\sqrt{ \omega/2D }x}.
$$
On va poser l'épaisseur de peau
$$
\delta(\omega)=\sqrt{ \frac{2D}{\omega} }.
$$
Ainsi
$$
\underline{f}(x)=e^{-(1+j)x/\delta}.
$$
On revient à la température
$$
\begin{align*}
T(x,t)&=T_{0}+\mathrm{Re}(ae^{-(1+j)x/\delta}e^{j\omega t})&&\cr
&=T_{0}+ae^{-x/\delta}\mathrm{Re}(e^{j(\omega t-x/\delta)})&&\cr
&=T_{0}+ae^{-x/\delta}\cos\left( \omega t-\frac{x}{\delta} \right).&&\cr
\end{align*}
$$
Il s'agit d'une onde exponentiellement amortie.
Joli dessin du tracé de la fonction.

**Rq:**
- $\frac{x}{\delta}$ traduit le déphasage.
- Il s'agit d'une onde progressive qui se propage à la vitesse de phase $v_{\phi}=\omega\delta\left( =\frac{\omega}{k} \right)$. (pour $k$, voir [[Phys - EM5 - Le champ électromagnétique]]).

**Rq importante:**
$\delta$, l'épaisseur de peau, c'est la taille caractéristique de pénétration.
Si on fait le calcul, on obtient que les variations annuelles sont ressenties plus en profondeur que celle de la journée.

# Conséquence
