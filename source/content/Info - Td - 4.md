
### Exo 1
Soit $G=(S,A)$ un graphe non-orienté, sans boucle.
On note $n=|S|$ et $p=|A|$.

1. a)
Si $G$ connexe, mq que $p\geq n-1$.
Par récurrence sur $n$:
I. pour $n=1$, $p\geq_{0}$ car c'est une taille
H. Pour $n+1$, on prends l'un des sommets extrémaux $i$, on vérifie bien que le graphe induit par $S\setminus \mathrm{Set}( i )$ est bien connexe, donc par hyp de rec, On conclut

2. b)
Mq $G$ acyclique $\;\implies\;p\leq n-1$.
Par récurrence forte sur $p$ ou $n$.
I. On trace un graphe simple
H.
Supposons par l'absurde que $p\geq n$:
On considère $S'=\mathrm{Set}( i\in S,\;|\mathcal{V}_{i}|\geq 2 )$.
- Si $S'=S$:
Alors on prends un sommets, déroule son chemin, et on trouve qu'on a 1 cycle
Absurde.
- Sinon:
Alors par $G_{S'}$ est acyclique, on obtient $p'\leq n'-1$.
Or, Par définition de $S'$, $p'\geq n'$.
Absurde.

2. On prends deux graphes complets assez grand
3. Un triangle et plein de sommet dispersé

### Exo 3
1. 
Si $G$ est cyclique, alors $\exists c\in \mathcal{C}_{i}$.
Notons $j=\mathcal{C}_{i}[-1]$.
Ainsi, par les propriétés du tri topologique, $s_{i}<s_{j}$.
Or $i\to j$.
Absurde

2. 
Supposons $G$ acyclique.
Invariant: La pile donne bien un ordre topologique sur les sommets déjà empilés
Quand la pile est vide, c'est vrai.
Quand on ajoute un sommet à la pile, c'est forcément qu'on a déjà vu tout sommet qui en découle. Donc, on a bien la propriété.

Sa complexité est en $O(n)$.

3. 
On prends un point.
On fait un parcours en profondeurs.
Si à un moment, on retombe sur un sommet visité, il y a un cycle.

4. 









### Exo 6
### Exo 10
