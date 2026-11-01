

Pour le td:
29 sauf d), 37, 52, 56, 28 jusqu'à d) incluse
### Exo 29
a)
Supposons par l'absurde que $f$ possède deux points fixes distincts, notées $l_{1},l_{2}$.
Alors:
$$
\begin{align*}
\|f(l_{1})-f(l_{2})\|&<\|l_{1}-l_{2}\|&&\cr
\|l_{1}-l_{2}\|&<\|l_{1}-l_{2}\|&&\cr
\end{align*}
$$
Absurde.

b)
$f$ est continue car $1$-lipschitzienne, donc $\varphi$ est continue.
Ainsi, $inf_{x \in K}\varphi(x)$ est en fait un minimum, car $K$ est fermé.

Comment en déduire que $\varphi$ s'annule?

c)
Si $x_{0}=l$, alors c'est finis
Si $x_{0}\not=l$, alors:
$$
\forall n\in \mathbb{N},\;\|x_{n+1}-l\|<\|x_{n}-l\|
$$
Or, $x_{n}\in K^{\mathbb{N}}$, donc possède une VA, et l'on montre que c'est $l$.
Ainsi, APCR, $x_{n}$ est aussi proche que voulue de $l$, et d'après le résultat établi, $(x_{n})$ ne s'en éloigne plus.
Ainsi, $x_{n}\underset{ n }{ \to }l$.



### Exo 37
a)
$$
\begin{align*}
|g|&=|u(f)|&&\cr
&=\int_{0}^{1}|\int_{0}^{x}f(t)\mathrm{d}t|\mathrm{d}x&&\cr
&\leq \int_{0}^{1}\int_{0}^{x}|f(t)|\mathrm{d}t\mathrm{d}x&&\cr
&\leq \int_{0}^{1}\int_{0}^{1}|f(t)|\mathrm{d}t\mathrm{d}x&&\cr
&\leq \int_{0}^{1}|f|\mathrm{d}x&&\cr
&\leq 1\cdot|f|&&\cr
\end{align*}
$$
Donc $u$ est continue.

Cherchons maintenant $|\|u\||$. Educated guess, is it $1$?
Introduisons $f_{n}=(t\to ne^{-tn})$.

On a alors, pour $n>1$:
$$
\begin{align*}
\frac{|u(f_{n})|}{|f_{n}|}&=\frac{\int_{0}^{1}|\int_{0}^{x}ne^{-nt}\mathrm{d}t|\mathrm{d}x}{\int_{0}^{1}|ne^{-nt}|\mathrm{d}t}&&\cr
&=\frac{\int_{0}^{1}|1-e^{-nx}|\mathrm{d}x}{1-e^{-n}}&&\cr
&=\frac{1-\left( -\frac{1}{n} \right)(e^{-n}-1)}{1-e^{-n}}&&\cr
&=-\frac{1}{n}+\frac{1}{1-e^{-n}}&&\cr
&\underset{ n }{ \to }1&&\cr
\end{align*}
$$
Donc, ça fonctionne.

b)
(i) $u$ est continue car application linéaire en dimension finie, et ce peu importe la norme, car elles sont équivalentes en dim fini
(ii) Notons $i_{\text{max}}$ le $i$ tq $|a_{i}|$ soit maximal.
Alors:
$$
\begin{align*}
|u(X)|&=|\sum_{i}x_{i}a_{i}|&&\cr
&\leq \sum_{i}|a_{i_{\text{max}}}||x|&&\cr
&\leq|a_{i_{\text{max}}}|\cdot\|X\|_{1}&&\cr
&\leq|a_{i_{\text{max}}}|\cdot \sqrt{ n }\|X\|_{2}&&\cr
\end{align*}
$$
Ainsi, $\|u\|_{op}\leq|a_{i_{\text{max}}}|\cdot \sqrt{ n }$.

En prenant $X=(\mathrm{si}(a_{i}))_{i}$, on a alors:
$$
\begin{align*}
\|X\|_{2}&=\sqrt{ n }&&\cr
|u(X)|&=\sum|a_{i}|&&\cr
\end{align*}
$$
·

(iii) Notons $i_{\text{max}}$ le $i$ tq $|x_{i}|$ soit maximal.
Alors:
$$
\begin{align*}
|u(X)|&=|\sum_{i}x_{i}a_{i}|&&\cr
&\leq \sum_{i}|a_{i}|\cdot|x_{i_{\text{max}}}|&&\cr
&\leq\|A\|_{1}\cdot\|X\|_{\infty}&&\cr
\end{align*}
$$
Ainsi, $\|u\|_{op}\leq\|A\|_{1}$.
Or, en prenant $X=(\mathrm{si}(a_{i})_{i})$, on a alors:
$$
\begin{align*}
\|X\|_{\infty}&=1&&\cr
|u(X)|&=\|A\|_{1}&&\cr
\end{align*}
$$
Ainsi, $\|u\|_{op}=\|A\|_{1}$.

c)
Prenons $(\mathbb{R}[X], \|\cdot\|_{\infty})$, alors considérons:
$$
D:\begin{cases}
E\to E \cr
P\to P'
\end{cases}
$$
Alors $D\in \mathcal{L}(E)$ mais la suite des $P_{n}=X^{n}$ permet de montrer que $D\\not\in \mathcal{L}_{c}(E)$.

### Exo 52
a)
Il s'agit de la norme opérateur de l'application canoniquement associée à $A$, or nous sommes en dimension finie, et donc cette application linéaire est continue, d'où l'existence.

b)
$$
\begin{align*}
\frac{\|AX\|_{1}}{\|X\|_{1}}&=\frac{max_{j=1}^{n}\left( |\sum_{i=0}^{n}a_{i,j}x_{i} |\right)}{max_{j=1}^{n}x_{j}}&&\cr
&\leq \frac{max_{j=1}^{n}\left( \sum_{i=0}^{n}|a_{i,j}|\cdot |x_{max}| \right)}{|x_{max}|}&&\cr
&\leq max_{j=1}^{n}\left( \sum_{i=0}^{n}|a_{i,j}| \right)&&\cr
\end{align*}
$$
c)
En prenant $X=(\mathrm{si}(a_{i,j}))_{i}$, avec $j$ tq $\sum_{i=0}^{n}|a_{i,j}|$ soit maximal.
Alors,
$$
\begin{cases}
\|X\|_{1}&=1 \cr
\|AX\|_{1}&=\sum_{i=0}^{n}|a_{i,j}|
\end{cases}
$$
Ce qui conclut.

### Exo 56
a) Non, car nous sommes en dimension infini, donc ça ne découle pas directement.

b)
(i)
$u\in \mathcal{L}(E,\mathbb{R})$, ainsi, on cherche à savoir s'il existe $k$ qui convient:
$$
\begin{align*}
|u(f)|&=|f(0)|&&\cr
&\leq1\cdot\|f\|_{\infty}&&\cr
\end{align*}
$$
(ii)
$F$ est l'image réciproque par une application continue d'un fermée, donc est un fermée.

c)
(i)
En découpant l'aire en deux morceaux:
$$
\|f_{n}-c\|_{1}=\frac{1}{2}\cdot \frac{1}{n}.
$$
(ii)
$c$ est limite d'une suite d'élément de $F$, donc $c\in \bar{F}$.
Or $c\not\in F$ donc $F$ n'est pas fermé pour $\|\cdot\|_{1}$. 


### Exo 28

a)
Soit $\lambda \in \mathrm{Sp}A$.
Alors:
$$
\exists X\in \mathbb{K}^{n^{\star}},\;AX=\lambda X
$$

b)
ça fonctionne pour $X_{0}=(1)$.

c)
Soit $A,B\in \mathscr{S}$, alors:
- $A\times B$ est à coefficient positif
- $(A\times B)X_{0}=X_{0}$
Donc $A\times B\in \mathscr{S}$.

d)








