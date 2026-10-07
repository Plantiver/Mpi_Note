---
deck: phys
---
# 1 - Rappels sur le champs magnétique

**Idée 1:** Les boussoles s'orientent sur le champ $\overrightarrow{V}$.

**Ordres de grandeur:**
Champs à la surface de la Terre: $5\cdot10^{-5}T$
Aimant: $0.1$ à $1T$
Bobine TP: $10mT$
Moteur électrique: $0.5T$
Electroaimant: $1$ à $10T$
IRM: $5T$.

**Propriété des lignes de champs:**
- Dirigés du pôle Nord vers le Sud
- Si deux lignes se croisent $\overrightarrow{B}=\overrightarrow{0}$
- 
- Elles sont toujours fermés
- Elles sont orientées et entourents les courants avec la rêgle de la main droite
- 
**Cartes à connaitres:**
- aimant droit
- spin



## 2 - Equation de Maxwell-flux (Maxwell-Thomson)
![[Phys - Formule#Equation de Maxwell-Thomson]]
$\;\implies\;$ Le champs magnétique est TOUJOURS à flux conservatif.
Donc
$$
\phi_{B}=\oint \int_{S}\overrightarrow{B}\cdot \overrightarrow{\mathrm{d}S}=0
$$
Comme $\overrightarrow{E}$ dans une région vide, les lignes de champs se resserrent quand la norme augmente.

De plus, les lignes de champs sont toujours fermées.

## 3 - Equation de Maxwell-Ampère
**a - Rotationnel d'un champ de vecteur**:
def du rotationnel, voir [[Phys - Math#Opérateur rotationnel]].

rappel sur le produit vectoriel:
règle de la main droite + longeur
ou alors produit croisée

**interprétation:**
- calculer la circulation sur un petit carré
- sommer les cotés face à face
- se rendre compte que 
> [!note]- Interprétation du rotationnel
![[Phys - Démo - Interprétation du rotationnel]]

**énoncé:**
![[Phys - Formule#Equation de Maxwell-Ampère]]
avec:
- $\mu_{0}$ la perméabilité magnétique du vide
- $c$ la célérité de la lumière dans le vide
- $\overrightarrow{j}$ vecteur densité volumique de courant

Dans le cadre de l'*ARQS magnétique* (cf [[Phys - EM5 - Le champ électromagnétique|EM5]]).
On a:
$$
\|\mu_{0}\overrightarrow{j}\|>>\|\frac{1}{c^{2} }\frac{ \partial E }{ \partial t } \|.
$$
Dans ce cadre, l'équation de Maxwell-Ampère devient:
$$
\overrightarrow{\mathrm{rot} }\overrightarrow{B}=\mu_{0}\overrightarrow{j}.
$$
On se place dans ce cadre pour le reste du chapitre.


# II - Le théorème d'Ampère
## 1 - Formule de Stokes
Généralisation de l'interprétation du rotationnel
Soit $\Gamma$ un contour fermé orienté.
On note $\overrightarrow{S}$ une surface orientée par la RMD, s'appuyant sur $\Gamma$

![[Phys - Formule#Formule de Stokes]]

**Rq:**
On admet que
$$
\overrightarrow{\mathrm{rot} }\overrightarrow{A}=0\iff \exists f,\;\overrightarrow{A}=\overrightarrow{ \mathrm{grad} }f.
$$

![[Phys - Formule#Equation de Maxwell-Faraday]]

Par la formule de stokes
$$
\begin{align*}
\oint_{\Gamma}\overrightarrow{E}\cdot \overrightarrow{\mathrm{d}l}&=\iint_{S}(\overrightarrow{\mathrm{rot} }\overrightarrow{E})\cdot \overrightarrow{\mathrm{d}S}&&\cr
&=\iint_{S}\left( -\frac{ \partial \overrightarrow{B} }{ \partial t }  \right)\overrightarrow{\mathrm{d}S}&&\cr
&=-\frac{ \partial  }{ \partial t } (\iint_{S}\overrightarrow{B}\cdot \overrightarrow{\mathrm{d}S})&&\cr
\end{align*}
$$

$$
e=-\frac{ \partial  }{ \partial t } \phi.
$$




## 2 - Enoncé du théorème d'Ampère
$$
\overrightarrow{\mathrm{rot}}\overrightarrow{B}=\mu_{0}\overrightarrow{\Gamma}
$$

Soit $\Gamma$ un contour fermé orienté.
$$
\oint_{\Gamma}\overrightarrow{B}\cdot \overrightarrow{\mathrm{d}l}=\iint_{S}(\overrightarrow{\mathrm{rot}}\overrightarrow{B})\cdot \overrightarrow{\mathrm{d}S}=\mu_{0}\iint_{S}\overrightarrow{j}\cdot \overrightarrow{\mathrm{d}S}
$$
On appelle courant enlacé:
$$
I_{\text{enlace}}=\iint_{S}\overrightarrow{j}\cdot \overrightarrow{\mathrm{d}S}.
$$
Algébrique, selon l'orientation de $\overrightarrow{j}$ et $\overrightarrow{dS}$.

![[Phys - Formule#Théorème d'Ampère]]

Att: $\Gamma$ doit être orienté.

## 3 - Application du théorème
A - Principe de curie
$$
\overrightarrow{F}_{\text{Lorentz}}=q\overrightarrow{E}+q\overrightarrow{v}\wedge \overrightarrow{B}.
$$
L'effet concret du champ magnétique est réalisé par $\overrightarrow{v}\wedge \overrightarrow{B}$. C'est cette grandeur qui vérifie le principe de Curie.
Cela implique.
<!-- basicblock-start -->
Prop. Champ Magnétique::
- $\overrightarrow{B}$ est orthogonal aux plans de symétrie de la distribution du courant
- $\overrightarrow{B}\in$ plans d'antisymétrie de cette distribution
<!-- basicblock-end -->

B - Choix du contour d'Ampère
On le veut orienté.
On choisit des contours telle que $\overrightarrow{B}\cdot \overrightarrow{\mathrm{d}l}=\begin{cases}0\cr\pm B\mathrm{d}l\end{cases}$.
On prends des contours telle que $\overrightarrow{B}$ soit uniforme, afin de le sortir de l'intégrale.

C - Principe de superposition
Il est conservé, de par les equations de Maxwell

# III - Exemple d'application
## 1 - Le fil infini
> [!note]- Le fil infini
![[Phys - Démo - Champ magnétique du fil infini]]
## 2 - 



