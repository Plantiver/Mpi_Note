---
deck: info
---



# Structure de donnée

<!-- basicblock-start oid="ObsMXisyLU8B3nhZDuTSXo1v" -->
Def. ADT::
Abstract Data Type: Un modèle mathématique pour une structure, où l'on spécifie les opérations disponible sur cette structure, et les résultat que l'on en obtient.
<!-- basicblock-end -->
<!-- basicblock-start oid="ObsCwiS7zhNJcIi8YbdEAYDU" -->
Def. ADT Pile::
- Créer une pile vide
- Ajouter un élément sur la pile
- Retirer l'élément sur le dessus de la pile.
<!-- basicblock-end -->
<!-- basicblock-start oid="ObsfM88IaN7sZDRbXcoHTdeV" -->
Def. ADT File::
- Créer une file vide
- Ajouter un élément au devant de la file
- Retirer un élément au fond de la pile.
<!-- basicblock-end -->
<!-- basicblock-start oid="Obsqu9XjYNkBW6nHtpnXaJ6G" -->
Def. ADT Union&Find::
- Créer $n$ partition vide
- Trouver la partition $k$
- Unir la partition de $i$ et $j$.
<!-- basicblock-end -->
<!-- basicblock-start oid="ObsVyDhLRLlEYY92ZIEqQ3XG" -->
Def. ADT Array::
- Créer un tableau vide à $n$ élément
- Mettre la valeur $x$ dans $i$
- Récupérer la valeur dans $i$.
<!-- basicblock-end -->
<!-- basicblock-start oid="ObspSOcXq2sreQyAq9eMAQzN" -->
Def. ADT Set::
- Créer un ensemble vide
- Ajouter $x$ à un ensemble
- Enlever $x$ à un ensemble
- Parcourir les éléments d'un ensemble
- Savoir si $x$ est dans un ensemble.
<!-- basicblock-end -->

<!-- basicblock-start oid="Obsh56uIUKMAP3yxfUX8KuQk" -->
Def. Implémentation d'un ADT::
Représentation réelle d'un ADT.
<!-- basicblock-end -->
<!-- basicblock-start oid="Obs0Xp8uokb8sWyhuIQSaaZy" -->
Def. Implémentations Union&Find::
- Tableau où $tab.(i)$ contient le représentant de $i$
- Graphe où la composante connexe de $i$ est sa classe d'aquivalence
- Forêt: un tableau où $tab.(i)$ est le parent de $i$.
<!-- basicblock-end -->
<!-- basicblock-start -->
Prop. Union par rang::
```ocaml
let rec unir_rang uf i j =
	let i = trouver uf i in
	let j = trouver uf j in
	let ri = uf.(i).rg in
	let rj = uf.(j).rg in
	if ri >= rj then
		uf.(j) <- (i, rj);
		uf.(i) <- (i, max(rj+1, ri));
	else
		uf.(i) <- (j, ri);
```
<!-- basicblock-end -->
<!-- basicblock-start -->
Prop. Good Find::
```ocaml
let rec gf uf i =
	if uf.(i) = i then i
	else let r = gf uf uf.(i) in
		uf.(i) = r;
		r;;
```
<!-- basicblock-end -->







