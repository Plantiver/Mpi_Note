# I - Les lois de frottements solide
# 1 - Les lois de Coulomb
Prenons un solide:
![[Drawing 2026-10-16 10.17.44.excalidraw.svg]]

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
Se rappeler que N plus petit que N ( #todo fix this): T peut facilement être nul, alors que N non.

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