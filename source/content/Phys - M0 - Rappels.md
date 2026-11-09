---
deck: phys
---
#todo finish this

Quand on fait de la mécanique, on définit notre système, le référentiel dans lequel on se place, et les coordonnées que l'on utilise.

# Notion de référentiel
<!-- basicblock-start -->
Def. référentiel galiléen::
- un référentiel qui satisfait la première loi de Newton.
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. référentiels usuels::
- Terrestre
- Géocentrique
- Héliocentrique
<!-- basicblock-end -->
# Notion de coordonnées
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
0 \cr
z
\end{pmatrix}
$$
<!-- basicblock-end -->
<!-- basicblock-start -->
Prop. Dérivée des vecteurs en cylindrique::
$$
\begin{align*}
\dot{\overrightarrow{u_{r}}}&=\dot{\theta}\overrightarrow{u_{\theta}}&&\cr
\dot{\overrightarrow{u_{\theta}}}&=-\dot{\theta}\overrightarrow{u_{r}}&&\cr
\end{align*}
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
0 \cr
0
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
# L'analogie rotationnelle
De même que les objets translatent, ils tournent, et l'on retrouve beaucoup d'analogie entre les deux mouvements.

On se place en coordonnée cylindrique, et l'on repère donc notre objet via l'angle plan $\theta$.
On définit ensuite la vitesse angulaire $\omega=\dot{\theta}$ et l'accélération angulaire $\alpha=\ddot{\theta}$.
De même qu'une force représente la modification apportée à l'accélération dépendamment de la masse, on peut calculer de même les moments de ces forces par rapports à un axe, et en déduire l'accélération angulaire, dépendamment du moment d'inertie:
#todo : change the name of this theorem.
<!-- basicblock-start -->
Th. pas moment cinétique::
$$
J_{\Delta}\alpha=\sum \mathcal{M}_{\Delta}(\overrightarrow{F}).
$$
<!-- basicblock-end -->
Avec la définition suivante du moment d'inertie:
<!-- basicblock-start -->
Def. moment d'inertie::
$$
J_{\Delta}=\sum_{i}m_{i}r_{i}^{2}.
$$
<!-- basicblock-end -->
et la définition suivante de moment d'une force:
<!-- basicblock-start -->
Def. moment d'une force par rapport à un axe::
$$
\mathcal{M}_{\Delta}(\overrightarrow{F})=\mathcal{M}_{O}(\overrightarrow{F})\cdot \overrightarrow{\Delta}.
$$
<!-- basicblock-end -->
<!-- basicblock-start -->
Def. moment d'une force par rapport à un point::
$$
\overrightarrow{\mathcal{M}_{O}}(\overrightarrow{F})=\overrightarrow{OM}\wedge \overrightarrow{F}.
$$
<!-- basicblock-end -->

#todo: fiche méthode: bras de levier.

On définit également le moment d'un point matériel par:
<!-- basicblock-start -->
Def. moment cinétique d'un point par rapport à un point::
$$
\overrightarrow{\mathcal{L}_{O}}(M)=\overrightarrow{OM}\wedge \overrightarrow{p}.
$$
<!-- basicblock-end -->
ainsi que son moment par rapport à un axe:
<!-- basicblock-start -->
Def. moment cinétique d'un point par rapport à un axe::
$$
\mathcal{L}_{\Delta}(M)=\overrightarrow{\mathcal{L}_{O}}(M)\cdot \overrightarrow{\Delta}.
$$
<!-- basicblock-end -->

Et l'on obtient alors le presque célèbre théorème du moment cinétique:
<!-- basicblock-start -->
Th. moment cinétique::
$$
\frac{\mathrm{d}\overrightarrow{\mathcal{L}_{O}}(M)}{\mathrm{d}t}=\sum \overrightarrow{\mathcal{M}_{O}}(\overrightarrow{F}).
$$
<!-- basicblock-end -->

#todo : justify with a demo, or something.
On en déduit la relation suivante:
<!-- basicblock-start -->
Prop. moment cinétique d'un solide par rapport à un axe::
$$
\mathcal{L}_{\Delta}(M)=J_{\Delta}\times\omega.
$$
<!-- basicblock-end -->
# Forces centrales
On étudie les forces conservatrice de la forme $\overrightarrow{F}=F(r,\theta,\varphi)\overrightarrow{u_{r}}$.
On démontre qu'elles se mettent sous la forme:
<!-- basicblock-start -->
Def. force centrale::
$$
\overrightarrow{F}=F(r)\overrightarrow{u_{r}}.
$$
<!-- basicblock-end -->

Ici, on se contentera d'étudier les forces newtoniennes, de la forme:
<!-- basicblock-start -->
Def. force newtonienne::
$$
\overrightarrow{F}=\frac{K}{r^{2}}\overrightarrow{u_{r}}.
$$
<!-- basicblock-end -->

Une des premières conséquence qui vient est la planéité du mouvement, on le démontre via le théorème du moment cinétique, avec ici notre force de moment nul.
<!-- basicblock-start -->
Prop. planéité du mouvement dû à une force centrale::
$$
\mathcal{L}_{O}(M)=cst.
$$
<!-- basicblock-end -->

> [!note]- Démonstration de la mise sous forme effective de l'énergie mécanique
> ![[Phys - Démo - Mise sous forme effective de l'énergie mécanique]]

# Exemple d'application






















