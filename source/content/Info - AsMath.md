
# Notation
Si $u$ est un tuple, alors $\bar{u}=|u|$ est sa longueur.

# Adt
Un adt est un tuple $(A,V,\mu,P)$.
On a:
- $A$ est un ensemble d'état abstrait
- $V$ est un ensemble d'ensemble quelconque
- $\mu$ est un ensemble d'opérateur sur $A$ et les ensembles $V$
- $P$ est un ensemble de propriété sur $\mu$
### Exemple:
**Tableau:**
Soit $X$ un ensemble quelconque:
On prends:
- $A=\bigcup_{n\in \mathbb{N}}X^{n}$
- $V=\mathrm{Set}( X,\mathbb{N},E)$
- $\mu=\mathrm{Set}( i:\mathbb{N}\to A,\;s:A\times \mathbb{N}\times X\to A,\;g:A\times \mathbb{N}\to A\times (X\cup E) )$
- $P=\mathrm{Set}( p_{0},\;p_{1},\;p_{2},\;p_{3},\;p_{4},\;p_{5} )$
Avec:
- $E$ un ensemble disjoint de $X$
- $p_{0}: \forall n\in \mathbb{N},\;|i(n)|=n$
- $p_{1}: \forall a\in A,\;\forall n\in \mathbb{N},\;(n\geq \bar{a}\;\implies\;s(a)=a)$
- $p_{2}:\forall a\in A,\;\forall n\in \mathbb{N},\;(n\geq \bar{a}\;\implies\;g(a)=(a,e),\;e\in E)$
- $p_{3}:\forall x \in X,\;\forall a\in A,\;\forall n\in[0,\bar{a}-1],\;g(s(a,n,x),n)=x$
- 
#todo 


# Algorithme

# Graphe
