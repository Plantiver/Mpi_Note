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
> ![[Phys - Démo - Interprétation du rotationnel]]

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
> ![[Phys - Démo - Champ magnétique du fil infini]]
## 2 - Le solénoïde infini
="La bobine"
Voir schéma:
On considère une infinité de spire s'enroulant autour de 
> [!note]- Le solénoïde infini
> ![[Phys - Démo - Champ magnétique du solénoïde infini]]

Définition de l'inductance:
Vu en première année: $\phi_{p}=LI$.
Le flux propre: Le flux du champs magnétique créé par un objet dans cet objet.
Ici, $\phi_{p}=N\phi_{1}$.
Or $\phi_{1}=S\mu_{0}nI$.
Donc $L=\frac{\mu_{0}N^{2}S}{l}$.
Avec:
- $l$ la longueur
- $N$ le nombre de spire
- $S$ la surface traversée.
Ainsi $L$ est en Henry.


# IV - Les dipôles magnétostatiques
## 1 - Le moment magnétique
Pour une boucle de courant:
$$
\overrightarrow{\mathcal{m}}=SI\overrightarrow{e}.
$$
Exemple du modèle de Bohr:
On prend un atome d'hydrogène:
- noyau: 1 proton de masse $m_{p}$
- 1 electron qui gravite autour (mécanique classique) de masse $m_{e}=\frac{m_{p}}{2000}$
Approximation de Born-Oppenheimer:
$$
\begin{align*}
m_{e}\overrightarrow{a_{e}}&=\overrightarrow{F}_{p\to e}&&\cr
&=-\overrightarrow{F}_{e\to p}&&\cr
&=-m_{p}e_{p}&&\cr
\end{align*}
$$
Donc:
$$
\begin{align*}
\overrightarrow{a_{p}}&=-\frac{m_{e}}{m_{p}}\overrightarrow{a_{e}}&&\cr
|a_{p}|&=\frac{m_{e}}{m_{p}}|a_{e}|&&\cr
|a_{p}|&<<|a_{e}|&&\cr
\end{align*}
$$
On va supposer les protons fixe.

Théorème du moment cinétique appliqué à l'electron:
- $\overrightarrow{F}_{p\to e}=-\frac{e^{2}}{4\pi\varepsilon_{0}r^{2}}\overrightarrow{e_{r}}$ est une force centrale
donc:
$\overrightarrow{\mathcal{M}}_{O}=\overrightarrow{OM}\wedge \overrightarrow{F}_{p\to e}=\overrightarrow{O}$
Ainsi:
$\frac{\mathrm{d}\overrightarrow{L}_{O}}{\mathrm{d}t}=\overrightarrow{0}$
$\overrightarrow{L}_{O}=m\overrightarrow{OM}\wedge \overrightarrow{v}$ est constant
- Donc $(\overrightarrow{OM},\overrightarrow{v})\in \overrightarrow{L}_{O}^{\bot}$
Le mouvement est plan
- Constantes des aires:
$\overrightarrow{OM}=r\overrightarrow{e_{r}}$
$\overrightarrow{v}=\dot{r}\overrightarrow{e_{r}}+r\dot{\theta}\overrightarrow{e_{\theta}}$
$\overrightarrow{L}_{O}=m\overrightarrow{OM}\wedge \overrightarrow{v}=mr^{2}\dot{\theta}\overrightarrow{e_{z}}=m\mathcal{C}\overrightarrow{e_{z}}$
En notant $\mathrm{d}A$ l'aire balayé par $M$ durant un petit $\mathrm{d}t$, on trouve $\mathrm{d}A=\frac{\mathcal{C}}{2}\mathrm{d}t$.

Autre démo que $r^{2}\dot{\theta}$ est constant: par l'accélération selon $e_{\theta}$ via la seconde loi de newton.

Retour su l'electrons:
On suppose pour simplifier un mouvement circulaire.
Alors $r^{2}\dot{\theta}$ est constant, donc $\dot{\theta}$ est constant aussi, et peut s'exprimer comme $\dot{\theta}=\frac{2\pi}{T}$, avec $T$ la période de rotation.
On voir un courant:
$I=\frac{\delta q}{\mathrm{d}t}=-\frac{e}{T}$
On a donc:
$$
\begin{align*}
\overrightarrow{L}&=\frac{mR^{2}2\pi}{T}\overrightarrow{e_{z}}&&\cr
&=\frac{2m}{T}\pi R^{2}\overrightarrow{e_{z}}&&\cr
\end{align*}
$$
et, on considérant l'electrons qui tourne comme une spire (bon, il faut avoir la vision):
$$
\overrightarrow{\mathcal{m}}_{H}=I\pi R^{2}\overrightarrow{e_{z}}=-\frac{e}{T}\pi R^{2}\overrightarrow{e_{z}}
$$
$$
\begin{align*}
\overrightarrow{\mathcal{m}}_{H}&=-\frac{2m_{e}e}{T}\cdot \frac{\pi R^{2}}{2m_{e}}&&\cr
&-\frac{e}{2m_{e}}\overrightarrow{L}_{O}&&\cr
\end{align*}
$$
Donc, un electrons qui tourne autour d'un proton provoque l'apparition d'un moment magnétique.

En réalité $\overrightarrow{L}_{O}$ est quantifié (par la méca quantique): $L_{O}=n\hbar$
On appelle magnéton de Bohr:
$$
\mu_{B}=-\frac{e\hbar}{2m_{e}}
$$
Pour les matériaux réels:
- Il existe des $\overrightarrow{m}$ microscopique sur chaque atomes
- Si chaque moment est aléatoire, le moment total est nul, donc pas de propriété
- Si tout les moments sont alignés, on obtient un aimant

Ordre de grandeur:
- Petit aimant: 1 Am$^{-2}$
- Aimant: 10...
- Terre: $8\cdot10^{22}$.
Rappel: les pôles magnétiques ne sont pas alignés avec les pôles géographiques, et sont inversées

## 2 - Champ créé par un dipôle magnétique
Soit $\overrightarrow{\mathcal{m}}$ un moment magnétique observée sous approximation dipolaires:
$r>>\text{taille du dipôle}$
Alors $\overrightarrow{\mathcal{m}}$ est un dipôle magnétique
On admet
$$
\overrightarrow{B} = \frac{\mu_{0}}{4\pi}\cdot \frac{\mathcal{m}}{r^{3}}(2\cos\theta \overrightarrow{e_{r}}+\sin\theta \overrightarrow{e_{\theta}})
$$

## 3 - Actions mécaniques d'un champ extérieur sur un dipôle
Soit un dipôle magnétique $\mathcal{\overrightarrow{M}}$ dans un champ uniforme est constant $\overrightarrow{B_{0}}$.
Le couple subit:
<!-- basicblock-start -->
Prop. Action d'un champ magnétique uniforme sur un dipôle::
$$
\overrightarrow{\Gamma}=\overrightarrow{\mu}\wedge \overrightarrow{B_{0}}.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Prop. Energie potentielle d'un dipôle dans un champ magnétique::
$$
\mathcal{E}_{p}=-\overrightarrow{\mu}\cdot \overrightarrow{B_{0}}
$$
<!-- basicblock-end -->
En conséquence, 
- Les moments magnétiques s'alignent sur le champ
- La position où $\overrightarrow{\mu}$ est aligné avec $\overrightarrow{B_{0}}$ est stable, et l'inverse est instable
















