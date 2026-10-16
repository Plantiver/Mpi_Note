#todo : clean this up
Hypothèse: $f=f_{s}=f_{d}$.
1. Hypothèse de glissement
La phase statique s'arrête quand $\|\overrightarrow{T}\|\leq f\|\overrightarrow{N}\|$ n'est plus respecté.
La phase de glissement s'arrête si (l'une est l'autre)
- $\overrightarrow{v}=\overrightarrow{0}$
- $\|\overrightarrow{T}\|\leq f\cdot\|\overrightarrow{N}\|$ peut être respectée.

2. L'équilibre
Système: {Solide sur un plan incliné} modélisé par un point
Référentiel: Terrestre supposé galiléen
Coordonnées: cartésiennes
![[Drawing 2026-10-16 11.17.45.excalidraw]]
Bilan des forces:
- $\overrightarrow{N}=N\overrightarrow{e_{y}}$
- $\overrightarrow{T}=-T\overrightarrow{e_{x}}$
- $\overrightarrow{P}=mg(\sin\theta \overrightarrow{e_{x}}-\cos\theta\overrightarrow{e_{y}})$
2nde loi de Newton
En statique ($\overrightarrow{v}=\overrightarrow{0},\;\overrightarrow{a}=\overrightarrow{0}$):
$$
\begin{cases}
N=mg\cos\theta \\
T=mg\sin\theta
\end{cases}
$$
Hypothèse de coulomb:
$$
\frac{T}{N}<f
$$
Ainsi:
$$
\boxed{\tan\theta<f}
$$
On pose $\theta_{l}$ tq:
$$
\tan\theta_{l}=f
$$
Et donc, on est en statique tant que:
$$
\theta<\theta_{l}
$$
3. La mise en mouvement
Même situation qu'avant MAIS $\theta>\theta_{l}$.
La phase statique est impossible.
On pose $\overrightarrow{a}=\ddot{x}\overrightarrow{e_{x}}$.
On a toujours:
$$
\begin{cases}
N&=mg\cos\theta \\
m\ddot{x}&=-T+mg\sin\theta
\end{cases}
$$
Loi de coulomb:
$$
\begin{align*}
T&=fN&&\cr
&=fmg\cos\theta&&\cr
\end{align*}
$$
Ainsi:
$$
\begin{align*}
m\ddot{x}&=-fmg\cos\theta+mg\sin\theta &&\cr
\ddot{x}&=g\cos\theta(\tan\theta-f):=a_{0}&&\cr
\end{align*}
$$
Ainsi, on a bien $a_{0}>0$ car $\tan\theta>f$, c'est cohérent, le solide descend

4. Lancer vers le haut
$\theta$ quelconque mais $\overrightarrow{v_{0}}=-v_{0}\overrightarrow{e_{x}}$.
C'est en dynamique parce que l'objet est mis en mouvement
![[Drawing 2026-10-16 11.37.27.excalidraw]]
Bilan des forces:
- $\overrightarrow{N}=N\overrightarrow{e_{y}}$
- $\overrightarrow{T}=T\overrightarrow{e_{x}}$
- $\overrightarrow{P}=mg(-\cos\theta h\overrightarrow{e_{y}}+\sin\theta h\overrightarrow{e_{x}})$

2nde loi de newton:
$$
\begin{cases}
m\ddot{x}&=T+mg\sin\theta \\
0&=N-mg\cos\theta
\end{cases}
$$
Loi de coulomb:
$$
\begin{align*}
T&=f\cdot N&&\cr
&fmg\cos\theta&&\cr
\end{align*}
$$
Ainsi:
$$
\ddot{x}=g(\sin\theta+f\cos\theta)=a_{1},\;cst
$$


Mais $x(0)=0$ et $\dot{x}(0)=-v_{0}<0$
Ainsi, en intégrant deux fois et en simplifiant les constantes #todo 
$x(t)=\frac{1}{2}a_{1}t^{2}-v_{0}t$
Le solide s'arrête lorsque $\dot{x}=0$, quand $t=\frac{v_{0}}{a_{1}}$.
Et donc $x_{t_{\text{arr}}}=-\frac{1}{2}\frac{v_{0}^{2}}{a_{1}}$
Et, on s'arrête si $\theta<\theta_{l}$.

















