---
deck: info
---



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



















































