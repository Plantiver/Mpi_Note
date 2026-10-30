---
deck: phys
---
#todo finish this

Quand on fait de la mécanique, on définit notre système, le référentiel dans lequel on se place, et les coordonnées que l'on utilise.

# Différents Systèmes
### Mécanique du point
### Mécanique du solide

# Différents référentiels
### Référentiels galiléens

### Référentiels usuels


# Différentes coordonnées
### Coordonnées cartésiennes
<!-- basicblock-start -->
Def. Coordonnées en cartésien::
$$
\overrightarrow{OM}=\begin{pmatrix}
x \cr
y \cr
z
\end{pmatrix}
$$
<!-- basicblock-end -->
<!-- basicblock-start -->
Prop. Vitesse en cartésien::
$$
\overrightarrow{v}=\begin{pmatrix}
\dot{x} \cr
\dot{y} \cr
\dot{z}
\end{pmatrix}
$$
<!-- basicblock-end -->
<!-- basicblock-start -->
Prop. Accélération en cartésien::
$$
\overrightarrow{a}=\begin{pmatrix}
\ddot{x} \cr
\ddot{y} \cr
\ddot{z}
\end{pmatrix}
$$
<!-- basicblock-end -->

Les coordonnées cartésiennes servent lorsque l'on décrit un problème avec des symétrie de translation, ou alors peu de symétrie. Dans ce cas, la simplicité de l'expression de la vitesse et de l'accélération permettent souvent de simplifier le problème.

### Coordonnées cylindrique
<!-- basicblock-start -->
Def. Coordonnées en cylindrique::
$$
\overrightarrow{OM}=\begin{pmatrix}
r \cr
\theta \cr
z
\end{pmatrix}
$$
<!-- basicblock-end -->
<!-- basicblock-start -->
Prop. Vitesse en cylindrique::
$$
\overrightarrow{v}=\begin{pmatrix}
\dot{r} \cr
r\dot{\theta} \cr
\dot{z}
\end{pmatrix}
$$
<!-- basicblock-end -->
<!-- basicblock-start -->
Prop. Accélération en cylindrique::
$$
\overrightarrow{a}=\begin{pmatrix}
\ddot{r}-r\dot{\theta}^{2} \cr
r \ddot{\theta}+2\dot{r}\dot{\theta} \cr
\ddot{z}
\end{pmatrix}
$$
<!-- basicblock-end -->

Les coordonnées cylindriques servent lorsqu'on cherche à décrire un mouvement circulaire, ou lorsqu'il s'avère que notre systèmes possèdes des symétries de rotation.

### Coordonnées sphérique
<!-- basicblock-start -->
Def. Coordonnées en sphérique::
$$
\overrightarrow{OM}=\begin{pmatrix}
r \cr
\theta \cr
\varphi
\end{pmatrix}
$$
<!-- basicblock-end -->
La vitesse et accélération étant une purge en cylindrique, elle ne sont pas très utilisées dans les exercices, et sont donc hors programmes.

Les coordonnées sphériques servent majoritairement à démontrer qu'utiliser les coordonnées cylindrique est suffisant, est établissant des symétries de rotation.



# La physique newtonienne
Le modèle de newton fait des estimations très réaliste à notre échelle et jusqu'à d'assez grand systèmes (voir études des corps célestes).
Ainsi, chaque objet interagit avec les autres aux travers de forces, réciproque entre deux objets (3ème loi). Un objet se déplace ainsi en accords avec la somme des forces qui lui sont appliquées (2ème loi).
On définit la quantité de mouvement d'un système par:
<!-- basicblock-start -->
Def. Quantité de mouvement d'un système::
$$
\overrightarrow{p}=m\overrightarrow{v}.
$$
<!-- basicblock-end -->
Alors, la deuxième loi de newton nous dis:
![[Phys - Formule#2ème loi de Newton]]
Ce qui se simplifie en la forme plus connue si la masse du système est constante:
$$
m\overrightarrow{a}=\sum \overrightarrow{F}.
$$
On dira qu'une force est conservatrice si elle ne dépend que des coordonnées de l'objet auquel elle s'applique. Ainsi, la force de gravité est conservatrice, mais pas les forces de frottements.
# L'analogie rotationnelle
De même que les objets translatent, ils tournent, et l'on retrouve beaucoup d'analogie entre les deux mouvements.

On se place en coordonnée cylindrique, et l'on repère donc notre objet via l'angle plan $\theta$.
On définit ensuite la vitesse angulaire $\omega=\dot{\theta}$ et l'accélération angulaire $\alpha=\ddot{\theta}$.
De même qu'une force représente la modification 


# Etude énergétique
L'énergie est une grandeur qui se conservent au cours de l'évolution d'un système fermé, et permet donc, en étudiant les formes d'énergies présentes dans un système, d'étudier le système en question.
En mécanique, on s'intéresse plus spécifiquement à l'énergie potentielle et cinétique d'un système, les deux se définissant comme suit:
<!-- basicblock-start -->
Def. énergie cinétique d'un objet::
$$
\mathcal{E}_{c}=\frac{1}{2}mv^{2}.
$$
<!-- basicblock-end -->
<!-- basicblock-start -->
Def. énergie potentielle d'un objet::
- énergie qui ne provient que de la position de l'objet
- $\mathcal{E}_{p}=E(x,y,z)$.
<!-- basicblock-end -->

On définit ensuite l'énergie mécanique comme:
<!-- basicblock-start -->
Def. énergie mécanique::
$$
\mathcal{E}_{m}=\mathcal{E}_{c}+\mathcal{E}_{p}.
$$
<!-- basicblock-end -->

De là, pour étudier l'action d'une force non plus sur le mouvement mais sur l'énergie, on introduit le travail d'une force, c'est l'énergie qu'elle apporte à notre système lorsque l'on se déplace le long d'une trajectoire.
<!-- basicblock-start -->
Def. travail infinitésimal d'une force::
$$
\delta W=\overrightarrow{F}\cdot \overrightarrow{\mathrm{d}l}.
$$
<!-- basicblock-end -->
<!-- basicblock-start -->
Prop. travail d'une force::
$$
W_{\Gamma}=\int_{\Gamma}\overrightarrow{F}\cdot \overrightarrow{\mathrm{d}l}.
$$
<!-- basicblock-end -->
Ainsi, la force étudiée n'est pas conservatrice, le travail variera selon le trajet suivi, d'où l'importance de préciser le chemin $\Gamma$.

Avec la deuxième loi de newton, ainsi que la définition que nous venons de donner du travail, on retrouve le théorème de l'énergie cinétique:
<!-- basicblock-start -->
Th. de l'énergie cinétique::
$$
\mathrm{d}\mathcal{E}_{c}=\sum \delta W(\overrightarrow{F}).
$$
<!-- basicblock-end -->
Ce qui signifie que la variation de l'énergie liée à la vitesse est déterminé par l'énergie échangée via les forces appliquées au système.

De plus, on peut montrer qu'une force conservatrice donne toujours lieu à une énergie potentielle liée:
<!-- basicblock-start -->
Prop. énergie potentielle associée à une force conservatrice::
$$
\overrightarrow{F}=-\overrightarrow{ \mathrm{grad}}\mathcal{E}_{p}.
$$
<!-- basicblock-end -->
Pour plus de précision sur ce point, voir les détails sur le potentiel électrique dans le chapitre [[Phys - EM1 - Champs et potentiels créés par des charges ponctuelles]].

Ainsi, en réinjectant dans l'expressions de l'énergie mécanique, on obtient:
<!-- basicblock-start -->
Th. énergie mécanique::
$$
\mathrm{d}\mathcal{E}_{m}=\sum \delta W(\overrightarrow{F}_{\text{non conservatrice}}).
$$
<!-- basicblock-end -->
# Forces centrales


# Exemple d'application














