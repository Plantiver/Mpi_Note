
# DM
# Exercice 1
### 1
$$
\boxed{\lim_{ n \to \infty } P_{n}=X^{3}+1}
$$
$$
\boxed{\mathrm{Rac}_{\mathbb{C}}P=\mathrm{Set}( 1,j,\bar{j} )}
$$
---
### 2
Non, $P_{n}\in \mathbb{R}[X]$, donc ses racines complexes sont deux à deux conjugués. Or, c'est un polynôme d'ordre 3, donc il ne peut pas avoir plus de deux racines non réelles. Ainsi, elles sont forcément distinctes.

---
### 3
- Par imparité du degré de $P_{n}$, $P_{n}$ possède au moins une racine réelle.
- Or, $P_{n}'=3X^{2}+\frac{1}{n}$ ne s'annule pas sur $\mathbb{R}$, donc $P_{n}$ est strictement monotone, et ne possède donc au plus une racine réelle.
Donc, $\exists!x_{n}\in \mathbb{R},\;P_{n}(x_{n})=0$.
![[Math - Sketchbook 2026-11-08 22.30.26.excalidraw.svg]]

---
### 4
- $P_{n}(0)=-1<0$
- $P_{n}(1)=\frac{1}{n}>0$
Par le Théorème des valeurs intermédiaire (TVI), $x_{n}\in[0;1]$.

---
### 5
On a:
$$
\begin{align*}
P_{n}\left( 1-\frac{1}{n} \right)&=\left( 1-\frac{1}{n} \right)^{3}+\frac{1}{n}\left( 1-\frac{1}{n} \right)-1&&\cr
&=1-\frac{3}{n}+\frac{3}{n^{2}}-\frac{1}{n^{3}}+\frac{1}{n}-\frac{1}{n^{2}}-1&&\cr
&=-\frac{2}{n}+\frac{2}{n^{2}}-\frac{1}{n^{3}}&&\cr
&=-\frac{2}{n}\left( 1-\frac{1}{n} \right)-\frac{1}{n^{3}}&&\cr
&\leq 0&&\cr
\end{align*}
$$
Et donc, par TVI, $x_{n}\in [1-\frac{1}{n};1]$.
Et donc par le théorème des gendarmes sur cette inégalité, on obtient:
$$
\boxed{\lim_{ n \to \infty } x_{n}=1}
$$
---
### 6
a)
$P_{n}$ est un polynôme scindé à racine simple sur $\mathbb{C}$ (par 2), et un polynôme annulateur de A, donc $A$ est diagonalisable, et son spectre complexe est inclus dans $\mathrm{Rac}_{\mathbb{C}}(P_{n})$.

b)
Considérons $\chi_{A}=(X-x_{n})^{p-2k}\left[ (X-\lambda_{n})(X-\bar{\lambda_{n}}) \right]^{k}$.
Alors, $\det A=(-1)^{p}(-x_{n})^{p-2k}(\lambda_{n} \bar{\lambda_{n}})^{k}=x_{n}^{p-2k}(\lambda_{n} \bar{\lambda_{n}})^{k}\underset{ n\geq 2 }{ > }0$.

---
### 7















