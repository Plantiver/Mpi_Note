---
deck: phys
---
#todo 
# Énoncé

# Idée

# Démo
**Calcul du flux unidimensionnel:**
$$
\begin{align*}
\phi_{\text{entrant}}&=j_{\text{th}}(x)S&&\cr
\phi_{\text{sortant}}&=j_{\text{th}}(x+\mathrm{d}x)S&&\cr
\end{align*}
$$
Et donc
$$
\begin{align*}
\phi_{\text{entrant}}-\phi_{\text{sortant}}&=-\frac{ \partial j_{\text{th}} }{ \partial x } \mathrm{d}xS&&\cr
\end{align*}
$$
D'où
$$
\rho c\frac{ \partial T }{ \partial t } =-\frac{ \partial j_{\text{th}} }{ \partial x }+\mathscr{P}_{V} 
$$
**Calcul du flux en cylindrique:**
$$
\begin{align*}
\overrightarrow{j_{\text{th}}}=j_{\text{th}}(r)\overrightarrow{e_{r}}&&&\cr
\mathrm{d}V&=2\pi rH\mathrm{d}r&&\cr
\phi_{\text{entrant}}&=j_{\text{th}}(r)2\pi rH&&\cr
\phi_{\text{sortant}}&=j_{\text{th}}(r+\mathrm{d}r)2\pi(r+\mathrm{d}r)H&&\cr
\phi_{\text{entrant}}-\phi_{\text{sortant}}&=-\frac{ \partial j_{\text{th}}(r)r }{ \partial r }2\pi H\mathrm{d}r&&\cr
&=-\frac{ \partial rj_{\text{th}} }{ \partial r } \frac{1}{r}2\pi Hr\mathrm{d}r &&\cr
\end{align*}
$$

Bilan d'énergie:
$$
\begin{align*}
\rho c\frac{ \partial T }{ \partial t } \mathrm{d}t\mathrm{d}V&=-\frac{1}{r}\frac{ \partial rj_{\text{th}} }{ \partial r } \mathrm{d}t\mathrm{d}V+\mathscr{P}_{V}\mathrm{d}t\mathrm{d}V&&\cr
\rho c\frac{ \partial T }{ \partial t } &=-\frac{1}{r}\frac{ \partial rj_{\text{th}} }{ \partial r } +\mathscr{P}_{V}&&\cr
\end{align*}
$$
**Calcul du flux en sphérique:**
$$
\begin{align*}
\mathrm{d}V&=4\pi r^{2}\mathrm{d}r &&\cr
\phi_{\text{entrant}}&=j_{\text{th}}(r)4\pi r^{2}&&\cr
\phi_{\text{sortant}}&=j_{\text{th}}(r+\mathrm{d}r)4\pi(r+\mathrm{d}r)^{2}&&\cr
\phi_{\text{entrant}}-\phi_{\text{sortant}}&=-4\pi \frac{ \partial r^{2}j_{\text{th}} }{ \partial r } \mathrm{d}r&&\cr
&=-\frac{1}{r^{2}}\frac{ \partial r^{2}j_{\text{th}} }{ \partial r } \mathrm{d}V&&\cr
\end{align*}
$$
Bilan d'énergie:
$$
\rho c\frac{ \partial T }{ \partial t } =-\frac{1}{r^{2}}\frac{ \partial r^{2}j_{\text{th}} }{ \partial r } +\mathscr{P}_{V}
$$
**Calcul du flux en général:**
$$
\rho c\frac{ \partial T }{ \partial t } =-\mathrm{div}\overrightarrow{j_{\text{th}}}+\mathscr{P}_{V}
$$
Démo:
$$
\begin{align*}
\phi_{\text{entrant}}-\phi_{\text{sortant}}&=-\oint \int_{S}\overrightarrow{j_{\text{th}}}\cdot \overrightarrow{\mathrm{d}S}&&\cr
&=-\iiint_{V}(\mathrm{div}\overrightarrow{j_{\text{th}}})\mathrm{d}V&&\cr
\end{align*}
$$
Et donc, on conclut par le bilan d'énergie.

# Conséquence
