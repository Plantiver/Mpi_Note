**Énoncé:**

**Idée:**

**Démo:**
#todo : do the thing
Prenons une portion de conducteur en $x$ et $x+\mathrm{d}x$.
Voir Sch2plutôt
Alors, la variation de charge dans ce volume pendant $\mathrm{d}t$.
Variation du stock: $Q(t+\mathrm{d}t)-Q(t)$.
$$
\mathrm{d}Q=Q(t+\mathrm{d}t)-Q(t)=\delta Q_{\text{entrant} }-\delta Q_{\text{sortant} }
$$
Or, $Q(t)=\rho(t)\mathrm{d}V$, $\rho$ uniforme car le volume est infinitésimal, avec $\mathrm{d}V=S\mathrm{d}x$.
$$
\mathrm{d}Q=(\rho(t+\mathrm{d}t)-\rho(t))S\mathrm{d}x
$$
On a: $\rho(t+\mathrm{d}t)=\rho(t)+\frac{ \partial \rho }{ \partial t }(t)\mathrm{d}t+o(\mathrm{d}t)$... SUPER IMPORTANT, A SAVOIR.
Donc:
$$
\mathrm{d}Q=\frac{ \partial \rho }{ \partial t }(t) \mathrm{d}tS\mathrm{d}x
$$
De plus:
$$
\delta Q_{\text{entrant} }=I_{\text{entrant} }\mathrm{d}t=j(x)S\mathrm{d}t
$$
et
$$
\delta Q_{\text{sortant} }=j(x+\mathrm{d}x)S\mathrm{d}t
$$
Donc, le flux:
$$
\delta Q_{\text{entrant} }-\delta Q_{\text{sortant} }=-\frac{ \partial j }{ \partial x } \mathrm{d}xS\mathrm{d}t
$$
Donc, au final:
$$
\frac{ \partial \rho }{ \partial t } \mathrm{d}tS\mathrm{d}x=-\frac{ \partial j }{ \partial x }\mathrm{d}xS\mathrm{d}t 
$$
$$
\implies \frac{ \partial \rho }{ \partial t } =-\frac{ \partial j }{ \partial x } 
$$
Demo. Equation de conservation de la charge en unidimensionnel:
$$
\frac{ \partial \rho }{ \partial t }=-\frac{ \partial j }{ \partial x }  
$$

**Conséquence:**
