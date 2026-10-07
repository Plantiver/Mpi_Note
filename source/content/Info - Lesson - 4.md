---
deck: info
---




# Notation
$G=(S,A)$ est un graphe.
$S\subset \mathbb{N}$ sont les sommets de $G$.
$A\subset S\times\Sigma \times S$ sont les arrêtes de $G$.
Si $(i,a,j)\in A$, on note $i\underset{ a }{ \to }j$.
Si le graphe est non-orienté (i.e. $i\underset{ a }{ \to  }j\implies j\underset{ a }{ \to }i$), on notera simplement $i\underset{a}{\leftrightarrow}j$.
Le graphe est dit anonyme ssi $|\Sigma|=1$, et dans ce cas on notera $i\to j$ pour $i\underset{ a }{ \to }j$.
Un chemin de $G$ est une suite de sommet et d'arrêtes tel que $c\in S\times(\Sigma \times S)^{k}$, et $k$ est appelée la longueur du chemin.
Pour $c=(i,a_{1},j_{1},\dots,a_{k},j_{k})$, on notera $c=i\underset{ a_{1} }{ \to }j_{1}\underset{ a_{2} }{ \to }\dots \underset{ a_{k} }{ \to }j_{k}$.

Lorsqu'il n'y a pas d'ambiguïté sur $G$, on ne notera pas la dépendance en $G$.

On note $\mathcal{C}^{k}(G)$ les chemins de longueurs $k$ de $G$.
On note $\mathcal{C}^{k}_{i,j}(G)$ les chemins de longueurs $k$ de $G$ qui commencent par $i$ et finissent par $j$.
On note $\mathcal{C}_{i,j}(G)$ les chemins de $G$ qui commencent par $i$ et finissent par $j$.
On notera plus simplement $\mathcal{C}_{i}(G)$ pour $\mathcal{C}_{i,i}(G)$ les cycles de $G$.

On dit que $G$ est acyclique ssi $\forall i\in S,\;\mathcal{C}_{i}(G)=\emptyset$.

On note $i\to^{k}j$ pour $\exists c\in \mathcal{C}^{k}_{_{i,j}}(G)$.
On note $i\to^{\star}j$ pour $\exists c\in \mathcal{C}_{i,j}(G)$.

On dit que $G$ est connexe ssi $\forall i,j\in S,\;i\to^{\star}j\vee j\to^{\star}i$.
On dit que $G$ est fortement connexe ssi $\forall i,j\in S,\;i\to ^{\star}j$.
On appelle sous-graphe $G'=(S',A')$, avec $\forall i\underset{ a }{ \to }j\in A',\;(i,j)\in S'^{2}$.
On appelle graphe induit sur $G$ par $S'$ et l'on note le graphe $G_{|S'}=(S',A\cap S'\times\Sigma \times S')$.
On appelle composante connexe de $G$ les graphe induit sur $G$ connexe maximaux par le nombre de sommet.

On note $\mathscr{C}(G)$ l'ensemble des composantes connexes de $G$.

Prop. Si $G$ est connexe ssi $\mathscr{C}(G)=\mathrm{Set}( G )$.

On note:
- $\mathbb{G}$ l'ensemble des graphes
- $\mathbb{G}_{n}$ l'ensemble des graphes anonymes à $n$ sommets
- $\mathbb{G}^{k}$ l'ensemble des graphes sur des alphabets à $k$ éléments
- $\mathbb{G}_{n}^{k}$ l'ensemble des graphes à $n$ sommets sur des alphabets à $k$ éléments.

On définit $\mathcal{V}_{i}=\mathrm{Set}( j\in S,\;\exists a\in\Sigma ,\;i\underset{ a }{ \to }j\in A )$ l'ensemble des voisins de $i$.

Dans la suite, on note $n=|S|$ et $m=|A|$.

# Parcours
Un parcours est une application $p:\mathbb{G}\times S\to([1,|S|]\to S)$.
C'est une application qui crée un ordre sur les sommets à partir d'un graphe et l'un de ses sommets.

On définit un ordre initial sur $X\subset S$ et sur $\sigma \subset\Sigma$, et l'on notera $\mathrm{min}_{X}$ et $\mathrm{min}_{\sigma}$ les minimums respectifs de $X$ et $\sigma$. (obligatoire pour avoir des algorithmes déterministe (à montrer)).

### Parcours en profondeurs
$$
p:(G,i)\to  \left(o:\begin{cases}
[1,|S|]&\to S \cr
k&\to o'[k\times X\to \begin{cases}

\end{cases}](k,\emptyset)
\end{cases}\right)
$$


# Graphe anonyme acyclique
Soit $G$ comme dans le titre.
Quitte à s'intéresser au composantes connexes de $G$, on peut assumer que $G$ est connexe.














<!-- basicblock-start oid="ObsgtZcqezdF63K13ZZlj02G" -->
Def. Graphe::
$$
G = (S,A),\;A\subset S^{2}.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obs8XG3gYmFcVuVSRuQLChFp" -->
Def. Graphe non-orienté::
$$
(x,y)\in A\;\implies\;(y,x)\in A.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsXHi0hIYsk7RQ0g304NofZ" -->
Def. Graphe pondéré::
$$
\forall a\in A,\;p(a)\in \mathbb{R}.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsSqiB58MQtfsxU5ydEUtSw" -->
Prop. Implémentation d'un graphe par liste d'adjacence::
- On stock les sommets dans un tableau
- Chaque sommet est une liste des sommets qui en découlent.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsQNVFHVlsi5zEhef5ypfbD" -->
Prop. Implémentation d'un graphe par matrice d'adjacence::
- On stock tout les sommet dans une grande matrice
- Le coefficient $G_{i,j}$ est le poids de l'arc $(i,j)$ s'il existe, $+\infty$ sinon.
<!-- basicblock-end -->

<!-- basicblock-start oid="Obs8vjWi3CV5JwM0PKgX6lsH" -->
Def. Graphe transposée::
$$
^{t}G=(S,^{t}A),\;^{t}A=\mathrm{Set}( (y,x),\;(x,y)\in A ).
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsApj3o1SWjyeEe1fwtSlw3" -->
Def. Graphe induit::
$$
S'\subset S,\;G_{S'}=(S',A\cap S'^{2}).
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsCM7FwTSZnNDKCO6KcNCRw" -->
Def. Chemin d'un graphe::
$$
C\in A^{n},\;\forall i\in[1,n-1],\;C_{i,2}=C_{i+1,1}.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obs6FPShnAZNTvcvO4bmd7Fb" -->
Def. Cycle d'un graphe::
- $C$ est un chemin de G
- $C_{1,1}=C_{-1,2}$.
<!-- basicblock-end -->

<!-- basicblock-start oid="Obslw1BxshPHamEHMJDiUFHr" -->
Def. Chemin et Cycle élémentaire::
$$
\forall (x,y)\in C,\;\mathrm{deg}^{+}(y)=1,\;\mathrm{deg}^{-}(x)=1.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsA98cS4OGsaFrap9gOTct2" -->
Def. Graphe acyclique::
- Pas de cycle dans G.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObstjNsQFctOSjrj6h4aiQbk" -->
Def. Graphe connexe::
$$
\forall(u,v)\in S^{2},\;u\to^{\star}v.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obsf6wLyxjjkQDoLLsuvIFSB" -->
Def. Composante Connexe d'un graphe::
- $P\in S$ maximal
- $G_{|P}$ est connexe.
<!-- basicblock-en\tod -->

<!-- basicblock-start oid="Obsf6wLyxjjkQDoLLsuvIFSB" -->
Def. Cycle absorbant::
- Un cycle de poids négatif.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsfhA17iddhtZfZ3VXmoHaw" -->
Def. Heuristique admissible::
- $h_{t}(t)=0$
- si $u\underset{ d }{ \to }t$, alors $h_{t}(u)\leq d$.
<!-- basicblock-end -->



















































