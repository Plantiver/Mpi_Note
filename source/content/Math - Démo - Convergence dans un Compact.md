**Énoncé:**
Soit $X\subset E$ un compact.
Soit $(u_{n})\in X^{\mathbb{N} }$ avec pour seule Valeur d'Adhérence $l\in X$.
Montrer que $(u_{n})\underset{ n }{ \to }l$.

**Idée:**
Par l'absurde, si $(u_{n})$ ne tends pas vers $l$, c'est qu'elle échappe toujours à une petite boule autour de $l$. $X$ privé de cette boule est un compact donc $(u_{n})$ possède un VA dedans, ce qui fait donc 2 VA, une contradiction.

**Démo:**
Supposons par l'absurde que $(u_{n})$ ne tend pas vers $l$. i.e.
$$
\begin{align*}
\exists\varepsilon>0,\;\forall n_{0}\in \mathbb{N},\;\exists n\geq n_{0},\;&u_{n}\not\in \dot{B}(l,\varepsilon)&&\cr
&u_{n}\in X\cap C_{E}(\dot{B}(l,\varepsilon))&&\cr
\end{align*}
$$
On note $p:\mathbb{N}\to \mathbb{N}$ l'application qui à un certains $n\in \mathbb{N}$ associe un $n_{0}\in \mathbb{N}$ telle que la propriété précédentes soit satisfaites.
On définit l'extractrice $\varphi:\mathbb{N}\to \mathbb{N}$  par récurrence par:
$$
\begin{cases}
\varphi(0)=p(0) \cr
\varphi(n+1)=p(\varphi(n)+1)
\end{cases}
$$
On démontre bien que c'est une extractrice telle que:
$$
\forall n\in \mathbb{N},\;u_{\varphi(n)}\in X\cap C_{E}(\dot{B}(l,\varepsilon)).
$$
Or $X\cap C_{E}(\dot{B}(l,\varepsilon))$ est un compact, car #todo.
Donc, $(u_{\varphi(n)})$ possède une VA dans cette ensemble.
Et donc $(u_{n})$ possède deux valeurs d'adhérence, ce qui contredis l'énoncé.

Ainsi, $(u_{n})$ converge, et par unicité de la limite:
$$
(u_{n})\underset{ n }{ \to }l
$$

**Conséquence:**
C'est très pratique pour montrer qu'une suite avec une valeur d'adhérence converge, il suffit de trouver le bon compact.