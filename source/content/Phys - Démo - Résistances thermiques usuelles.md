---
deck: phys
---
# Énoncé
Un milieu sépare deux zones à températures différentes, on suppose qu'il n'y a pas de chaleur produite, et que l'on est en régime stationnaire. Calculez la résistance thermique du matériau à travers un pavé droit, les bords d'un cylindre, et la surface d'une sphère.
# Idée
On déroule à partir de l'équation de la chaleur en stationnaire sans source, et de l'équation de Fourrier.
# Démo
On est en stationnaire sans chaleur produite, donc
$$
\dot{\Delta}T=0.
$$

### Cartésien 1D
![[Phys - Démo - Résistances thermiques usuelles 2026-11-23 13.58.20.excalidraw.svg]]
On obtient
$$
\begin{align*}
T&=Ax+B&&\cr
T(0)&=T_{1}=B&&\cr
T(L)&=T_{2}=AL+B.&&\cr
\end{align*}
$$
Ainsi
$$
T=T_{1}+\frac{T_{2}-T_{1}}{L}x.
$$
Et donc, en cartésien
$$
\begin{align*}
\overrightarrow{j_{\text{th}}}&=-\lambda \overrightarrow{ \mathrm{grad}}T&&\cr
j_{th}&=-\lambda \frac{ \partial T }{ \partial x } &&\cr
&=-\lambda \frac{T_{2}-T_{1}}{L}.&&\cr
\end{align*}
$$
D'où
$$
\begin{align*}
R_{\text{th}}&=|\frac{T_{2}-T_{1}}{\phi}|&&\cr
&=|\frac{T_{2}-T_{1}}{Sj_{\text{th}}}|&&\cr
&=|\frac{T_{2}-T_{1}}{-\lambda S \frac{T_{2}-T_{1}}{L}}|&&\cr
&=\frac{L}{\lambda S}.&&\cr
\end{align*}
$$
<!-- basicblock-start oid="ObsD9p0gf14zZpuzQgdRyhod" -->
Prop. résistance thermique d'un ::
$$
R_{\text{th}}=\frac{L}{\lambda S}.
$$
<!-- basicblock-end -->

# Bord d'un cylindre
On a
$$
\begin{align*}
\phi&=\int_{S}\overrightarrow{j_{\text{th}}}\cdot \overrightarrow{\mathrm{d}S}&&\cr
&=j_{\text{th}}S&&\cr
&=(-\lambda \overrightarrow{ \mathrm{grad}}T)(2\pi rH)&&\cr
&=-2\pi\lambda rH \frac{\mathrm{d}T}{\mathrm{d}r}.&&\cr
\end{align*}
$$
Or, en stationnaire, $\phi$ est constant, donc
$$
\begin{align*}
\frac{\mathrm{d}T}{\mathrm{d}r}&=-\frac{\phi}{2\pi\lambda rH}&&\cr
\Delta T&=-\frac{\phi}{2\pi\lambda H}\ln\left( \frac{r_{2}}{R_{1}} \right).&&\cr
\end{align*}
$$
Ainsi, finalement
$$
R_{\text{th}}=\frac{1}{2\pi\lambda H}|\ln\left( \frac{r_{2}}{r_{1}} \right)|
$$

# Sphérique
De même
$$
\begin{align*}
\phi&=-\frac{\lambda \mathrm{d}T}{\mathrm{d}r}4\pi r^{2}&&\cr
\frac{\mathrm{d}T}{\mathrm{d}r}&=-\frac{\phi}{4\pi\lambda r^{2}}&&\cr
T_{2}-T_{1}&=\frac{\phi}{4\pi\lambda}\left( \frac{1}{r_{2}}-\frac{1}{r_{1}} \right)&&\cr
R&=\frac{1}{4\pi\lambda}|\frac{1}{r_{2}}-\frac{1}{r_{1}}|.&&\cr
\end{align*}
$$

# Conséquence
La première est à connaitre, les suivantes à retrouver.