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

# IV - Le rayonnement thermique
## 1 - Définition

Tout corps à une certaine température $T$ émet un champ électromagnétique appelé "rayonnement thermique", qui se propage à la vitesse de la lumière;

Il s'agit du flux du vecteur de Poynting (voir [[Phys - EM5 - Le champ électromagnétique]]).

À une certaine longueur d'onde, on distingue deux type des de matériaux:
- Ceux transparent, qui laissent passer le rayonnement. On calculera alors le rayonnement totale d'après le volume.
- Ceux opaque, qui ne laissent pas passer le rayonnement. On calculera alors le rayonnement totale d'après la surface.

**Propriété radiative:**
- La réflexion
Tout rayonnement provenant de source de extérieur est réfléchi.
- L'absorption
Le rayonnement est absorbé, et fait augmenter l'énergie interne du milieu.
- L'émission
Un rayonnement est émis par le milieu, ce qui diminue son énergie interne.

En général, un milieu capable d'émettre une longueur d'onde peut aussi l'absorber.

Certains solides sont *diffusant*, l'émission et la réflexion sont aléatoire dans leur direction.

On définit le flux (puissance) surfacique:
- $\varphi_{r}$ : le flux surfacique réfléchi
- $\varphi_{a}$ : le flux surfacique absorbé
- $\varphi_{e}$ : le flux surfacique émis
Ici, $\varphi$ est en $W\cdot m^{-2}$, et par convention, on le prends toujours positif.

On définit alors:
- $\varphi_{i}=\varphi_{r}+\varphi_{a}$, le flux surfacique incident
- $\varphi_{p}=\varphi_{r}+\varphi_{e}$, le flux surfacique partant
- $\varphi_{R}=\varphi_{p}+\varphi_{i}=\varphi_{e}-\varphi_{a}$, le flux surfacique radiatif

## 2 - Le rayonnement d'équilibre

![[Phys - Formule#Loi de Planck]]

Schéma... #todo_later 

On comprends le spectre émis par un corps chaud à une certaine température.

On admet
$$
\varphi_{e}=\int_{0}^{+\infty} \frac{c}{4}w_{\lambda}\mathrm{d}\lambda.
$$

![[Phys - Formule#Loi de Wien]]

On pose $x=\frac{hc}{\lambda h_{0}T}$, donc $w_{\lambda}(x)=A\frac{x^{5}}{e^{x}-1}$.
Par le calcul, on montre $\frac{\mathrm{d}w_{\lambda}}{\mathrm{d}\lambda}=0\iff \frac{\mathrm{d}w_{\lambda}}{\mathrm{d}x}$.
Or
$$
\begin{align*}
\frac{\mathrm{d}w_{\lambda}}{\mathrm{d}x}&=A \frac{5x^{4}}{e^{x}-1}+Ax^{5} \frac{-e^{x}}{(e^{x}-1)^{2}}&&\cr
&=\frac{Ax^{4}}{(e^{x}-1)^{2}}(5(e^{x}-1)-xe^{x}).&&\cr
\end{align*}
$$
S'annule ssi
$$
\begin{align*}
5(e^{x}-1)&xe^{x}&&\cr
e^{x}(5-x)&=5&&\cr
e^{-x}&=1-\frac{x}{5}&&\cr
\end{align*}
$$
On ne sait pas résoudre analytiquement, donc on procède numériquement.
Méthode dichotomique:
Posons
$$
f(x)=e^{-x}-1+\frac{x}{5}
$$
On trace $f$ et l'on cherche $x_{1},x_{2}$ telle que $x_{0}\in[x_{1};x_{2}]$.
Attention, il faut qu'il y ait une unique solution entre $x_{1}$ et $x_{2}$, sinon on ne sait pas vers laquelle on va converger.

```pseudo-code
fn resolution_dichotomique(f,x1,x2,e) {
    x_m = (x1+x2)/2
    while |f(x_m)| > e {
        Si f(x1)xf(x_m) > 0 { x1 <- x_m }
        Sinon { x2 <- x_m }
        x_m = (x1+x2)/2
    }
    => x_m
}
```

On peut également utiliser $|x_{2}-x_{1}|<\varepsilon$ comme condition d'arrêt.

ICI, on trouve
$$
x_{0}\simeq 4.965
$$
Or, par définition de $x_{0}$
$$
\lambda_{m}T=\frac{hc}{k_{B}x_{0}}.
$$
L'application numérique nous donne la loi de Wien vue plus haut.

On admet que 98% de l'énergie est émise dans l'intervalle
<!-- basicblock-start -->
Prop. intervalle de concentration de l'énergie émise::
$$
\left[ \frac{\lambda_{m}}{2};8\lambda_{m} \right].
$$
<!-- basicblock-end -->

À partir de notre formule à ne pas savoir, on pose $x$ de même que plus haut, et l'on fait un changement de variable. On utilise ensuite le cours [[Math - Lesson - 13]].
$$
\begin{align*}
\varphi_{p}&\int_{0}^{+\infty} \frac{c}{4}w_{\lambda}\mathrm{d}\lambda &&\cr
&=\int_{0}^{+\infty} \frac{2\pi hc^{2}}{\lambda^{5}} \frac{1}{e^{hc/\lambda k_{B}T}-1}\mathrm{d}\lambda &&\cr
&=\frac{2\pi k_{B}^{4}T^{4}}{h^{3}c^{2}} \int_{0}^{+\infty} \frac{x^{3}}{e^{x}-1}\mathrm{d}x&&\cr
&=\frac{2\pi k_{B}^{4}T^{4}}{h^{3}c^{2}}\cdot \frac{\pi^{4}}{15}&&\cr
&=\frac{2\pi^{5}}{15}\cdot \frac{k_{B}^{4}}{h^{3}c^{2}}T^{4}.&&\cr
\end{align*}
$$

![[Phys - Formule#Loi de Stefan]]

> [!note]- Exemple du soleil
> ![[Phys - Exemple - Le Soleil]]

## 3 - Le modèle du corps noir

<!-- basicblock-start -->
Def. corps noir::
- opaque
- absorbeur totale d'énergie.
<!-- basicblock-end -->

Pour un corps noir
$$
\varphi_{a}=\varphi_{i}.
$$

...

Dans ce cas, même si l'objet n'est pas à l'équilibre thermique avec son environnement, on a
<!-- basicblock-start -->
Prop. flux surfacique émis d'un corps noir::
$$
\varphi_{e}=\sigma T^{4}.
$$
<!-- basicblock-end -->

En conséquence, la couleur d'un corps noir ne dépends que de sa température.

> [!note]- Exemple - Objet dans un four
> ![[Phys - Exemple - Objet dans un four]]

> [!note]- Exemple - L'effet de serre
> ![[Phys - Exemple - L'effet de Serre]]






