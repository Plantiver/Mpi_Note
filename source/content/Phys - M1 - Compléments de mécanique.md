---
deck: phys
---
# I - Les lois de frottements solide
# 1 - Les lois de Coulomb
Prenons un solide:
![[Loi de coulomb.svg]]

Lors d'un contact support/solide, le solide subit une réaction de la part du support:
$$
\overrightarrow{R}=\overrightarrow{T}+\overrightarrow{N}
$$
avec:
- $\overrightarrow{N}$ normale au support
- $\overrightarrow{T}$ tangentielle au support et opposé à la vitesse $\overrightarrow{v}$ ou permettant l'équilibre

$\overrightarrow{R}$ s'applique au barycentre de la surface de contact et est indépendant de la taille de la surface de contact.
**Loi de coulomb:**
En cas de glissement
![[Phys - Formule#Loi de Coulomb]]

**Rq:**
Ici, $\overrightarrow{v}$ est la vitesse de l'objet par rapport au support, non pas absolu.
Ce sont des égalités/inégalités sur des normes, pas sur les vecteurs.
On a: $f_{d}\leq f_{s}$. (il est plus difficile de mettre en mouvement un objet que de le pousser une fois qu'il se déplace).
On note souvent $f=f_{d}=f_{s}$.
L'absence de frottement implique $\overrightarrow{T}=\overrightarrow{0}$et si contacte avec un support, $\overrightarrow{v}=\overrightarrow{0}$.
$\overrightarrow{N}$ est nul seulement s'il n'y a pas de contact.
Se rappeler que $\|\overrightarrow{T}\|$ plus petit que $\|\overrightarrow{N}\|$: T peut facilement être nul, alors que N non.

**Ordre de grandeur:**

| solide | support       | $f_{s}$ | $f_{d}$ |
| ------ | ------------- | ------- | ------- |
| freins | acier         | 0.4     | 0.25    |
| pneu   | route sèche   | 0.9     | 0.5     |
| pneu   | route mouillé | 0.6     | 0.37    |
| pneu   | neige         | 0.2     | ...     |
| pneu   | glace         | 0.05    | ...     |
Attention, $f$ est mal défini, car il dépend énormément de l'état de surface.
Pour mesurer $f$, on prend un plan incliné sur lequel on pose l'objet, on mesure l'angle auquel il se met à glisser, et l'on prends l'arctangeante.

**Idée:**
Si on regarde microscopiquement les surfaces:
...Schéma avec des vagues pas très plates...
Donc les aspérités créé: les frottements

> [!note]- Exemple rupture de glissement
> ![[Phys - Exemple - Rupture de contact]]

> [!note]- Exemple du slip-stick
> ![[Phys - Exemple - Le slip-stick]]
## 2 - Différentes phases possibles

> [!note]- Exemple du solide sur une pente
> ![[Phys - Exemple - Solide posée sur une pente]]

# 3 - Travail de la force de frottement
- $\overrightarrow{N}$ est orthogonal à $\overrightarrow{v}$ donc ne travaille pas
- Seul $\overrightarrow{T}$ travaille

Et $\overrightarrow{T}=-T\frac{\overrightarrow{v}}{\|\overrightarrow{v}\|}$.
Donc:
$$
\begin{align*}
\delta W&=\overrightarrow{F}\cdot \overrightarrow{v}&&\cr
&=-T\frac{\overrightarrow{v}\cdot \overrightarrow{v}}{\|\overrightarrow{v}\|}&&\cr
&=-T\|\overrightarrow{v}\|&&\cr
\end{align*}
$$
Théorème de l'énergie cinétique:
$$
\delta \mathcal{E}_{c}=W<0
$$
Donc l'énergie cinétique diminue par les frottements, c'est bien cohérent.
Si $T$ constant:
$$
\begin{align*}
W&=-\int_{\gamma}Tv\mathrm{d}t&&\cr
&=-T\int_{\gamma}v\mathrm{d}t&&\cr
&=-T\int_{\gamma}\mathrm{d}l &&\cr
&=-Tl&&\cr
\end{align*}
$$

Ce travail dépend du chemin suivi, les frottements ne sont jamais conservatifs.

# II - Cinématique et changement de référentiels

(! ce chapitre ne suit pas la construction du prof, et a été écris par mes soins !)

Dès que l'on se place dans un référentiel non-galiléen, toute notre théorie s'effondre, et l'on ne sait plus comment appliquer nos connaissance. Étendons donc la théorie au référentiel non-galiléen.

Pour cela, prenons 2 référentiel, $\mathcal{R_{g}}(O,\overrightarrow{e_{i}},\overrightarrow{e_{j}},\overrightarrow{e_{k}})$ galiléen, et $\mathcal{R}(O',\overrightarrow{e_{x}},\overrightarrow{e_{y}},\overrightarrow{e_{z}})$ non, et un objet $M$ en mouvement.
On sait décrire le mouvement de $M$ dans $\mathcal{R}$, et le mouvement de $\mathcal{R}$ selon $\mathcal{R_{g}}$, on va donc essayer de combiner les deux pour retrouver nos lois du mouvement.

$$
\overrightarrow{OM}=\overrightarrow{OO'}+\overrightarrow{O'M}.
$$

## 1 - Vitesse dans un référentiel non-galiléen

La vitesse est la dérivée de la position, calculons
$$
\begin{align*}
\frac{\mathrm{d}\overrightarrow{OM}}{\mathrm{d}t}&=\frac{\mathrm{d}\overrightarrow{OO'}}{\mathrm{d}t}+ \frac{\mathrm{d}\overrightarrow{O'M}}{\mathrm{d}t}&&\cr
&=\frac{\mathrm{d}\overrightarrow{OO'}}{\mathrm{d}t}+\frac{\mathrm{d}(x\overrightarrow{e_{x}}+y\overrightarrow{e_{y}}+z\overrightarrow{e_{z}})}{\mathrm{d}t}&&\cr
&=\frac{\mathrm{d}\overrightarrow{OO'}}{\mathrm{d}t}+x \dot{\overrightarrow{e_{x}}}+y \dot{\overrightarrow{e_{y}}}+z \dot{\overrightarrow{e_{z}}}+\dot{x}\overrightarrow{e_{x}}+\dot{y}\overrightarrow{e_{y}}+\dot{z}\overrightarrow{e_{z}}&&\cr
&=\overrightarrow{v_{e}}+\overrightarrow{v_{r}}.&&\cr
\end{align*}
$$
avec
- $\overrightarrow{v_{e}}$ la vitesse d'entrainement, la vitesse due au mouvement de $\mathcal{R}$ dans $\mathcal{R_{g}}$
- $\overrightarrow{v_{r}}$ la vitesse relative, la vitesse de $M$ dans $\mathcal{R}$.

![[Phys - Formule#Loi de composition des vitesses]]

Pour simplifier l'expression de $\overrightarrow{v_{e}}$, on introduit $\overrightarrow{\Omega}$, le vecteur rotation, orienté selon l'axe de rotation, dirigé par la règle de la main droite, et de norme la vitesse de rotation.
En exprimant les vecteurs $\dot{\overrightarrow{e_{x}}},\dot{\overrightarrow{e_{y}}},\dot{\overrightarrow{e_{z}}}$ dans la base $\overrightarrow{e_{i}},\overrightarrow{e_{j}},\overrightarrow{e_{k}}$, on obtient que dérivée ces vecteurs revient à faire un produit scalaire avec $\overrightarrow{\Omega}$. Ainsi
<!-- basicblock-start -->
Prop. vitesse d'entrainement::
$$
\overrightarrow{v_{e}}=\frac{\mathrm{d}\overrightarrow{OO'}}{\mathrm{d}t}+\overrightarrow{\Omega}\wedge \overrightarrow{O'M}.
$$
<!-- basicblock-end -->

> [!note]- Exemple - La rotation de même centre
> ![[Phys - Exemple - Rotation de même centre]]


## 2 - Accélération dans un référentiel non-galiléen

L'accélération est la dérivée de la vitesse, calculons
$$
\begin{align*}
\overrightarrow{a}&=\frac{\mathrm{d}\overrightarrow{v}}{\mathrm{d}t}&&\cr
&=\frac{\mathrm{d}\overrightarrow{v_{e}}}{\mathrm{d}t}+\frac{\mathrm{d}\overrightarrow{v_{r}}}{\mathrm{d}t}&&\cr
&=\frac{\mathrm{d}^{2}\overrightarrow{OO'}}{\mathrm{d}t^{2}}+\frac{\mathrm{d}(\overrightarrow{\Omega}\wedge \overrightarrow{O'M})}{\mathrm{d}t}+\frac{\mathrm{d}(\dot{x}\overrightarrow{e_{x}}+\dot{y}\overrightarrow{e_{y}}+\dot{z}\overrightarrow{e_{z}})}{\mathrm{d}t}&&\cr
&=\frac{\mathrm{d}^{2}\overrightarrow{OO'}}{\mathrm{d}t^{2}}+\dot{\overrightarrow{\Omega}}\wedge \overrightarrow{O'M}+\overrightarrow{\Omega}\wedge \dot{\overrightarrow{O'M}}+\ddot{x}\overrightarrow{e_{x}}+\ddot{y}\overrightarrow{e_{y}}+\ddot{z}\overrightarrow{e_{z}}+\dot{x} \dot{\overrightarrow{e_{x}}}+\dot{y}\dot{\overrightarrow{e_{y}}}+\dot{z}\dot{\overrightarrow{e_{z}}}&&\cr
&=\frac{\mathrm{d}^{2}\overrightarrow{OO'}}{\mathrm{d}t^{2}}+\dot{\overrightarrow{\Omega}}\wedge \overrightarrow{O'M}+\overrightarrow{\Omega}\wedge (\overrightarrow{v_{r}}+\overrightarrow{\Omega}\wedge \overrightarrow{O'M})+\ddot{x}\overrightarrow{e_{x}}+\ddot{y}\overrightarrow{e_{y}}+\ddot{z}\overrightarrow{e_{z}}+\overrightarrow{\Omega}\wedge \overrightarrow{v_{r}}&&\cr
&=\frac{\mathrm{d}^{2}\overrightarrow{OO'}}{\mathrm{d}t^{2}}+\dot{\overrightarrow{\Omega}}\wedge \overrightarrow{O'M}+\overrightarrow{\Omega}\wedge (\overrightarrow{\Omega}\wedge \overrightarrow{O'M})+\ddot{x}\overrightarrow{e_{x}}+\ddot{y}\overrightarrow{e_{y}}+\ddot{z}\overrightarrow{e_{z}}+2\overrightarrow{\Omega}\wedge \overrightarrow{v_{r}}&&\cr
&=\overrightarrow{a_{e}}+\overrightarrow{a_{r}}+\overrightarrow{a_{c}}.&&\cr
\end{align*}
$$
avec
- $\overrightarrow{a_{e}}$ l'accélération d'entrainement
- $\overrightarrow{a_{r}}$ l'accélération relative, l'accélération de $M$ dans $\mathcal{R}$*
- $\overrightarrow{a_{e}}$ l'accélération de Coriolis.

![[Phys - Formule#Loi de composition des accélérations]]

**Attention,** on remarque que l'accélération d'entrainement n'est pas la dérivée de la vitesse d'entrainement, de même que l'accélération relative n'est pas la dérivée de la vitesse relative.

<!-- basicblock-start -->
Prop. accélération d'entrainement::
$$
\overrightarrow{a_{e}}=\frac{\mathrm{d}^{2}\overrightarrow{OO'}}{\mathrm{d}t^{2}}+\dot{\overrightarrow{\Omega}}\wedge \overrightarrow{O'M}+\overrightarrow{\Omega}\wedge(\overrightarrow{\Omega}\wedge \overrightarrow{O'M}).
$$
<!-- basicblock-end -->
<!-- basicblock-start -->
Prop. accélération de Coriolis::
$$
\overrightarrow{a_{c}}=2\overrightarrow{\Omega}\wedge \overrightarrow{v_{r}}.
$$
<!-- basicblock-end -->

> [!note]- Cas particulier de la rotation uniforme
> ![[Phys - Exemple - Rotation uniforme]]

# III - Dynamique en référentiel non galiléen
# 1 - Seconde loi de Newton
- $\mathcal{R_{g}}$ référentiel galiléen supposé fixe
- $\mathcal{R_{1}}$ référentiel mobile dans $\mathcal{R_{g}}$

Dans $\mathcal{R_{g}}$, on a la seconde loi de Newton:
$$
m\overrightarrow{a}(M/\mathcal{R_{g}})=\sum \overrightarrow{F}
$$
Mais, par la loi de composition des accélérations:
$$
\begin{align*}
\overrightarrow{a}(M/\mathcal{R_{g}})&=\overrightarrow{a}(M/\mathcal{R_{1}})+\overrightarrow{a_{e}}+\overrightarrow{a_{c}}&&\cr
m(\overrightarrow{a}(M/\mathcal{R_{1}})+\overrightarrow{a_{e}}+\overrightarrow{a_{c}})&=\sum \overrightarrow{F}&&\cr
m\overrightarrow{a}(M/\mathcal{R_{1}})&=\sum \overrightarrow{F}-m\overrightarrow{a_{e}}-m\overrightarrow{a_{c}}&&\cr
\end{align*}
$$
En référentiel galiléen on rajoute deux pseudo-forces d'inertie:
<!-- basicblock-start oid="ObsPOQqHoK93fJe6xTTyKR6X" -->
Prop. pseudo-forces d'inertie::
- Force d'inertie d'entrainement: $\overrightarrow{F_{ie}}=-m\overrightarrow{a_{e}}$
- Force d'inertie de Coriolis: $\overrightarrow{F_{ic}}=-m\overrightarrow{a_{c}}$
<!-- basicblock-end -->

ex:
- Une voiture accélère, $\overrightarrow{F_{ie}}$ est opposé à l'accélération, on "recule".
- Une machine à laver qui tourne, $\overrightarrow{F_{ie}}=m\omega^{2}\overrightarrow{HM}$ est la "force centrifuge", et projette à l'extérieur.

De même, on a le théorème du moment cinétique:
$$
\frac{\mathrm{d}}{\mathrm{d}t}\overrightarrow{L_{O}}(M/\mathcal{R_{1}})=\sum \overrightarrow{\mathcal{M}_{O}(\overrightarrow{F})}+\overrightarrow{\mathcal{M}_{O}(\overrightarrow{F_{ie}})}+\overrightarrow{\mathcal{M}_{O}(\overrightarrow{F_{ic}})}
$$
## 2 - Aspects énergétiques
**Coriolis:**
$$
\begin{align*}
P(\overrightarrow{F_{ic}})_{\mathcal{R_{1}}}&=(-2m\overrightarrow{\Omega}\wedge \overrightarrow{v_{r}})\cdot \overrightarrow{v_{r}}&&\cr
&=0&&\cr
\end{align*}
$$
La force d'inertie de Coriolis ne travaille pas.

**Entrainement:**
- Si translation uniforme $\overrightarrow{a_{c}}=a_{c}\overrightarrow{e_{u}}$
$$
\overrightarrow{F_{ie}}=-ma_{e}\overrightarrow{e_{u}}=-\overrightarrow{ \mathrm{grad}}(\mathcal{E}_{p}).
$$
- Si rotation uniforme $\overrightarrow{a_{c}}=-\omega^{2}r\overrightarrow{e_{r}}$
$$
\overrightarrow{F_{ie}}=m\omega^{2}r\overrightarrow{e_{r}}=-\overrightarrow{ \mathrm{grad}}(\mathcal{E}_{p}).
$$
Dans ces deux cas, $\overrightarrow{F_{ie}}$ est conservatrice.

**Théorème:**
- de la puissance cinétique
$$
\frac{\mathrm{d}}{\mathrm{d}t}\mathcal{E}_{c}(M/\mathcal{R_{1}})=\sum \mathcal{P}_{F}+\mathcal{P_{ie}}.
$$
- de l'énergie cinétique
$$
\Delta \mathcal{E}_{c}(M/\mathcal{R_{1}})=\sum W(\overrightarrow{F})+W(\overrightarrow{F_{ie}}).
$$
## 3 - Caractère non galiléen du référentiel terrestre
**Rappel:** Un référentiel est galiléen ssi le principe d'inertie s'applique.
Un référentiel en translation rectiligne uniforme avec un référentiel galiléen est galiléen.

![[Phys - Formule#1ère loi de Newton]]
(ce qui est totalement faux).

1. Le référentiel terrestre
Il tourne avec la Terre.
Pour une expérience de durée $<<24h$, il peut être supposé galiléen.
2. Le référentiel géocentrique
Il tourne autour du Soleil.
Supposé galiléen pour $\tau<<1$ an
3. Le référentiel héliocentrique
Il tourne dans la galaxie.
Supposé galiléen pour $\tau<<220$ millions d'année.

##### a) Le référentiel terrestre
Durée de rotation de la terre:
$$
\begin{align*}
T&=23h,\;56min,\;4s&&\cr
&\simeq24h&&\cr
\end{align*}
$$
Mais une journée dure bien 24h, la différence vient de si on compte en jour sidéral ou jour solaire.
La vitesse angulaire de rotation de la terre: $\boxed{\Omega_{T}=\frac{2\pi}{T}}$.
## 4 - Dynamique dans le référentiel terrestre

On se place dans $\mathcal{R_{T}}$ étudié par rapport à $\mathcal{R_{géo}}$.
D'après la seconde loi de Newton:
$$
m\overrightarrow{a}=\sum \overrightarrow{F}+\overrightarrow{F_{ie}}+\overrightarrow{F_{ic}}.
$$
avec $\sum \overrightarrow{F}=m\overrightarrow{g}+\sum \overrightarrow{F}_{\text{autres}}$ avec $\overrightarrow{g}$ définit par un théorème de Gauss gravitationnel.

> [!note]- Exemple 1
> ![[Phys - Exemple - Direction du fil à plomb]]

> [!note]- Exemple 2
> ![[Phys - Exemple - La déviation vers l'est]]

> [!note]- Exemple 3
> ![[Phys - Exemple - Les marées]]

# IV - Calculs matriciels

(! ce chapitre ne suit pas la construction du prof, et a été écris par mes soins !)


