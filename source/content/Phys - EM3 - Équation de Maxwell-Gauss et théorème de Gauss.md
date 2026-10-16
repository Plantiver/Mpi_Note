---
deck: phys
---


# I - Equation de Maxwell-Gauss
## 1 - Enoncé
![[Phys - Formule#Equation de Maxwell-Gauss]]
<!-- basicblock-start oid="Obsxrocn5932CWoSzHwqwg5K" -->
Def. Permittivité diélectrique du vide::
$$
\varepsilon_{0}=8.85418782\times10^{-12}F\cdot m^{-1}.
$$
<!-- basicblock-end -->


Le champ $\overrightarrow{E(M,t)}$ s'écrit:
$$
\overrightarrow{E(x,y,z,t)}=E_{x}(x,y,z,t)\overrightarrow{e_{x} }+E_{y}(x,y,z,t)\overrightarrow{e_{y} }+E_{z}(x,y,z,t)\overrightarrow{e_{z} }
$$
Connaissant $\rho$, on ne peut pas retrouver $\overrightarrow{E}$, pas assez d'équation.

## 2 - Principe de Curie

On appelle **élément de symétrie** toute transformation géométrique qui laisse cette objet invariant (= en égale correspondance avec lui-même).
*Ex*: Un cube possède ses rotations et ses symétries, mais en nombre finis, alors que la sphère c'est en nombre infinis. Si je colorie les faces de mon cube, je ne peux plus aussi facilement le faire tourner/symétriser.
**Principe de Mr. Curie (1894)**:
- Lorsque certaines causes produisent certains effets, les éléments de symétries des causes doivent se retrouver dans les effets.
- Lorsque certains effets révèlent une dissymétrie, elle doit se retrouver dans les causes.
- Un effet a au moins les symétries de sa cause.
**Rappel de géométrie**
Un plan de symétrie est un plan qui divise l'espace en deux parties identiques et superposables quand on effectue une réflexion par rapport à ce plan.
Un plan d'antisymétrie transforme chaque propriété de l'espace en son opposé par reflexion.
**Application**
*ex*: sphère uniforme chargée en volume
$$
\rho(r,\theta,\varphi,t)=\begin{cases}
\rho_{0}\text{ si }r<R  \\
O \text{ sinon}
\end{cases}
$$
Soit un point $M$ quelconque.
Toute rotation autour de l'axe $\overrightarrow{OM}$ laisse la situation inchangée.
Le champ $\overrightarrow{E}$ doit respecter cette symétrie. On dis que:
$\overrightarrow{E}\in$ tout les plans de symétrie passant par $M$.

Si on place une charge $q$ sans vitesse initiale, en $M$, le champs électrique ne peut la déplacer que sur l'axe $\overrightarrow{OM}$.
Tout plan contenant $\overrightarrow{OM}$ est un plan de symétrie.

De plus, on oublie le point $M$.
- Les rotations d'angle $\theta$ ou $\varphi$ laisse la sphère invariante.
- De même pour les translations de temps.
$\rho$ indépendant de $\theta ,\;\varphi \text{ et }t,\;\implies \overrightarrow{E(r,\theta,\varphi,t)}=\overrightarrow{E(r)}$.
D'où $\overrightarrow{E(M,t)}=E(r)\overrightarrow{e_{r} }$
On passe de 12 trucs inconnus à 1.

**Principe de Superposition**
Maxwell-gauss est linéaire: on peut sommer ses équations.
Un problème sans symétrie peut être décomposé en sous problèmes symétrique.
*ex "classique"*:
Une sphère pleine - une plus petite sphère:
$$
\rho = \begin{cases}
0\text{ si }|OM_{1}|>R_{1} \\
0\text{ si }|OM_{2}|<R_{2} \\
\rho_{0} \text{ sinon}
\end{cases}
$$
On peut la voir comme la somme de deux sphère, et donc trouver plein de symétries, puis trouver $\overrightarrow{E}$ final par principe de superposition.

## 3 - Théorème de Gauss
![[Phys - Formule#Green-Ostrogradski]]
Soit un champ vectoriel $\overrightarrow{A(M)}$ définie sur un volume $V$ de surface fermée de contour $S$.
ça veut dire qu'on peut calculer la divergence d'un volume juste en regardant ce qu'il se passe à sa surface, en échange avec l'extérieur.
formule de stockes?

![[Phys - Formule#Théorème de Gauss]]
Soit un volume $V$ quelconque de surface fermée $S$.
$$
\phi_{s}(\overrightarrow{E})=\oint \int_{S}\overrightarrow{E}\cdot \overrightarrow{\mathrm{d}S}=\iiint_{V}\mathrm{div}\overrightarrow{E}\cdot \mathrm{d}V=\iiint_{V}\frac{\rho}{\varepsilon_{0} }\mathrm{d}V=\frac{1}{\varepsilon_{0} }\iiint_{V}\rho\mathrm{d}V=\frac{Q_{\text{intérieur à }S} }{\varepsilon_{0} }
$$
Pour les distribution de charge à "Haut degré de symétrie", le théorème de Gauss limite les calculs.
**Rq**
Si $\rho=0$, $\overrightarrow{E}$ est à flux conservatif. i.e. Tout le champ entrant ressort.
Construisons un tube de champs:
- S'appuie sur les lignes de champs
- se ferme orthogonalement aux lignes.
Ainsi, le flux de cette surface est la somme de celui à l'entrée, sur les cotés, et à la sortie.
La partie latérale vaut 0 par définition
Et on trouve en égalisant avec 0 que $E_{\text{entrée} }S_{\text{entrée} }=E_{\text{sortie} }S_{\text{sortie} }$.

**Méthode**
On peut appliquer le théorème de Gauss sur n'importe quel surface.
On va choisir des surfaces de Gauss tel que le calcul soit simple:
- $\overrightarrow{E}\cdot \overrightarrow{\mathrm{d}S}=0$, flux nul
- $\overrightarrow{E}$ constant sur $\mathrm{d}S$.

**Rq**
Dans le cas statique, on peut utiliser $\overrightarrow{E}=-\overrightarrow{ \mathrm{grad} }V$pour calculer V.

**Analogie avec la gravitation**
$$
F_{1\to{2} }=-\mathscr{G}\frac{m_{1}m_{2} }{r^{2} }\overrightarrow{u}
$$
$$
\overrightarrow{F_{1\to2} }=\frac{q_{1}q_{2} }{4\pi\varepsilon_{0}r^{2} }
$$
![[Phys - Formule#Théorème de Gauss gravitationnel]]

# II - Exemple de calculs de champs
## 1 - La charge ponctuelle

> [!note]- Calcul du champ engendré par une charge ponctuelle
> ![[Phys - Démo - Champ électrique d'une particule]]

## 2 - Sphère chargée uniformément en volume

> [!note]- Calcul du champ engendré par une sphère chargée uniformément
> ![[Phys - Démo - Champ électrique d'une sphère]]



#todo : demo: champ electrique d'une sphère par Maxwell-Gauss

> [!note]- Calcul du champs engendré par une sphère chargée uniformément via Maxwell-Gauss
> ![[Phys - Démo - Champ électrique d'une sphère par Maxwell-Gauss]]

**Application: énergie de liaison d'un noyau atomique**:

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

## 3 - Le cylindre infini chargé en Volume
#todo : turn this into a demo

> [!note]- Calcul du champ engendré par un cylindre infini chargé en volume
> ![[Phys - Démo - Champ électrique d'un cylindre infini]]

# III - Le condensateur plan
## 1 - Champs d'un plan infini chargé en surface

> [!note]- Calcul du champ engendré par un plan infini chargé en surface
> ![[Phys - Démo - Champ électrique d'un plan]]

## 2 - Le condensateur plan

Différence des potentiels entre 2 plans $\infty$.
Modélisation du condensateur plan:
Deux plaque des charges opposées ($\sigma$).
On place le $O$ entre les deux, et elles sont distantes de $e$.
On obtient (faire un dessin) que le champs, à l'extérieur des deux plaques, est nul, et de norme $\frac{\sigma}{\varepsilon_{0} }$ orienté de la plaque + vers la -.

$$
\overrightarrow{E}(x)= \begin{cases}
\overrightarrow{0},\;\text{si }|x|>\frac{e}{2} \cr
\frac{\sigma}{\varepsilon_{0} }\overrightarrow{e_{x} },\;\text{sinon}
\end{cases}
$$
La différence de potentielle:
$$
\begin{align*}
U&=V(+\sigma)-V(-\sigma)&&\cr
&=\left( -\frac{\sigma}{\varepsilon_{0} }\left( -\frac{e}{2} \right)+K \right)-\left( -\frac{\sigma}{\varepsilon_{0} }\left( +\frac{e}{2} \right)+K \right)&&\cr
&=\frac{\sigma e}{\varepsilon_{0} }&&\cr
\end{align*}
$$
C'est le modèle du condensateur plan.
Ce sont des armatures de surfaces $S$ et de charges $\pm Q$ que l'on modélise par des plaques $\infty$ et de charges surfacique $\sigma=\frac{Q}{S}$.

Dans un condensateur réel, on a des effets de fuites sur les bords. Ce sont les effets de bords, ils sont négligeable. (Les calculs sont faisables apparrement #work).
On définit la capacité du condensateur, en Farad (F):
$$
\boxed{C=\frac{Q}{U} }
$$

Or
$$
\begin{align*}
U=&\frac{\sigma e}{\varepsilon_{0} }=\frac{Qe}{S\varepsilon_{0} }&&\cr
\;\implies\;C=&\frac{S\varepsilon_{0} }{e}&&\cr
\end{align*}
$$

**rq:**
Les condensateur réels, on rajoute un matériau diélectrique entre les armatures:
$$
C=\frac{\varepsilon_{0}\varepsilon_{r}S}{e}
$$
avec $\varepsilon_{r}$ la permitivité relative (sans unité) du milieu.
Vide: $\varepsilon_{r}=1$
Air: $\varepsilon_{r}\simeq1$
Papier: $\varepsilon_{r}\simeq2$
Mica: $\varepsilon_{r}\simeq7$

Un diélectrique est un isolant à faible champ (le courant ne passe pas).
Si $E<E_{\text{dissruptif} }$, le milieu est isolant
Pour l'air: $~30kV/cm$
Papier: $~70kV/cm$
Mica: $~140kV/cm$

# IV - Les équations de Poisson et de Laplace
Equation de poisson:
$$
-\mathrm{div}(\overrightarrow{ \mathrm{grad} }V)=\frac{\rho}{\varepsilon_{0} }
$$
Démo: par Maxwell-Gauss.
On définit le Laplacien Scalaire:
$$
\dot{\Delta} f=\mathrm{div}(\overrightarrow{ \mathrm{grad} }f)
$$
$$
\dot{\Delta}=\overrightarrow{\nabla }^{2}
$$
L'équation de poisson devient simple:
![[Phys - Formule#Equation de Poisson]]

Et s'il n'y a pas de charge, i.e. $\rho=0$.
![[Phys - Formule#Equation de Laplace]]

Pourquoi on ne l'utilise pas:

> [!note]- Calcul du champ engendré par une sphère chargé uniformément en volume via Poisson
> ![[Phys - Démo - Champ électrique d'une sphère par Poisson]]








