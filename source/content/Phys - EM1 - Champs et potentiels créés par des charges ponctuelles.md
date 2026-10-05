---
deck: phys
---

<!-- basicblock-start oid="Obsd5iNjtG0CqwBJ4FRRKp3v" -->
Loi. de Coulomb entre $M_{1}(q_{1})$ et $M_{2}(q_{2})$::
$$
\overrightarrow{F_{E,M_{1}\to M_{2}}}=\frac{q_{1}q_{2}}{4\pi\varepsilon_{0}||\overrightarrow{M_{1}M_{2}}||^{3}}\overrightarrow{M_{1}M_{2}}.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsOyIxU0sBQNbgmJpzC4vMN" -->
Def. Champ électrostatique d'une particule $P(q_{1})$::
$$
\overrightarrow{E(M)}=\frac{q}{4\pi\varepsilon_{0}||\overrightarrow{PM}||^{3}}\overrightarrow{PM}.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obs7YnHeYRvyxpFK7u9wc9S8" -->
Prop. Principe de superposition du champs électrostatique::
$$
\overrightarrow{E}=\sum_{i}\overrightarrow{E_{i}}.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obs0KKbXhbTTw3goDk4gRrD6" -->
Def. Circulation d'un champ $\overrightarrow{a}$ le long de $\gamma$::
$$
\phantom{`}\mathcal{C}_{\gamma}=\int_{\gamma}\overrightarrow{a}\cdot \overrightarrow{dl}.\phantom{`}
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsvWhP7AfQI2KTT2nYxkXaP" -->
Prop. Propriété de la circulation::
- $\phantom{`}\mathcal{C}_{\gamma}+\mathcal{C}'_{\gamma} = (\mathcal{C}+\mathcal{C}')_{\gamma}\phantom{`}$
- $\phantom{`}\mathcal{C}_{-\gamma}=-\mathcal{C}_{\gamma}\phantom{`}$
- $\phantom{`}\mathcal{C}_{\gamma_{1}+\gamma_{2}}=\mathcal{C}_{\gamma_{1}}+\mathcal{C}_{\gamma_{2}}\phantom{`}$.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsQs4dxCozdUidfFJoM87Ta" -->
Def. Opérateur nabla::
$$
\overrightarrow{\nabla}=\begin{pmatrix}
\frac{ \partial  }{ \partial x }  \cr
\frac{ \partial  }{ \partial y }  \cr
\frac{ \partial  }{ \partial z } 
\end{pmatrix}
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObseS13l3QgyjzwoweoHEr4M" -->
Def. Opérateur gradient::
$$
\overrightarrow{grad}f=\overrightarrow{\nabla}f
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsyduipQ7uZ9NBPZbSHBHSf" -->
Def. Opérateur divergence::
$$
\mathrm{div}\overrightarrow{f}=\overrightarrow{\nabla}\cdot \overrightarrow{f}
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obsj06n3JnMPAKM1896l9JgQ" -->
Def. Opérateur rotationnel::
$$
\overrightarrow{rot}\overrightarrow{f}=\overrightarrow{\nabla}\wedge \overrightarrow{f}
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obs0iyoIFcLg06kzRL0Xn7N1" -->
Def. Potentielle électrostatique d'une particule::
$$
V(r) = \frac{1}{4\pi\varepsilon_{0}}\frac{q}{r}+K
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsaXVHOwOvTmq4cwVJ0nv4M" -->
Rel. Champ et potentielle électrostatique::
$$
\overrightarrow{E}=-\overrightarrow{grad}V
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obsxmc3Wohngf4etARBkL3SN" -->
Prop. Circulation conservative du champ électrostatique::
$$
\oint_{\gamma}\overrightarrow{E}\cdot \overrightarrow{dl}=0
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obs0SWEnJ3SOowUzU31DK5yQ" -->
Def. La différentielle::
$$
df=(\overrightarrow{\mathrm{grad}}f)\cdot \overrightarrow{dl}=\frac{ \partial y }{ \partial x }\mathrm{d}x+\frac{ \partial f }{ \partial y }\mathrm{d}y+\frac{ \partial f }{ \partial z }\mathrm{d}z  
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsFqP8mxQ351ofJFjyzU8Tn" -->
Prop. Dév Limité de $f$ en $M$ proche de $O$::
$$
f(M)\simeq f(O)+\overrightarrow{OM}\cdot (\overrightarrow{\mathrm{grad}}f)(O)
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsuDNGXnvGGTKyyE1ex9eiD" -->
Prop. Gradient en cylindrique::
$$
\overrightarrow{ \mathrm{grad}}f=\frac{ \partial f }{ \partial r } \overrightarrow{e_{r}}+\frac{1}{r}\frac{ \partial f }{ \partial \theta } \overrightarrow{u_{\theta}}+\frac{ \partial f }{ \partial z } \overrightarrow{u_z}
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obss510Q4Bp7TUqBWasKP7b4" -->
Def. Energie potentielle électrostatique::
$$
\mathcal{E}_{p}=qV
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsTOFeFdXZOJxm7GD0JcOGM" -->
Def. Tension électrique entre $A$ et $B$::
$$
\phantom{`}U_{AB}=\mathcal{C}_{\gamma_{AB}}\phantom{`}
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsyJd2hB2Ymn4AZETIQFpvr" -->
Def. Energie potentielle à partir de la force::
$$
\overrightarrow{F}=-\overrightarrow{ \mathrm{grad}}\mathcal{E}_{p}
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsyMSWtLbrkYpgHbA1QB6AY" -->
Prop. Circulation d'un fonction $f$ différentiable::
$$
\oint \overrightarrow{ \mathrm{grad}}f\cdot \overrightarrow{dl}=0
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsxvMskrO6UHuMJKHWHWiuc" -->
Def. Travail élémentaire d'une force::
$$
\delta W=\overrightarrow{F}\cdot \overrightarrow{\mathrm{d}l}
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsAzbMFuwmp6Yu49aZyNN9F" -->
Def. Travail d'une force::
$$
\phantom{`}W_{\gamma_{A\to B}}=\int_{\gamma_{A\to B}}\delta W\phantom{`}
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObscP7wigxlAyU2LDEMHhl6q" -->
Prop. Travail élémentaire d'une force conservative::
$$
\delta W=-\mathrm{d}\mathcal{E}_p
$$
<!-- basicblock-end -->

$$
W_{\infty \to M}=\int_{+\infty}^{M} \delta W =-\int_{+\infty}^{M}\mathrm{d}\mathcal{E}_p=-\mathcal{E}_p(M)=-qV(M)=-\frac{qq_{0}}{4\pi\varepsilon_{0}r}
$$
Si $r\to_{0}$, l'energie diverge:
- $qq_{0}<0\implies \mathcal{E}_p\to-\infty$
- $qq_{0}>0\implies \mathcal{E}_p\to+ \infty$
Pour $N$ particules
<!-- basicblock-start oid="ObsafzwmncVRlSjiobMBkADy" -->
Prop. Energie potentielle de N particules::
$$
\phantom{`}\mathcal{E}_p=\frac{1}{2}\sum_{i\not=j}\mathcal{E}_{p,i,j}\phantom{`}
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObstqCY6UlWt8rwMQNuQ7odG" -->
Prop. Les lignes du champ électrique::
- $\overrightarrow{E}$ est tangent aux lignes de champ.
- #todo 
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsXN2lYJdIy5klRC89trkFb" -->
Def. Dipôle électrostatique::
- $P$ de charge $+q$
- $N$ de charge $-q$
- Dipolaire: $\overrightarrow{p}=q\overrightarrow{NP}$.
<!-- basicblock-end -->

<!-- basicblock-start -->
Def. Approximation dipolaire::
$$
\forall M,\;\|\overrightarrow{OM}\|>>\|\overrightarrow{NP}\|.
$$
<!-- basicblock-end -->

> [!note]- Potentielle d'un dipôle
![[Phys - Démo - Potentiel d'un dypole]]


<!-- basicblock-start -->
Prop. Action d'un champs électrique uniforme sur un dipôle::
$$
\text{Couple de force de moment }\overrightarrow{\Gamma_{0}}=\overrightarrow{p}\wedge \overrightarrow{E_{0}}.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. Energie potentielle d'un dipôle soumis à un champs électrique uniforme::
$$
\mathcal{E}_{p}=-\overrightarrow{p}\cdot \overrightarrow{E_{0}}.
$$
<!-- basicblock-end -->

> [!note]- Application au modèle de la molécule
![[Phys - Démo - Modélisation d'un molécule comme un dipôle]]
