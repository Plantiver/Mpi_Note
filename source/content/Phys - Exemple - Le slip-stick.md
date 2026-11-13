On se place dans le référentiel terrestre supposé galiléen.
On considère une masse $m$ accroché à un mur par un ressort $(l_{0},k)$, et posée sur un tapis roulant de vitesse horizontale $\overrightarrow{v_{0}}$ fixe qui éloigne la masse de son attache.
On considérera les forces de frottements, et l'on donne $f_{d}=0$.
Décrire le mouvement de la masse.
Schéma:
![[Phys - Exemple - Le slip-stick 2026-11-13 15.29.27.excalidraw.svg]]

On décomposera le mouvement en deux phases, une phase ou la masse est entraînée par le tapis, et une phase ou elle glisse jusqu'à revenir à une position initiale, et l'on détaillera les conditions de changement de phase.

Bilan des forces:
- $\overrightarrow{P}=m\overrightarrow{g}$
- $\overrightarrow{R_{N}}=R_{N}\overrightarrow{u_{y}}$
- $\overrightarrow{R_{T}}=R_{T}\overrightarrow{u_{x}}$
- $\overrightarrow{F_{r}}=-k(l-l_{0})\overrightarrow{u_{x}}$

1. 
$$
x(t)=v_{0}t
$$
Donc
$$
\overrightarrow{R}+\overrightarrow{T}+\overrightarrow{P}+\overrightarrow{N}=0
$$
Vu statique
$$
\begin{align*}
T&\leq f_{s}N&&\cr
kx&\leq f_{s}mg&&\cr
x&\leq f_{s}\frac{mg}{k}=x_{max}&&\cr
\end{align*}
$$
2. 
On dépasse $x_{max}$.
Donc $T=0$ et ainsi
$$
m\ddot{x}=-kx
$$
Et ainsi
$$
\ddot{x}+\omega^{2}x=0
$$
avec $\omega_{0}=\sqrt{ \frac{k}{m} }$.
Avec les conditions initiales $\begin{cases}x(0)&=x_{max} \\  \dot{x}(0)&=v_{0}\end{cases}$
$$
x(t)=x_{max}\cos(\omega t)+\frac{v_{0}}{\omega}\sin(\omega t).
$$

3. 
La phase dynamique s'arrète si:
$$
\begin{cases}
x<x_{max} \\
\dot{x}=v_{0}
\end{cases}
$$
4. 
Joli schéma, que je ne vais pas refaire, pour des raisons...






