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
<!-- basicblock-start oid="ObsyE4fnji6LubN0up3vjko9" -->
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

On travaille sur un volume infinitésimal de phase condensée idéale, et l'on souhaite établir une expression de la variation de l'énergie. On se place dans un cas sans variation de l'énergie cinétique, ni travaille sur la matière.

Par les hypothèses, on a
$$
\begin{align*}
\mathrm{d}U&=\mathrm{d}H&&\cr
&=\dots &&\cr
&=\rho c\mathrm{d}T\mathrm{d}V.&&\cr
\end{align*}
$$
#todo correct this

<!-- basicblock-start -->
Prop. variation de l'énergie interne d'une phase condensé idéale::
$$
\mathrm{d}U=\rho c\mathrm{d}T\mathrm{d}V.
$$
<!-- basicblock-end -->


Mais, ici, le premier principe s'écrit
$$
\begin{align*}
\mathrm{d}U&=\delta Q&&\cr
&=\delta Q_{\text{échangée}}+\delta Q_{\text{produit}}&&\cr
\end{align*}
$$

Différentes réaction qui libère de la chaleur:
- chimique
- nucléaires
- effet Joule
- frottements
On écrit dans ce cas
<!-- basicblock-start oid="Obsm9UxbWIjv1v3uWgbc63QS" -->
Def. chaleur produite par une puissance::
$$
\delta Q_{\text{produit}}=\mathscr{P}_{V}\mathrm{d}V\mathrm{d}T
$$
<!-- basicblock-end -->
avec
- $\mathscr{P}_{V}$ la puissance volumique produite, en $W\cdot m^{-3}$.


On définit la chaleur échangée à travers une surface comme l'intégrale du flux de chaleur au cour du temps. Ce flux thermique peut être décrit comme le flux d'un vecteur densité à travers cette surface, on l'appelle le vecteur densité de chaleur.
On peut distinguer dans la chaleur échangée la chaleur entrante dans la surface, et la chaleur sortante, l'un compté positivement et l'autre négativement.

<!-- basicblock-start oid="ObsfENGwX429tqD5pyzZCn1k" -->
Def. chaleur échangée infinitésimale::
$$
\delta Q_{\text{échangée}}=\phi_{\text{th}}\mathrm{d}t.
$$
<!-- basicblock-end -->
<!-- basicblock-start -->
Def. flux thermique::
$$
\phi_{\text{th}}=\int_{S}\overrightarrow{j_{\text{th}}}\cdot \overrightarrow{\mathrm{d}S}.
$$
<!-- basicblock-end -->

On a donc
$$
\rho c\frac{ \partial T }{ \partial t } \mathrm{d}t\mathrm{d}V=(\phi+\mathscr{P}_{V}\mathrm{d}V)\mathrm{d}t.
$$

> [!note]- Démo - Calcul du flux thermique
> ![[Phys - Démo - Calcul du flux thermique]]

# II - Conduction dans un milieu immobile
## 1 - Loi de Fourier
Par l'observation, Fourier a donné la loi phénoménologique éponyme
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
- On admet que, dans le cas des métaux, bon conducteur électrique $\iff$ bon conducteur thermique.
- $\oplus$ les atomes sont liés, $\oplus$ la conduction est bonne.
- Le - dans l'équation est la matérialisation de l'inversion de gradient de température.

## 2 - Equation de diffusion de la chaleur

> [!note]- Démo - Équation de diffusion de la chaleur
> ![[Phys - Démo - Équation de diffusion de la chaleur]]

$$
\rho c\frac{ \partial T }{ \partial t } =-\mathrm{div}\overrightarrow{j_{\text{th}}}+\mathscr{P}_{V}
$$
Or $\overrightarrow{j_{\text{th}}}=-\lambda \overrightarrow{ \mathrm{grad}}T$
Donc
$$
\begin{align*}
\mathrm{div}\overrightarrow{j_{\text{th}}}&=\lambda \mathrm{div}\overrightarrow{ \mathrm{grad}T}&&\cr
&=\lambda \dot{\Delta} T&&\cr
\end{align*}
$$
<!-- basicblock-start oid="ObsmgzCniY22pVuf9AxVSSVh" -->
Th. equation de diffusion de la chaleur::
$$
\frac{ \partial T }{ \partial t } =\frac{\lambda}{\rho c}\dot{\Delta}T+\frac{\mathscr{P}_{V}}{\rho c}
$$
<!-- basicblock-end -->
On l'écrit souvent en 1D sans source de chaleur ($\mathscr{P}_{V}=0$):
$$
\frac{ \partial T }{ \partial t } =D\frac{ \partial^{2} T }{ \partial x^{2} } 
$$
avec $D=\frac{\lambda}{\rho c}$ la diffusivité thermique en $m^{2}\cdot s^{-1}$.
### Irréversibilité inhérente à l'équation de la chaleur
C'est une équation de **diffusion** qui traduit un phénomène **irreversible**. C'est l'inverse de l'équation de d'Alembert (cf [[Phys - EM5 - Le champ électromagnétique]]).
### Loi d'échelle
On note $\tau$ le temps caractéristique de la diffusion, et $L$ la distance associée à ce temps.
Voir schema...
On peut estimer que $\frac{ \partial T }{ \partial t }\simeq\frac{T_{1}-T_{0}}{\tau}$.
Voir schema 2...
On peut estimer que $\frac{ \partial^{2} T }{ \partial x^{2} }\simeq\frac{T_{1}-T_{0}}{L^{2}}$.
Ce sont des estimations très violentes, mais en ordre de grandeur, ça va.
Et donc
$$
\begin{align*}
\frac{ \partial T }{ \partial t } &=D\frac{ \partial^{2}T }{ \partial x^{2} } &&\cr
\frac{T_{1}-T_{0}}{\tau}&\simeq D\frac{T_{1}-T_{0}}{L^{2}}&&\cr
L&\simeq\sqrt{ D\tau }&&\cr
L&\propto \sqrt{ \tau }&&\cr
\end{align*}
$$
On retrouvera ça dans la vitesse de phase.

## 3 - Régime stationnaire sans source: les résistances thermiques
Repartons de l'équation de la chaleur
$$
\frac{ \partial T }{ \partial t } =D \dot{\Delta}T+\frac{\mathscr{P}_{V}}{\rho c}.
$$

On considère que la distribution de la chaleur ne varie plus, et qu'il n'y a pas de chaleur émise, ainsi
- $\frac{ \partial T }{ \partial t }=0$
- $\mathscr{P}_{V}=0$.

L'équation de la chaleur devient
<!-- basicblock-start -->
Prop. équation de la chaleur en stationnaire sans source::
$$
\dot{\Delta}T=0
$$
<!-- basicblock-end -->
### Analogie avec l'ARQS magnétique

| Elec                                                           | Thermo                                                                     |
| -------------------------------------------------------------- | -------------------------------------------------------------------------- |
| $\overrightarrow{j}=-\sigma \overrightarrow{ \mathrm{grad}}V$  | $\overrightarrow{j_{\text{th}}}=-\lambda \overrightarrow{ \mathrm{grad}}T$ |
| $I=\iint \overrightarrow{j}\cdot \overrightarrow{\mathrm{d}S}$ | $\phi=\iint \overrightarrow{j_{th}}\cdot \overrightarrow{\mathrm{d}S}$     |
| $V_{2}-V_{1}=RI$                                               | $T_{2}-T_{1}=R\phi$                                                        |

> [!note]- Calculs des résistances thermiques usuelles
> ![[Phys - Démo - Résistances thermiques usuelles]]

### Effet de peau thermique
> [!note]- Effet de peau thermique
> ![[Phys - Démo - Effet de peau thermique]]
 
# Couplage conducto-convectif à l'interface fluide/solide
### 1 - Loi de Newton

> [!note]- Exemple - Solide en contact avec un fluide en mouvement
> ![[Phys - Exemple - Solide en contact avec un fluide en mouvement]]

### 2 - Un exemple

> [!note]- Exemple - La tige de refroidissement
> ![[Phys - Exemple - La tige de refroidissement]]



