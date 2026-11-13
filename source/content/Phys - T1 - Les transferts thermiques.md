---
deck: phys
---
# I - Rappels
## 1 - La chaleur
Constat: On prends deux matières en contact avec des températures différentes -> On a uniformisation de la température.
Il s'agit d'échange d'énergie désordonné au niveau microscopique.
L'agitation thermique des atomes est transférée à d'autres.
On la note $Q$, et, pour une transformation infinitésimale, $\delta Q$.

## 2 - Les 3 types d'échanges thermiques
<!-- basicblock-start -->
Def. les types d'échanges thermiques::
- Conduction
- Convection
- Rayonnement.
<!-- basicblock-end -->

1. La conduction
C'est un échange thermique par contact de proche en proche.
Il n'y a pas de déplacement de matière.
Ex: la casserole en métal sur le feu chauffe.

2. La convection
C'est un échange par déplacement de matière de températures différentes.
En générale, c'est avec un fluide.
Ex: l'eau dans la casserole qui bouillonne.

3. Le rayonnement
Tout corps chaud rayonne un champ électromagnétique qui porte et transfert de l'énergie.
Il n'y a pas besoin de support matériel, le milieu peut être le vide.
Ex: Un feu de cheminée, ou le soleil (et d'autres, c'est pas parce que je met ou que ce sont les seuls).

## 3 - Bilan local d'énergie
Système: {portion infinitésimale de phase condensée (solide ou liquide)}
Appliquons le premier principe sur une transformation infinitésimale.
Ici, on néglige tout les travaux et variations microscopique d'$\mathcal{E}_{c}$.
Pour rappels, pour une phase condensée:
$$
\mathrm{d}U\simeq \mathrm{d}H\text{ car }C_{V}\simeq C_{p}=C
$$
Donc:
$$
\begin{align*}
\mathrm{d}U&\simeq \mathrm{d}H&&\cr
&=C\mathrm{d}T&&\cr
&=c_{v}\mathrm{d}V\mathrm{d}T&&\cr
\end{align*}
$$
On utilise les grandeurs massiques:
- $c$: capacités calorifique massique en $J\cdot K^{-1}\cdot kg^{-1}$
et
$$
c_{v}=c\rho.
$$
Ainsi
$$
\mathrm{d}U=\rho c\mathrm{d}V\mathrm{d}T.
$$
**Bilan d'énergie** entre $t$ et $t+\mathrm{d}t$:
$$
\begin{align*}
U(t+\mathrm{d}t)-U(t)&=\frac{ \partial U }{ \partial t } \mathrm{d}t&&\cr
&=\rho c\frac{ \partial T }{ \partial t } \mathrm{d}t\mathrm{d}V&&\cr
\end{align*}
$$
Mais, ici, le premier principe s'écrit
$$
\begin{align*}
\mathrm{d}U&=\delta Q&&\cr
&=\delta Q_{\text{entrant}}-\delta Q_{\text{sortant}}+\delta Q_{\text{produit}}&&\cr
\end{align*}
$$
Différentes réaction qui libère de la chaleur:
- chimique
- nucléaires
- effet Joule
- frottements
On écrit dans ce cas
<!-- basicblock-start -->
Def. chaleur produite par une puissance::
$$
\delta Q_{\text{produit}}=\mathscr{P}_{V}\mathrm{d}V\mathrm{d}T
$$
<!-- basicblock-end -->
avec
- $\mathscr{P}_{V}$ la puissance volumique produite, en $W\cdot m^{-3}$.

On définit
<!-- basicblock-start -->
Def. chaleur infinitésimale échangée::
$$
\delta Q_{\text{échangé}}=\delta Q_{\text{entrant}}-\delta Q_{\text{sortant}}
$$
<!-- basicblock-end -->
On l'écrit comme un flux d'un vecteur
<!-- basicblock-start -->
Def. vecteur densité de flux thermique::
$$
\overrightarrow{j_{th}}
$$
<!-- basicblock-end -->
ou courant thermique.
On a donc
$$
\delta Q_{\text{échangé}}=-\oint \int_{S}\overrightarrow{j_{th}}\cdot \overrightarrow{\mathrm{d}S}\mathrm{d}t=\phi \mathrm{d}t.
$$
Et donc
$$
\begin{align*}
\delta Q_{\text{entrant}}&=\phi_{\text{entrant}}\mathrm{d}t &&\cr
\delta Q_{\text{sortant}}&=\phi_{\text{sortant}}\mathrm{d}t&&\cr
\end{align*}
$$
avec $\phi=jS$.
Ainsi
$$
\rho c\frac{ \partial T }{ \partial t } \mathrm{d}t\mathrm{d}V=(\phi_{\text{entrant}}-\phi_{\text{sortant}}+\mathscr{P}_{V}\mathrm{d}V)\mathrm{d}t.
$$

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

# II - Conduction dans un milieu immobile
## 1 - Loi de Fourier
Par l'observation, Fourier a donné la loi phénoménologique de Fourier
![[Phys - Formule#Loi phénoménologique de Fourier]]
avec $\lambda$ la conductivité thermique en $W\cdot m^{-1}\cdot K^{-1}$.


| Matériau   | $\lambda$ |
| ---------- | --------- |
| Cuivre     | 390       |
| Acier      | 13        |
| Verre      | 1         |
| Béton      | 0.9       |
| eau (20°C) | 0.6       |
| air        | 0.03      |

Rq:
- On admet que bon conducteur électrique $\iff$ bon conducteur thermique.
- $\oplus$ les atomes sont liés, $\oplus$ la conduction est bonne.
- Le - dans l'équation est la matérialisation de l'inversion de gradient de température.




































