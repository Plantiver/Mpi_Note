# Énoncé
On considère un fil parcourue par un courant $I$ constant et uniforme.
On veut calculer $\overrightarrow{B}$.
# Idée
On applique la méthode et on l'apprends
# Démo
On se place en coordonnée cylindrique, et l'on oriente le fil le long de l'axe $O_{z}$.

1. Invariance et symétrie
- Invariance par translation selon $z$ et par rotation d'angle $\theta$.
- Pour $M$ quelconque, $(M,\overrightarrow{e_{r}},\overrightarrow{e_{z}})$ est un plan de symétrie.
Donc: $\overrightarrow{B}=B(r)\overrightarrow{e_{\theta}}$.
2. Choix du contour d'Ampère
On prend un cercle $\Gamma$ de centre $O$ passant par $M$, orienté dans le sens de $\overrightarrow{e_{\theta}}$. 
$$
\begin{align*}
\oint_{\Gamma}\overrightarrow{B}\cdot \overrightarrow{\mathrm{d}l}&=\oint_{\Gamma}B(r)\mathrm{d}l&&\cr
&=2\pi rB(r)&&\cr
\end{align*}
$$
3. Application du théorème
$$
\oint_{\Gamma}\overrightarrow{B}\cdot \overrightarrow{\mathrm{d}l}=\mu_{0}I_{\text{enl}}
$$
Ici, $I_{\text{enl}}=I$, donc:
$$
B(r)=\frac{\mu_{0}I}{2\pi r}.
$$
# Conséquence
Pratique...