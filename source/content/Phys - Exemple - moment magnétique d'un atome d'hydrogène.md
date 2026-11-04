#todo : clean up this mess
On prend un atome d'hydrogène:
- noyau: 1 proton de masse $m_{p}$
- 1 electron qui gravite autour (mécanique classique) de masse $m_{e}=\frac{m_{p}}{2000}$
Approximation de Born-Oppenheimer:
$$
\begin{align*}
m_{e}\overrightarrow{a_{e}}&=\overrightarrow{F}_{p\to e}&&\cr
&=-\overrightarrow{F}_{e\to p}&&\cr
&=-m_{p}e_{p}&&\cr
\end{align*}
$$
Donc:
$$
\begin{align*}
\overrightarrow{a_{p}}&=-\frac{m_{e}}{m_{p}}\overrightarrow{a_{e}}&&\cr
|a_{p}|&=\frac{m_{e}}{m_{p}}|a_{e}|&&\cr
|a_{p}|&<<|a_{e}|&&\cr
\end{align*}
$$
On va supposer les protons fixe.

Théorème du moment cinétique appliqué à l'electron:
- $\overrightarrow{F}_{p\to e}=-\frac{e^{2}}{4\pi\varepsilon_{0}r^{2}}\overrightarrow{e_{r}}$ est une force centrale
donc:
$\overrightarrow{\mathcal{M}}_{O}=\overrightarrow{OM}\wedge \overrightarrow{F}_{p\to e}=\overrightarrow{O}$
Ainsi:
$\frac{\mathrm{d}\overrightarrow{L}_{O}}{\mathrm{d}t}=\overrightarrow{0}$
$\overrightarrow{L}_{O}=m\overrightarrow{OM}\wedge \overrightarrow{v}$ est constant
- Donc $(\overrightarrow{OM},\overrightarrow{v})\in \overrightarrow{L}_{O}^{\bot}$
Le mouvement est plan
- Constantes des aires:
$\overrightarrow{OM}=r\overrightarrow{e_{r}}$
$\overrightarrow{v}=\dot{r}\overrightarrow{e_{r}}+r\dot{\theta}\overrightarrow{e_{\theta}}$
$\overrightarrow{L}_{O}=m\overrightarrow{OM}\wedge \overrightarrow{v}=mr^{2}\dot{\theta}\overrightarrow{e_{z}}=m\mathcal{C}\overrightarrow{e_{z}}$
En notant $\mathrm{d}A$ l'aire balayé par $M$ durant un petit $\mathrm{d}t$, on trouve $\mathrm{d}A=\frac{\mathcal{C}}{2}\mathrm{d}t$.

Autre démo que $r^{2}\dot{\theta}$ est constant: par l'accélération selon $e_{\theta}$ via la seconde loi de newton.

Retour su l'electrons:
On suppose pour simplifier un mouvement circulaire.
Alors $r^{2}\dot{\theta}$ est constant, donc $\dot{\theta}$ est constant aussi, et peut s'exprimer comme $\dot{\theta}=\frac{2\pi}{T}$, avec $T$ la période de rotation.
On voit un courant:
$I=\frac{\delta q}{\mathrm{d}t}=-\frac{e}{T}$
On a donc:
$$
\begin{align*}
\overrightarrow{L}&=\frac{mR^{2}2\pi}{T}\overrightarrow{e_{z}}&&\cr
&=\frac{2m}{T}\pi R^{2}\overrightarrow{e_{z}}&&\cr
\end{align*}
$$
et, on considérant l'electrons qui tourne comme une spire (bon, il faut avoir la vision):
$$
\overrightarrow{\mathcal{m}}_{H}=I\pi R^{2}\overrightarrow{e_{z}}=-\frac{e}{T}\pi R^{2}\overrightarrow{e_{z}}
$$
$$
\begin{align*}
\overrightarrow{\mathcal{m}}_{H}&=-\frac{2m_{e}e}{T}\cdot \frac{\pi R^{2}}{2m_{e}}&&\cr
&-\frac{e}{2m_{e}}\overrightarrow{L}_{O}&&\cr
\end{align*}
$$
Donc, un electrons qui tourne autour d'un proton provoque l'apparition d'un moment magnétique.

En réalité $\overrightarrow{L}_{O}$ est quantifié (par la méca quantique): $L_{O}=n\hbar$
On appelle magnéton de Bohr:
$$
\mu_{B}=-\frac{e\hbar}{2m_{e}}
$$