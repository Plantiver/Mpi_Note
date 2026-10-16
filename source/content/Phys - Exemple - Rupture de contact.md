#todo : clean this up
**Énoncé:**
On prend un pingouin sur un igloo.
à quel angle s'envole-t-il?
(sans vitesse initiale)
On néglige les frottements: $\overrightarrow{T}=\overrightarrow{0}$.

**Calcul:**
Système: {pingouin} modélisé par un point matériel
On se place dans le référentiel terrestre supposé galiléen.
On se place en coordonnée cylindrique.
Schéma:
![[Drawing 2026-10-16 10.44.30.excalidraw.svg]]
On considère:
- $\theta(t=0)=\theta_{0}$ petit

Bilan des forces:
- Le poids $\overrightarrow{P}=mg(-\cos\theta\overrightarrow{e_{r}}+\sin\theta \overrightarrow{e_{\theta}})$
- Réaction normale $\overrightarrow{N}=N\overrightarrow{e_{r}}$

**2nde loi de Newton**
$$
\begin{align*}
m\overrightarrow{a}&=\overrightarrow{P}+\overrightarrow{N}&&\cr
m\begin{pmatrix}
-r\dot{\theta}^{2} \\
r \ddot{\theta} \\
0
\end{pmatrix}&=\begin{pmatrix}
-mg\cos\theta \\
mg\sin\theta \\
0
\end{pmatrix}+\begin{pmatrix}
N \\
0 \\
0
\end{pmatrix}&&\cr
\end{align*}
$$
Ainsi:
$$
N=m(g\cos\theta-R\dot{\theta}^{2})
$$
et
$$
\begin{align*}
\ddot{\theta}&=\frac{g}{R}\sin\theta &&\cr
\dot{\theta}\ddot{\theta}&=\frac{g}{R}\dot{\theta}\sin\theta &&\cr
\frac{d}{dt} \left( \frac{1}{2}\dot{\theta}^{2} \right)&=\frac{d}{dt} \left( -\frac{g}{R}\cos\theta \right)&&\cr
\frac{1}{2}\dot{\theta}^{2}-\frac{1}{2}\dot{\theta}^{2}(0)&=-\frac{g}{R}(\cos\theta-\cos\theta_{0})&&\cr
\end{align*}
$$
On rappelle que la vitesse initiale est nulle.
Ainsi:
$$
N=m(g\cos\theta-2g(\cos\theta-\cos\theta_{0}))=mg(3\cos\theta-2\cos\theta_{0})
$$
Ainsi, le pingouin décolle pour:
$$
\begin{align*}
\cos\theta_{l}&=\frac{2}{3}\cos\theta_{0}&&\cr
\theta_{l}&=\mathrm{arcos}\left( \frac{2}{3}\cos\theta_{0} \right)&&\cr
\end{align*}
$$









