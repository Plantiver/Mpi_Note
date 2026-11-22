---
deck: math
---

<!-- basicblock-start oid="ObsNwnuvcFNalOxSVwfx4AYD" -->
Def. groupe::
- $(G,\star)$:
- $\star$ est une l.c.i.
- $\star$ est associative
- $\star$ possède un neutre $n_{g}$
- $\forall g\in G,\;\exists g^{-1}\in G,\;g\star g^{-1}=g^{-1}\star g=n_{g}$.
<!-- basicblock-end -->

<!-- basicblock-start oid="Obsuec4TgBKVD8gbFTiGOapG" -->
Prop. construction de nouveau groupe::
- Groupe produit
- Sous-groupe de groupe connu
- Groupe quotient
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsoKAao95tB9E3lZjoTmaUO" -->
Def. sous-groupe::
- $(H,\star)<(G,\star)$:
- $n_{g}\in H$
- $\forall(x,y)\in H^{2},\;x\star y\in H$
- $\forall x \in H,\;x^{-1}\in H$.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsIdP7sQg4jJbC09BZsNlPG" -->
Th. sous-groupes de $\mathbb{Z}$ de la forme::
$$a\mathbb{Z},\;a\in \mathbb{Z}.$$
<!-- basicblock-end -->

stabilité des sous groupes par intersection

<!-- basicblock-start oid="Obsn7YDq4tb7x9A0fP1rE1Ei" -->
Def. sous groupe engendré par un élément::
$$
<x> = \mathrm{Set}( x^{k},\;k\in \mathbb{Z} ) = \bigcap_{x \in H<G}^{}H.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obs6n8NevpgQQIqwgmiNKbla" -->
Def. groupe monogène::
$$
\exists x \in G,\;G = <x>
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obs4wvPTYSHMedf5QMBrSsxQ" -->
Def. morphisme de Groupe::
- $\varphi:(G,\star_{1})\to(H,\star_{2})$
- $\forall(x,y)\in G,\;\varphi(x\star_{1} y)=\varphi(x)\star_{2}\varphi(y)$.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsqM8Rr1moICqojdjXQ3iAb" -->
Def. endomorphisme::
$$
\varphi:S\to S.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsMDYHhfCylnxNT4UDUwAqJ" -->
Def. isomorphisme::
$$
\varphi:S\leftrightsquigarrow S'.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsikON1l8Es0I38jolIOiJm" -->
Def. automorphisme::
$$
\varphi:S\leftrightsquigarrow S.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsHKkBvrYcyovjIOGA4F01m" -->
Def. ensemble isomorphe::
$$
S\simeq S'\iff\exists \varphi:S\leftrightsquigarrow S'.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsOl58mo99LmRpEVsYmaoHr" -->
Def. noyau d'un morphisme de groupe::
$$
\mathrm{Ker}f = \mathrm{Set}( x \in X,\;f(x)=n_{G} ).
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsZgQaYJe1ASitG3njmpqXi" -->
Def. image d'une application::
$$
\mathrm{Im}f = f(X).
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obs9C5fK8yvwrYLEvDaPiOoL" -->
Prop. morphisme de Groupe::
- $f(n_{G})=n_{H}$
- $f(g^{-1})=f(g)^{-1}$
- $G'<G\;\implies\;f(G')<H$
- $H'<H\;\implies\;f^{-1}(H')<G$.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsMXFrBaYECMMXQpBaEjDqa" -->
Th. du Noyau::
$$
f:(G,\star_{G})\leftrightarrow (H,\star_{H})\iff \mathrm{Ker}f=\mathrm{Set}( n_{G} )
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObskKSoxYf6HgkK95vH5khmA" -->
Def. anneau::
- $(A,+,\times)$:
- $(A,+)$ est un groupe abélien
- $(A,\times)$ est un monoïde
- $\times$ est distributive sur $+$.
<!-- basicblock-end -->

<!-- basicblock-start oid="Obs18XO7JZwBxM6rtiprb5a8" -->
Def. division dans un anneau::
$$
a|b\iff\exists k\in A,\;b=k\cdot a.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsXLPj8oUx1ey2bub2L4sJq" -->
Def. inversibilité dans un anneau::
$$
a\in A^{\times}\iff\exists b\in A,\;a\times b=b\times a=1_{A}.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsD7jE5B8EajZlYUpEL2HQ2" -->
Def. groupe des inversibles d'un anneau::
$$
A^{\times}=\mathrm{Set}( x \in A,\;\exists x^{-1}\in A ).
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsfwWY2Ewfn3yKqkFFGvGNf" -->
Def. anneau intègre::
$$
\forall(a,b)\in A^{2},\;a\times b=0_{A}\implies \begin{cases}
a=0_{A}\cr b=0_{A}
\end{cases}
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obs62wV6amVMXQpgoY9N3GJ3" -->
Def. corps::
- $(\mathbb{K},+,\times)$
- $(\mathbb{K},+,\times)$ est un anneau commutatif
- $\mathbb{K}^{\times}=\mathbb{K}\setminus \mathrm{Set}( 0_{A} )$.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObstGuRJQ5dtevdLa4qMH6TK" -->
Def. bijection::
$$
f:X\leftrightsquigarrow Y\iff \begin{cases}
f:X\leftrightarrow Y \cr
f:X\rightsquigarrow Y.
\end{cases}
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obsn0nUW6AugC6FxlMHaVnzW" -->
Prop. sur/inj::
- Pour $f:X\to Y$ et $g:Y\to Z$:
- $g\circ f:X\leftrightarrow Z\;\implies\;f:X\leftrightarrow Y$
- $g\circ f:X\rightsquigarrow Y\;\implies\;g:Y\rightsquigarrow Z$.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsRs7b2LBOMX9Bc3tKsOwXi" -->
Def. élément nilpotent::
$$
\exists n\in \mathbb{N},\;x^{n}=0_{A}.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObssXhjlY8JxIyF8APPFmChS" -->
Def. élément idempotent::
$$
x\star x=x.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obs7tR5AYbvP9VlULH21FnAI" -->
Prop. construction de nouveaux anneaux::
- Anneau produit
- Sous anneau d'anneau connu
- Quotient d'un anneau par un idéal bilatère.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsDhiteosIuwQ3a5ckPTjEH" -->
Def. sous-anneau::
- $(B,+,\times)<(A,+,\times)$:
- $1_{A}\in B$
- $(B,+)<(A,+)$
- $(B,\times)$ est un monoïde.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsJ2C7DXi9ohcqVTPqxtKwv" -->
Def. morphisme d'anneau::
- $\varphi:(A,+_{A},\times_{A})\to (B,+_{B},\times_{B})$
- $\varphi(1_{A})=1_{B}$
- $\varphi$ transforme les lois respectives.
<!-- basicblock-end -->

<!-- basicblock-start oid="Obs39H84qdZ9iInqsDEH5hzz" -->
Prop. morphisme d'anneau::
- $a\in A^{\times}\implies \varphi(a)\in A'^{\times}\text{ et }\varphi(a)^{-1}=\varphi(a^{-1})$
- $B<A\implies \varphi(B)<A'$
- $B<A'\implies \varphi^{-1}(B)<A$.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsWWIkEsPgrYuGtdfsjRlp3" -->
Def. idéal::
$$
I\subset A,\;\begin{cases}
(I,+)<(A,+)\cr
AI\subset I
\end{cases}
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsejFseqSEhIBjHyqKqrKTf" -->
Prop. idéal::
- Somme et intersection d'idéal reste un idéal
- Si $\varphi$ est un morphisme d'anneau, $\mathrm{Ker}\varphi$ est un idéal
- Si $I$ est un idéal bilatère de $A$, $A/I$ est un anneau
- Si $a\in A^{\times}$ est dans $I$, alors $I=A$.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObscbZrnyX8EqJfTjGpGNMCG" -->
Def. idéal principal::
$$
I=aA,\;a\in A.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsSq5D6IJR10ecICon95YMj" -->
Def. anneau principal::
- Un anneau dont tout les idéaux sont principaux.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsXT42Ur0MDUqiCfzaL9I0s" -->
Def. idéal propre::
$$
\emptyset\subsetneq I\subsetneq A.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obss8sZDhYFiozNiy2fM9WVP" -->
Def. Idéal maximal::
- Un idéal propre contenu dans aucun autre idéal propre de l'anneau.
<!-- basicblock-end -->

<!-- basicblock-start oid="Obs0PF5IwY1pBMqi1TcmOyNz" -->
Def. $a$ et $b$ sont associés sur un anneau intègre::
$$
\exists k\in A^{\times},\;a=kb.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obsv51HHaiDIFxQ4Tq8jFYvL" -->
Prop. taylor polynôme::
$$
\begin{align}
\phantom{`}P(X+a)&=\sum_{k=0}^{n}\frac{P^{(k)}(a)}{k!}X^{k}\phantom{`}\cr
\phantom{`}P(X)&=\sum_{k=0}^{n}\frac{P^{(k)}(a)}{k!}(X-a)^{k}.\phantom{`}
\end{align}
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObslC8DSvFwc4Svo1l05If6o" -->
Th. division Euclidienne de polynômes::
$$
\forall(A,B)\in\mathbb{K}[X]^{\star^{2} },\;\exists!(Q,R)\in \mathbb{K}[X]^{2},\;\begin{cases}
A=BQ+R \cr
\mathrm{deg}R<\mathrm{deg}B
\end{cases}.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsDiLLDRzF9HvOrEPdXnUFV" -->
Th. equivalence entre racine et divisibilité::
$$
P(\alpha)=0\iff(X-\alpha)|P
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsW2GS4ghs6gNP7JUf9CWq7" -->
Def. ordre de multiplicité d'une racine::
- $P^{(m-1)}(\alpha)=0$ et $P^{(m)}(\alpha)\not=0$
- $(X-\alpha)^{m-1}|P$ et $(X-\alpha)^{m}\not| P$.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsD3akoMicYpPSIh74NmyqA" -->
Def. racine simple et multiple::
- $\alpha$ est racine simple si $m_{P}(\alpha)=1$
- $\alpha$ est racine multiple si $m_{P}(\alpha)>1$.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsRK1owGNNvlPvGiBvzuu0a" -->
Def. polynôme scindé::
$$
\exists(\alpha_{i})\in \mathbb{K}^{n},\;P=a_{n}\prod_{i=1}^{n}(X-\alpha_{i}).
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsJAAHu1EWJzZ653KU2ThSc" -->
Th. d'Alembert Gauss::
$$
\forall P\in \mathbb{C}[X],\;\mathrm{deg}P\geq 1,\;\exists\alpha \in \mathbb{C},\;(X-\alpha)|P
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsYSbGvmxRPqi9HSd0dAeJa" -->
Th. formule de Viète::
$$
\phantom{`}\forall k\in[1;n],\;\sigma_{k}=\sum_{I\in \mathscr{P}_{k}([1;n])}\prod_{i\in I}\alpha_{i}=(-1)^{k}\frac{a_{n-k} }{a_{n} }.\phantom{`}
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsgLH5hWHhtyMZVvgtbLH2w" -->
Prop. polynôme à coefficient réel::
- Racines complexes deux à deux conjugués
- Si $\mathrm{deg}P$ est impair,alors $P$ possède une racine réelle.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsRBZNcNAJErSn6iutSLXsS" -->
Def. PPCM de $a$ et $b$ dans $A$::
$$
a\lor b\in A,\;aA\cap bA=(a\lor b)A.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObseLvZUajhc3AOPwscKFymd" -->
Def. PGCD de $a$ et $b$ dans A::
$$
a\wedge b\in A,\;aA+bA=(a\wedge b)A.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsgRqgT6sVl28kXhGk9oIRB" -->
Th. de Bézout::
$$
\forall(a,b)\in A^{2},\exists(u,v)\in A^{2},\;au+bv=a\wedge b.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsLH74gv5MfXqPLbkF3k9ro" -->
Th. de Gauss::
$$
\begin{cases}
a|bc\cr
a\wedge b=1
\end{cases}\implies a|c.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obshyum86iFLltwM6E2Hi4hI" -->
Def. polynôme de Lagrange::
$$
\mathrm{Set}( a_{i} )\in \mathbb{K},L_{i}=\prod_{j\in[1,n]\setminus \mathrm{Set}( i )}\frac{X-a_{j} }{a_{i}-a_{j} }
$$
<!-- basicblock-end -->

