# Énoncé
On souhaite trouver le plus cours chemin entre deux point d'un graphe pondéré, et l'on a pour s'aider une heuristique admissible sur ce graphe.

# Algorithme
```pseudo-code
Entree: G=(S,A,w), avec la poid de deux arrètes toujours positif
		h, une heuristique admissible de G
		s, notre sommet source
		t, notre sommet target
Sortie: La taille du plus court chemin et l'arbre de parenté des chemins
		Ou Rien si le sommet n'est pas accessible

F <- NouvelleFilePriorité()

d <- [+inf; |S|]
p <- [(x->x); |S|]

d[s] <- 0
F.enfiler(s,0)
Tant que u <- F.defiler() faire
	si u=t alors => (d[t],p)
	pour v dans u.voisins() faire
		si d[u]+w(u,v)<d[v] alors
			d[v] <- d[u]+w(u,v)
			p[v] <- u
			F.enfiler(v, d[v]+h(v))
	fini
fini

=> Rien
```

# Preuve
#todo : démo de correction, et de terminaison, et de complexité

# Implémentation
#todo : make it work...
```rust
pub struct graphe {[Vec<(u8,f32)>]}

pub impl graphe {
	fn a_star(&self, s:int, t:int, h:fn(u8)->f32) -> Option<[u8]> {
		let f = FilePrio::new();
		let d = (0..self.0.len).map(|i| -1).collect();
		let p = (0..self.0.len).map(|i| i).collect();
		
	}
}
```
