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
L'absence de frottement implique $\overrightarrow{T}=\overrightarrow{0}$.
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

**Idée:**
Si on regarde microscopiquement les surfaces:
...Schéma avec des vagues pas très plates...
Donc les aspérités créé: les frottements

> [!note]- Exemple rupture de glissement
> ![[Phys - Exemple - Rupture de contact]]

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

Un référentiel, c'est avant tout un point de vu sur un mouvement.

Ex: Valve d'une roue de vélo
- Vache sur la route: cycloïde
- Cycliste: cercle
- roue: immobile
## 1 - Notion de point coïncident
Introduisons 2 référentiels:
- $\mathcal{R}$ considéré fixe
- $\mathcal{R_{1}}$ considéré mobile
Soit un point $M(t)$ mobile dans $\mathcal{R}$ et $\mathcal{R_{1}}$

Le point coïncident est le point fixe dans $\mathcal{R_{1}}$ qui coincide avec $M(t)$ à l'instant $t$.
Ce point fixe dans $\mathcal{R_{1}}$ permet de décrire le mouvement $\mathcal{R_{1}}/\mathcal{R}$.

## 2 - Loi de composition des vitesses
- $\mathcal{R}$ repère fixe $O,\overrightarrow{i}, \overrightarrow{j}, \overrightarrow{k}$
- $\mathcal{R_{1}}$ repère mobile $O_{1},\overrightarrow{e_{x}},\overrightarrow{e_{y}},\overrightarrow{e_{z}}$
On veut étudier le mouvement de $M$:
$$
\begin{align*}
\overrightarrow{v}(M/\mathcal{R})&=\frac{\mathrm{d}\overrightarrow{OM}}{\mathrm{d}t}&&\cr
&=\frac{\mathrm{d}(\overrightarrow{OO_{1}}+\overrightarrow{O_{1}M})}{\mathrm{d}t}&&\cr
&=&&\cr
\end{align*}
$$
Vu $\overrightarrow{O_{1}M}=x\overrightarrow{e_{x}}+y\overrightarrow{e_{y}}+z\overrightarrow{e_{z}}$, et ces vecteurs étant mobiles dans $\mathcal{R}$:
$$
\frac{\mathrm{d}\overrightarrow{O_{1}M}}{\mathrm{d}t}=\dot{x}\overrightarrow{e_{x}}+\dot{y}\overrightarrow{e_{y}}+\dot{z}\overrightarrow{e_{z}}+x \dot{\overrightarrow{e_{x}}}+y \dot{\overrightarrow{e_{y}}}+z \dot{\overrightarrow{e_{z}}}.
$$
On appelle vitesse relative $\overrightarrow{v}(M/\mathcal{R_{1}})$.
On appelle vitesse d'entrainement de $\mathcal{R}/\mathcal{R_{1}}$: $\overrightarrow{v}_{e}=\frac{\mathrm{d}\overrightarrow{OO_{1}}}{\mathrm{d}t}+x \dot{\overrightarrow{e_{x}}}+y \dot{\overrightarrow{e_{y}}} +z \dot{\overrightarrow{e_{z}}}$.

On retient:
![[Phys - Formule#Loi de composition des vitesses]]

Regardons la vitesse d'entrainement:
- Si $\mathcal{R_{1}}$ est en translation dans $\mathcal{R}$:
Dans ce cas, les vecteurs sont d'orientations fixe dans $\mathcal{R}$ #todo : be more precise
ex: voiture sur une route droite, nacelle de grande roue
à ce moment là:
$$
\overrightarrow{v_{e}}=\frac{\mathrm{d}\overrightarrow{OO_{1}}}{\mathrm{d}t}.
$$
- Si $\mathcal{R_{1}}$ est en rotation (sans translation) dans $\mathcal{R}$:
$O_{1}$ est fixe dans $\mathcal{R}$.
à ce moment là:
$$
\overrightarrow{v_{e}}=x \dot{\overrightarrow{e_{x}}}+y \dot{\overrightarrow{e_{y}}}+z \dot{\overrightarrow{e_{y}}}.
$$
> [!note]- Exemple de rotation de même centre
> ![[Phys - Exemple - Rotation de même centre]]

- Si $\mathcal{R_{1}}$ est un mouvement quelconque
$$
\overrightarrow{v_{e}}=\frac{\mathrm{d}\overrightarrow{OO_{1}}}{\mathrm{d}t}+\overrightarrow{\Omega}\wedge \overrightarrow{O_{1}M}
$$


<!-- basicblock-start oid="Obs0BQbXhU2qJTgUnMR2JxFJ" -->
Def. vitesse d'entrainement::
vitesse du point coïncident dans $\mathcal{R}$
<!-- basicblock-end -->


## 3 - Loi de composition des accélérations

$$
\begin{align*}
\frac{\mathrm{d}^{2}\overrightarrow{OM}}{\mathrm{d}t^{2}}&=\frac{\mathrm{d}}{\mathrm{d}t}\left( \frac{\mathrm{d}\overrightarrow{OO_{1}}}{\mathrm{d}t}+x \dot{\overrightarrow{e_{x}}}+y \dot{\overrightarrow{e_{y}}}+z \dot{\overrightarrow{e_{z}}}+\dot{x}\overrightarrow{e_{x}}+\dot{y}\overrightarrow{e_{y}}+\dot{z}\overrightarrow{e_{z}} \right)&&\cr
&=\frac{\mathrm{d}^{2}\overrightarrow{OO_{1}}}{\mathrm{d}t^{2}}+x \ddot{\overrightarrow{e_{x}}}+y \ddot{\overrightarrow{e_{y}}}+z \ddot{\overrightarrow{e_{z}}}+2(\dot{x} \dot{\overrightarrow{e_{x}}}+\dot{y} \dot{\overrightarrow{e_{y}}}+\dot{z} \dot{\overrightarrow{e_{z}}})&&\cr
\end{align*}
$$
#todo add $\ddot{x}$ and all (coriolis)
- On appelle accélération relative $\overrightarrow{a_{r}}=\overrightarrow{a}(M/\mathcal{R_{1}})$
- On appelle accélération d'entrainement l'accélération du point coïncident dans $\mathcal{R}$ notée $\overrightarrow{a_{e}}$.

Dans un cas de translation, $\overrightarrow{a_{e}}=\frac{\mathrm{d}^{2}\overrightarrow{OO_{1}}}{\mathrm{d}t^{2}}$.

Dans un cas de rotation:
$$
\begin{align*}
\ddot{\overrightarrow{e_{x}}}&=\dot{\overrightarrow{\Omega}\wedge \overrightarrow{e_{x}}}&&\cr
&=\dot{\overrightarrow{\Omega}}\wedge \overrightarrow{e_{x}}+\overrightarrow{\Omega}\wedge \dot{\overrightarrow{e_{x}}}&&\cr
&=\dot{\overrightarrow{\Omega}}\wedge \overrightarrow{e_{x}}+\overrightarrow{\Omega}\wedge(\overrightarrow{\Omega}\wedge e_{x})&&\cr
\end{align*}
$$
Donc:
$$
\begin{align*}
\overrightarrow{v_{e}}&=\overrightarrow{\Omega}\wedge \overrightarrow{OM}&&\cr
\overrightarrow{a_{e}}&=\dot{\overrightarrow{\Omega}}\wedge \overrightarrow{OM}+\overrightarrow{\Omega}\wedge(\overrightarrow{\Omega}\wedge \overrightarrow{OM})&&\cr
\end{align*}
$$

- Dans le cas générale:
$$
\overrightarrow{a_{}}=\frac{\mathrm{d}^{2}\overrightarrow{OO_{1}}}{\mathrm{d}t^{2}}+x \ddot{\overrightarrow{e_{x}}}+y \ddot{\overrightarrow{e_{y}}}+z \ddot{\overrightarrow{e_{z}}}.
$$

!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! Attention !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
$$
\overrightarrow{a_{e}}\not=\frac{\mathrm{d}\overrightarrow{v_{e}}}{\mathrm{d}t}
$$
!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! Attention !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!


On appelle accélération de Coriolis et l'on note $a_{c}$ le terme restant.

Et donc:
<!-- basicblock-start oid="ObsHAS0PICTyjPVKZQRehbgI" -->
Prop. accélération de Coriolis::
$$
\overrightarrow{a_{c}}=2\overrightarrow{\Omega}\wedge \overrightarrow{v_{r}}.
$$
<!-- basicblock-end -->
Ainsi, pour $\overrightarrow{\Omega}=\overrightarrow{0}$ ou $\overrightarrow{v_{r}}=\overrightarrow{0}$, alors $\overrightarrow{a_{c}}=\overrightarrow{0}$.

![[Phys - Formule#Loi de composition des accélérations]]

> [!note]- Cas particulier de la rotation uniforme
> ![[Phys - Exemple - Rotation uniforme]]

Remarque:
Le mouvement d'une fourmi sur un rayon de roue de vélo:
$$
\begin{align*}
\overrightarrow{OM}&=r(t)\overrightarrow{e_{r}}&&\cr
\overrightarrow{v}&=\dot{r}\overrightarrow{e_{r}}+r\dot{\theta}\overrightarrow{e_{\theta}}&&\cr
\overrightarrow{a}&=\ddot{r}\overrightarrow{e_{r}}+2\dot{r}\dot{\theta}\overrightarrow{e_{\theta}}+(r \ddot{\theta}\overrightarrow{e_{\theta}}-r\dot{\theta}^{2}\overrightarrow{e_{r}}).&&\cr
\end{align*}
$$
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
\frac{\mathrm{d}}{\mathrm{d}t}\overrightarrow{L_{O}}(M/\mathcal{R_{1}})=\sum \overrightarrow{\mathcal{M}_{O}(\overrightarrow{F})}+\mathcal{M}_{O}(\overrightarrow{F_{ie}})+\mathcal{M}_{O}(\overrightarrow{F_{ic}})
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

![[Phys - Formule#2ème loi de Newton]]
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
