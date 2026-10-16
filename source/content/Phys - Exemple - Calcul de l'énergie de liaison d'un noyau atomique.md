#todo : clean this up

Pour "construire un atome", on veut construire une boule de rayon $R$ et de charge uniforme $\rho_{0}$.
On apporte une charge $dq$ de l'infini qu'on place en coquille sphérique au rayon $r$ d'une boule déjà construite.
Le travaille nécessaire: $\delta W=V(r)dq$.
Or $dq=\rho_{0}dV=\rho_{04}\pi r^{2}dr$
et $V(r)=\frac{\rho_{0}r^{2} }{3\varepsilon_{0} }$
Donc: $\delta W=\frac{\rho_{0}^{2}4\pi r^{2} }{3\varepsilon_{0} }dr$
$$
\begin{align*}
\mathscr{E}&=\int_{0}^{R}\delta W&&\cr
&=\int_{0}^{R}\frac{\rho_{0}^{2}4\pi r^{4} }{3\varepsilon_{0} }dr&&\cr
&=\frac{\rho_{0}^{2}4\pi R^{5} }{15\varepsilon_{0} }&&\cr
\end{align*}
$$
**Rq**:
On peut montrer que:
$$
\mathscr{E}=\frac{1}{2}\iiint_{V}\rho(\overrightarrow{r})V(\overrightarrow{r})\mathrm{d}\tau
$$
Exo: retrouver $\mathscr{E}$ à partir de cette formule.
