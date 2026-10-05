---
deck: phys
---


# I - Equation de Maxwell-Gauss
## 1 - Enoncé
<!-- basicblock-start oid="ObsRdTxODgoTl4dT8oUNrCYA" -->
Loi. 1ère équation de Maxwell-Gauss::
$$
\forall M,\;\forall t,\;\mathrm{div}\overrightarrow{E(M,t)}=\frac{\rho(M,t)}{\varepsilon_{0}}
$$
<!-- basicblock-end -->
<!-- basicblock-start oid="Obsxrocn5932CWoSzHwqwg5K" -->
Def. Qu'est-ce qu'$\varepsilon_{0}$ ?::
La permittivité diélectrique du vide.
<!-- basicblock-end -->


Le champ $\overrightarrow{E(M,t)}$ s'écrit:
$$
\overrightarrow{E(x,y,z,t)}=E_{x}(x,y,z,t)\overrightarrow{e_{x}}+E_{y}(x,y,z,t)\overrightarrow{e_{y}}+E_{z}(x,y,z,t)\overrightarrow{e_{z}}
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
D'où $\overrightarrow{E(M,t)}=E(r)\overrightarrow{e_{r}}$
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
<!-- basicblock-start oid="ObsRsV2YxOyxcw67bKn3XKz2" -->
Loi. Formule de Green-Ostrogradski::
$$
\iiint_{V}\mathrm{div}\overrightarrow{E(M)}\mathrm{d}V=\oint \int_{S}\overrightarrow{E(M)}\cdot \overrightarrow{\mathrm{d}S}.
$$
<!-- basicblock-end -->
Soit un champ vectoriel $\overrightarrow{A(M)}$ définie sur un volume $V$ de surface fermée de contour $S$.
ça veut dire qu'on peut calculer la divergence d'un volume juste en regardant ce qu'il se passe à sa surface, en échange avec l'extérieur.
formule de stockes?

<!-- basicblock-start oid="ObsSkFoo4AB9FXTnJaG62ZFA" -->
Th. de Gauss::
$$
\phi_{S}(\overrightarrow{E})=\frac{Q_{\text{dans }S}}{\varepsilon_{0}}
$$
<!-- basicblock-end -->
Soit un volume $V$ quelconque de surface fermée $S$.
$$
\phi_{s}(\overrightarrow{E})=\oint \int_{S}\overrightarrow{E}\cdot \overrightarrow{\mathrm{d}S}=\iiint_{V}\mathrm{div}\overrightarrow{E}\cdot \mathrm{d}V=\iiint_{V}\frac{\rho}{\varepsilon_{0}}\mathrm{d}V=\frac{1}{\varepsilon_{0}}\iint_{V}S\mathrm{d}V=\frac{Q_{\text{intérieur à }S}}{\varepsilon_{0}}
$$
Pour les distribution de charge à "Haut degré de symétrie", le théorème de Gauss limite les calculs.
**Rq**
Si $\rho=0$, $\overrightarrow{E}$ est à flux conservatif. i.e. Tout le champ entrant ressort.
Construisons un tube de champs:
- S'appuie sur les lignes de champs
- se ferme orthogonalement aux lignes.
Ainsi, le flux de cette surface est la somme de celui à l'entrée, sur les cotés, et à la sortie.
La partie latérale vaut 0 par définition
Et on trouve en égalisant avec 0 que $E_{\text{entrée}}S_{\text{entrée}}=E_{\text{sortie}}S_{\text{sortie}}$.

**Méthode**
On peut appliquer le théorème de Gauss sur n'importe quel surface.
On va choisir des surfaces de Gauss tel que le calcul soit simple:
- $\overrightarrow{E}\cdot \overrightarrow{\mathrm{d}S}=0$, flux nul
- $\overrightarrow{E}$ constant sur $\mathrm{d}S$.

**Rq**
Dans le cas statique, on peut utiliser $\overrightarrow{E}=-\overrightarrow{ \mathrm{grad}}V$pour calculer V.

**Analogie avec la gravitation**
$$
F_{1\to{2}}=-\mathscr{G}\frac{m_{1}m_{2}}{r^{2}}\overrightarrow{u}
$$
$$
\overrightarrow{F_{1\to2}}=\frac{q_{1}q_{2}}{4\pi\varepsilon_{0}r^{2}}
$$
<!-- basicblock-start oid="ObslddyIpZvLKISfRJEAaxYN" -->
Th. de Gauss gravitationnel::
$$
\oint \int_{S}\overrightarrow{G}\cdot \overrightarrow{\mathrm{d}S}=-4\pi \mathscr{G}M_{\text{intérieur a }S}
$$
<!-- basicblock-end -->

# II - Exemple de calculs de champs
## 1 - La charge ponctuelle

> [!note]- Calcul du champ engendré par une charge ponctuelle
![[Phys - Démo - Champ électrique d'une particule]]

## 2 - Sphère chargée uniformément en volume

> [!note]- Calcul du champ engendré par une sphère chargée uniformément
![[Phys - Démo - Champ électrique d'une sphère]]

#todo : Clean up this mess, maybe put Maxwell-Gauss in a demo

**Autres méthode:** calcul direct par Maxwell-Gauss.
En sphérique:
$$
\mathrm{div}\overrightarrow{E}=\frac{1}{r^{2}}\frac{ \partial r^{2}E_{r} }{ \partial r } +\frac{1}{r\sin\varphi}\frac{ \partial E_{\theta} }{ \partial \theta } +\frac{1}{r\sin}\frac{ \partial \sin\theta E_{\varphi} }{ \partial \varphi } 
$$
Or $\overrightarrow{E}=E(r)\overrightarrow{e_{r}}$
$\implies \mathrm{div}\overrightarrow{E}=\frac{1}{r^{2}}\frac{ \partial r^{2}E_{r} }{ \partial r }$

En symétrie sphérique, calculons le flux sortant d'une coquille sphérique de rayon $r$ et d'épaisseur $\mathrm{d}r$.

Flux entrant en $r$: $\phi(r)=4\pi r^{2}E(r)$
Flux sortant en $r+\mathrm{d}r$: $\phi(r+\mathrm{d}r)=4\pi(r+\mathrm{d}r)^{2}E(r+\mathrm{d}r)$.

En posant: $f(r)=r^{2}E(r)$:
$\implies d\phi=4\pi \frac{df}{dr}dr$
Mais $d\phi=(\mathrm{div}\overrightarrow{E})dV$.
$dV=4\pi r^{2}dr$.

Mais
$$
d\phi=4\pi \frac{d}{dr} (r^{2}R)dr
$$
et
$$
d\phi=\mathrm{div}\overrightarrow{E}dV=\mathrm{div}\overrightarrow{E}4\pi r^{2}dr
$$
Donc:
$$
\mathrm{div}\overrightarrow{E}=\frac{1}{r^{2}}\frac{ \partial  }{ \partial r } (r^{2}E)
$$
*D'après Maxwell-Gauss:*
$$
\mathrm{div}\overrightarrow{E}=\frac{\rho(r)}{\varepsilon_{0}}
$$
- Si $r<R$:
$\rho(r)=\rho_{0}$
$$
\begin{align*}
\frac{1}{r^{2}}\frac{ \partial  }{ \partial r } (r^{2}E)=&\frac{\rho_{0}}{\varepsilon_{0}}&&\cr
\frac{ \partial  }{ \partial r } (r^{2}E)=&\frac{\rho_{0}r^{2}}{\varepsilon_{0}}&&\cr
r^{2}E=&\frac{\rho_{0}r^{3}}{3\varepsilon_{0}}+K_{1}&&\cr
\end{align*}
$$
En $r=0$, $\overrightarrow{E}$ appartient à tout les plans de symétrie, donc $\overrightarrow{E(0)}=\overrightarrow{0}$.
Donc $K_{1}=0$.
D'où, si $r<R$:
$$
E(r)=\frac{\rho r}{3\varepsilon_{0}}
$$
- Si $r>R$:
$$
\begin{align*}
\rho(r)=&0&&\cr
\mathrm{div}\overrightarrow{E}=&0&&\cr
\frac{ \partial  }{ \partial r } (r^{2}E)=&0&&\cr
E=&\frac{K_{2}}{r^{2}}&&\cr
\end{align*}
$$
$E$ est continue, étant solution d'une équation différentielle:
$E(R^{+})=E(R^{-})$
$$
K_{2}=\frac{\rho_{0}R^{3}}{3\varepsilon_{0}}
$$
$$
\begin{align*}
E(r)=&\frac{1}{r^{2}}\int_{0}^{r}\frac{\rho(u)u^{2}}{\varepsilon_{0}}du&&\cr
\end{align*}
$$
**Calcul du potentiel électrostatique**
$$
\overrightarrow{E}=-\overrightarrow{ \mathrm{grad}}V=-\frac{dV}{dr}\overrightarrow{e_{r}}
$$

- Si $r<R$:
$$
\begin{align*}
E=&\frac{r\rho_{0}}{3\varepsilon_{0}}&&\cr
\implies \frac{dV}{dr}=&-\frac{r\rho_{0}}{3\varepsilon_{0}}&&\cr
\implies V(r)=&-\frac{\rho_{0}r^{2}}{6\varepsilon_{0}}+K_{3}&&\cr
\end{align*}
$$
- Si $r>R$:
$$
V(r)=\frac{\rho_{0}R^{3}}{3\varepsilon_{0}r}+K_{4}
$$
On CHOISIT de prendre l'origine des potentiels en $+\infty$.
Donc $K_{4}=0$
... calculs
$K_{2}=\frac{1}{2}\frac{\rho_{0}R^{2}}{\varepsilon_{0}}$
... schémas

**Application: énergie de liaison d'un noyau atomique**:

Pour "construire un atome", on veut construire une boule de rayon $R$ et de charge uniforme $\rho_{0}$.
On apporte une charge $dq$ de l'infini qu'on place en coquille sphérique au rayon $r$ d'une boule déjà construite.
Le travaille nécessaire: $\delta W=V(r)dq$.
Or $dq=\rho_{0}dV=\rho_{04}\pi r^{2}dr$
et $V(r)=\frac{\rho_{0}r^{2}}{3\varepsilon_{0}}$
Donc: $\delta W=\frac{\rho_{0}^{2}4\pi r^{2}}{3\varepsilon_{0}}dr$
$$
\begin{align*}
\mathscr{E}&=\int_{0}^{R}\delta W&&\cr
&=\int_{0}^{R}\frac{\rho_{0}^{2}4\pi r^{4}}{3\varepsilon_{0}}dr&&\cr
&=\frac{\rho_{0}^{2}4\pi R^{5}}{15\varepsilon_{0}}&&\cr
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
En coordonnée cylindrique:
$$
\rho(r)=\begin{cases}
\rho_{0}\text{ si }r<R \cr
0 \text{ sinon}
\end{cases}
$$
1. Symétries et invariances:
invariant:
- translation d'axe $z$
- translation dans le temps
- rotation d'angle $\theta$.
symétrie:
- Le plan de $\overrightarrow{OM}$ et $\overrightarrow{O_{z}}$.
- Le plan de $(M,\overrightarrow{e_{r}},\overrightarrow{e_{\theta}})$
Donc: $\overrightarrow{E(r)}=E(r)\overrightarrow{e_{r}}$.
2. Choix de la surface de Gauss
On choisit la surface du cylindre centrée en $O_{z}$, passant par $M$, de hauteur $H$.
$$
\begin{align*}
\oint \int_{S}\overrightarrow{E}\cdot \overrightarrow{dS}&=\iint_{\text{Haut}}\overrightarrow{E}\cdot \overrightarrow{dS}+\iint_{\text{Bas}}\overrightarrow{E}\cdot \overrightarrow{dS}+\iint_{\text{side}}\overrightarrow{E}\cdot \overrightarrow{dS}&&\cr
&=\iint_{\text{side}} E\times dS&&\cr
&=E(r)2\pi rH&&\cr
\end{align*}
$$
3. Application du th.
$$
\oint \int_{S}\overrightarrow{E}\cdot \overrightarrow{dS}=\frac{Q_{\text{int}}}{\varepsilon_{0}}
$$
- Si $r<R$:
$$
Q_{\text{int}}=\rho_{0}V=\rho_{0}\pi r^{2}H
$$
Donc:
$$
\begin{align*}
E(r)2\pi rH=&\frac{\rho_{0} \pi r^{2}H}{\varepsilon_{0}}&&\cr
\implies E(r)=&\frac{\rho_{0}r}{Z\varepsilon_{0}}&&\cr
\end{align*}
$$
- Si $r>R$:
$$
Q_{\text{int}}=\rho_{0}\pi R^{2}H
$$
Donc:
$$
\begin{align*}
E(r)2\pi rH=&\frac{\rho_{0}\pi R^{2}H}{\varepsilon_{0}}&&\cr
\implies E(r)=&\frac{\rho_{0}R^{2}}{2\varepsilon_{0}r}&&\cr
\end{align*}
$$

4. Calcul direct par Maxwell-Gauss
$$
\mathrm{div}\overrightarrow{E}=\frac{1}{r}\frac{ \partial  }{ \partial r } (rE(r))
$$
rq: $d\phi=\phi(r+dr)-\phi(r)$.
$\phi(r)=E(r)2\pi rH$
$\phi(r+dr)=E(r+dr)2\pi(r+dr)H$
$d\phi=2\pi \frac{d}{dr}(rE(r))H=(\mathrm{div}\overrightarrow{E})dV$
avec
$dV=2\pi rdrH=\pi(r+dr)^{2}H-\pi r^{2}H$
$\implies \mathrm{div}\overrightarrow{E}=\frac{1}{r}\frac{ \partial  }{ \partial r }(rE)$
Ensuite, on raisonne de même que précédemment, et on obtient des valeurs similaire, on choisit  notre origine des potentielles, et c'est tout bon...
(Je ne vais pas tout écrire, surtout si le prof dis que c'est pas tant obligatoire.)

5. Calcul du potentiel
$$
\overrightarrow{E}=-\overrightarrow{ \mathrm{grad}}V=-\frac{dV}{dr}\overrightarrow{e_{r}}
$$
- $r<R$:
$V(r)=-\frac{\rho_{0}r^{2}}{4\varepsilon_{0}}+K_{3}$
- $r>R$:
$V(r)=-\frac{\rho_{0}R^{3}}{2\varepsilon_{0}}+K_{4}$

Choix de l'origine des potentiels:
Dans le poly, $V(0)=0$
Ici, on choisit $V(r=R)=0$. Le choix n'a pas d'importance tant que ce n'est pas l'infini, qui diverge.
- $r<R$:
$-\frac{\rho_{0}R^{2}}{4\varepsilon_{0}}+K_{3}=0\implies V(r)=\frac{\rho_{0}}{4\varepsilon_{0}}(R^{2}-r^{2})$
- $r>R$:
$V(r)=-\frac{\rho_{0}R^{2}}{2\varepsilon_{0}}\ln\left( \frac{r}{R} \right)$

# III - Le condensateur plan
## 1 - Champs d'un plan infini chargé en surface

> [!note]- Calcul du champ engendré par un plan infini chargé en surface
![[Phys - Démo - Champ électrique d'un plan]]

1. Invariances et symétries
Invariances:
- Toute translation de x,y, et t
Symétries:
- $(M,\overrightarrow{e_{z}},\overrightarrow{e_{x}})$
- $(M, \overrightarrow{e_{z}}, \overrightarrow{e_{y}})$
D'où: $\overrightarrow{E}=E(z)\overrightarrow{e_{z}}$
De plus, il y a une symétrie globale, le plan est un plan de symétries
Donc, $\overrightarrow{E(z)}=-\overrightarrow{E(-z)}$
2. Choix de la surface de Gauss
On prends un cylindre orientée selon $\overrightarrow{e_{z}}$, de hauteur $2H$, et coupée en son milieu par notre surface.
$$
\begin{align*}
\oint \int_{S}\overrightarrow{E}\cdot \overrightarrow{dS}=&\iint_{\text{Haut}}\overrightarrow{E}\cdot \overrightarrow{dS}+\iint_{\text{Bas}}\overrightarrow{E}\cdot \overrightarrow{dS}+\iint_{\text{side}}\overrightarrow{E}\cdot \overrightarrow{dS}&&\cr
=&E(z)S+ (-E(-z)S)+0&&\cr
=&2E(z)S&&\cr
\end{align*}
$$
3. Application du th.
$Q_{\text{int}}=\sigma S$
$$
\begin{align*}
\oint \int_{S}\overrightarrow{E}\cdot \overrightarrow{dS}=&\frac{Q_{\text{int}}}{\varepsilon_{0}}&&\cr
\implies2E(z)S=&\frac{\sigma S}{\varepsilon_{0}}&&\cr
\implies E(z)=&\frac{\sigma}{2\varepsilon_{0}}&&\cr
\end{align*}
$$


4. Calcul du potentiel
$$
\overrightarrow{E}=-\overrightarrow{ \mathrm{grad}}V = -\frac{\mathrm{d}V}{\mathrm{d}z}\overrightarrow{e_{z}}
$$
- $z>0$:
$$
V(z)=-\frac{\sigma z}{2\varepsilon_{0}}+V_{1}
$$
- $z<0$
$$
V(z)=\frac{\sigma z}{2\varepsilon_{0}}+V_{2}
$$
Avec l'origine des potentiels à $0$, on fait disparaître les variables.

## 2 - Le condensateur plan

Différence des potentiels entre 2 plans $\infty$.
Modélisation du condensateur plan:
Deux plaque des charges opposées ($\sigma$).
On place le $O$ entre les deux, et elles sont distantes de $e$.
On obtient (faire un dessin) que le champs, à l'extérieur des deux plaques, est nul, et de norme $\frac{\sigma}{\varepsilon_{0}}$ orienté de la plaque + vers la -.

$$
\overrightarrow{E}(x)= \begin{cases}
\overrightarrow{0},\;\text{si }|x|>\frac{e}{2} \cr
\frac{\sigma}{\varepsilon_{0}}\overrightarrow{e_{x}},\;\text{sinon}
\end{cases}
$$
La différence de potentielle:
$$
\begin{align*}
U&=V(+\sigma)-V(-\sigma)&&\cr
&=\left( -\frac{\sigma}{\varepsilon_{0}}\left( -\frac{e}{2} \right)+K \right)-\left( -\frac{\sigma}{\varepsilon_{0}}\left( +\frac{e}{2} \right)+K \right)&&\cr
&=\frac{\sigma e}{\varepsilon_{0}}&&\cr
\end{align*}
$$
C'est le modèle du condensateur plan.
Ce sont des armatures de surfaces $S$ et de charges $\pm Q$ que l'on modélise par des plaques $\infty$ et de charges surfacique $\sigma=\frac{Q}{S}$.

Dans un condensateur réel, on a des effets de fuites sur les bords. Ce sont les effets de bords, ils sont négligeable. (Les calculs sont faisables apparrement #work).
On définit la capacité du condensateur, en Farad (F):
$$
\boxed{C=\frac{Q}{U}}
$$

Or
$$
\begin{align*}
U=&\frac{\sigma e}{\varepsilon_{0}}=\frac{Qe}{S\varepsilon_{0}}&&\cr
\;\implies\;C=&\frac{S\varepsilon_{0}}{e}&&\cr
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
Si $E<E_{\text{dissruptif}}$, le milieu est isolant
Pour l'air: $~30kV/cm$
Papier: $~70kV/cm$
Mica: $~140kV/cm$

# IV - Les équations de Poisson et de Laplace
Equation de poisson:
$$
-\mathrm{div}(\overrightarrow{ \mathrm{grad}}V)=\frac{\rho}{\varepsilon_{0}}
$$
On définit le Laplacien Scalaire:
$$
\dot{\Delta} f=\mathrm{div}(\overrightarrow{ \mathrm{grad}}f)
$$
$$
\dot{\Delta}=\overrightarrow{\nabla }^{2}
$$
L'équation de poisson devient simple:
<!-- basicblock-start oid="ObsRuI9mpuyhJqPlLYO8BIAD" -->
Def. Equation de Poisson::
$$
\dot{\Delta} f+\frac{\rho}{\varepsilon_{0}}=0
$$
<!-- basicblock-end -->
<!-- basicblock-start oid="ObsHlXgVrI6eQ0V3Vv1onuZJ" -->
Def. Equation de Laplace::
$$
\dot{\Delta} V=0
$$
<!-- basicblock-end -->
Pourquoi on ne l'utilise pas:
Reprenons la sphère uniforme chargée en volume:
En sphérique:
$$
\begin{align*}
\dot{\Delta} V&=\frac{1}{r^{2}}\frac{ \partial  }{ \partial r } \left( r^{2}\frac{ \partial V }{ \partial r }  \right)+\frac{1}{r^{2}\sin\theta}\frac{ \partial  }{ \partial \theta } \left( \sin\theta \frac{ \partial V }{ \partial \theta }  \right)+\frac{1}{r^{2}\sin\theta}\frac{ \partial^{2}V }{ \partial \varphi^{2} } &&\cr
\end{align*}
$$
Par les invariances:
$$
\frac{1}{r^{2}}\frac{ \partial  }{ \partial r } \left( r^{2}\frac{ \partial V }{ \partial r }  \right)=-\frac{\rho}{\varepsilon_{0}}
$$
- $r<R$:
$$
\begin{align*}
\frac{ \partial  }{ \partial r } \left( r^{2}\frac{ \partial V }{ \partial r }  \right)=&-\frac{\rho r^{2}}{\varepsilon_{0}}&&\cr
r^{2}\frac{ \partial V }{ \partial r } =&-\frac{\rho r^{3}}{3\varepsilon_{0}}+A&&\cr
\end{align*}
$$
Or $\overrightarrow{E}(0)=\overrightarrow{0}$, donc $A=0$
$$
V(r)=-\frac{\rho r^{2}}{6\varepsilon_{0}}+B
$$
- $r>R$
$$
\begin{align*}
\frac{1}{r^{2}}\frac{ \partial  }{ \partial r }\left( r^{2}\frac{ \partial V }{ \partial r }  \right) &=0&&\cr
r^{2}\frac{ \partial V }{ \partial r } &=C&&\cr
\frac{ \partial V }{ \partial r } &=\frac{C}{r^{2}}&&\cr
V(r)&=-\frac{C}{r}+D&&\cr
\end{align*}
$$
En choisissant l'origine des potentiels à l'$\infty$, on retrouve la même chose...
C'est possible de faire la même chose pour le cylindre. Mais bon...


<!-- basicblock-start oid="ObsZF0qqNB0pyKkt5ZsOXaQ4" -->
Def. Laplacien::
$$
\dot{\Delta}=\overrightarrow{\nabla}^{2}
$$
<!-- basicblock-end -->







