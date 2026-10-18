---
deck: phys
---
Pour plus de précision sur la théorie derrière tout cela, voir les chapitres EM.

# Circuit électrique
Un circuit est un enchevêtrement de cable électrique, reliant ensemble différents composant.
A chaque point de ce circuit, on peut associer un potentiel électrique.
La tension entre deux points est la différence de potentielles entre ces deux points.
Les charges présentent dans le circuit se déplacent des hauts potentielles vers les bas potentielles.
Le courant désigne le déplacement de ses charges dans le circuit.
L'intensité quantifie ce courant, on mesure la quantité de charge traversant une section (orientée) au cours d'un petit temps. Par convention, on oriente la section des bas potentielles vers les hauts potentielles.

Dans un circuit, il existe deux manières principales d'associer des composants, en série et en dérivations (voir schéma (en ligne pour l'instant #todo )).

Un nœud est un point de jonction de plusieurs composants.
Une branche désigne l'ensemble des composants entre deux nœuds.
Une maille est une branche qui se referme sur elle même.

# Dipôle électrique
Un dipôle est un composant électrique avec deux bornes.
La majorité des composants que nous allons étudier sont des dipôles:
- Générateur
- Résistance
- Condensateur
- Bobine

# ARQS
L'ARQS est une approximation dans laquelle on se place pour simplifier beaucoup de situation, notamment nos études de petits circuits en laboratoire.

En considérant que le temps que mets le courant à circuler dans le circuit est petit devant la période du signal, on obtient une approximation suffisante.

Cela donne lieu à deux théorème fondamentaux:
La loi des nœuds affirme que l'intensité électrique sortante d'un nœud est égale à l'intensité électrique entrante.
La loi des mailles affirme que la somme des tensions aux bornes des composants d'une maille est nulle.

# Propriété des dipôles usuels dans l'Arqs
### Le générateur
Un **générateur de tension idéal** est un dipôle qui, comme son nom l'indique si bien, génère une certaine tension, permettant ainsi d'alimenter un circuit.
On choisira d'orienter la tension des générateurs en convention **générateur**, afin de simplifier les calculs.
En réalité, les générateurs de tensions ne sont pas parfait et possède une certaine résistance. Il est possible si nécessaire de la modéliser par une petite résistance en série d'un générateur idéal.

### Le fil
Un **fil** permet de relier deux composant d'un circuit, en permettant au courant de les traverser.
On les considère comme idéaux, c'est à dire sans résistance. La tension aux bornes d'un fil est nuls dans ce cas là.

### La résistance
Une **résistance** est un dipôle qui "freine" le courant. La matière dans une résistance n'étant pas conductrice, le charges ont plus de mal à se déplacer, et cela se matérialise par une relation linéaire entre la tension aux bornes de la résistance et l'intensité du courant:
$$
U=RI.
$$
Où $R$ est donc la résistance en Ohm du dipôle.
La résistance dissipe de l'énergie sous forme de chaleurs, et la puissance dissipée est:
<!-- basicblock-start -->
Prop. Puissance dissipée par une résistance::
$$
\mathcal{P}_{R}=RI^{2}.
$$
<!-- basicblock-end -->

### Le condensateur
Un **condensateur** est un dipôle qui crée une différence de tension entre ses deux bornes en empêchant le passage des charges. Au cours de son fonctionnement, il va se charger jusqu'à atteindre une tension maximale, à partir de laquelle il se comportera comme un interrupteur ouvert.
Tant que cette tension maximale n'est pas atteinte, des charges vont s'accumuler d'un coté du condensateur, et se dissiper de l'autre coté pour répondre à l'appel du circuit, créant un simili de courant "à travers" le condensateur.
Le condensateur est caractérisé par la relation entre la charge accumulée et la tension:
$$
Q=CU
$$
où $C$ est la capacité du condensateur en Farad.
Ainsi, par la définition du courant, on obtient:
$$
i=C\frac{\mathrm{d}U}{\mathrm{d}t}.
$$
Si la tension imposé à un condensateur est trop haute, le courant va commencer à circuler à travers le condensateur, créant des arcs électriques entre les deux bornes du condensateur.
Ce phénomène apparaît pour une tension supérieur à la tension disruptive du matériaux entre les deux bornes.

L'énergie stocké par un condensateur est:
<!-- basicblock-start -->
Prop. Energie stocké par un condensateur::
$$
E_{C}=\frac{1}{2}CU^{2}
$$
<!-- basicblock-end -->

Lorsqu'une tension n'est plus appliqué à un condensateur pour le charger, la tension accumulée à ses bornes lui permet de générer du courant, le faisant se décharger.

### La bobine
Une bobine est un dipôle qui crée un champs magnétique s'opposant à la variation du courant dans la bobine.
Ainsi, le courant est continue dans une bobine et l'on obtient l'équation caractéristique du dipôle:
$$
u=L\frac{\mathrm{d}i}{\mathrm{d}t}.
$$





