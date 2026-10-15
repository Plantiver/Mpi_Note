

**Énoncé:**
On place une infinité de spires enroulées autour de l'axe $O_{z}$. Parcourue par un courant $I$.
On veut calculer $\overrightarrow{B}$.

**Idée:**
#todo 

**Démo:**
1. Invariance et symétrie
- Invariance par translation selon $z$ et par rotation d'angle $\theta$.
- Pour $M$ quelconque, $(M,\overrightarrow{e_{r}},\overrightarrow{e_{\theta}})$ est un plan de symétrie
Donc: $\overrightarrow{B}=B(r)\overrightarrow{e_{z}}$.

2. Choix du contour d'Ampère
On prend un rectangle $(ABCD)$.
Donc
$$
\begin{align*}
\oint_{ABCD}\overrightarrow{B}\cdot \overrightarrow{\mathrm{d}l}&=\int_{AB}\overrightarrow{B}\cdot \overrightarrow{\mathrm{d}l}+\int_{BC}\overrightarrow{B}\cdot \overrightarrow{\mathrm{d}l}+\int_{CD}\overrightarrow{B}\cdot \overrightarrow{\mathrm{d}l}&&\cr
&=\int_{AB}B\mathrm{d}l+0-\int_{CD}B\mathrm{d}l+0&&\cr
&=(B(r_{1})-B(r_{2}))L&&\cr
\end{align*}
$$
3. Application du théorème
$$
\oint_{\Gamma}\overrightarrow{B}\cdot \overrightarrow{\mathrm{d}l}=\mu_{0}I_{\text{enl}}
$$
- Si le rectangle est à l'intérieur ou à l'extérieur des spires:
Alors $I_{\text{enl}}=0$.
Donc, $B(r_{1})=B(r_{2})$.
Ainsi, le champs est uniforme à l'extérieur et à l'intérieur.

- Si le rectangle passe par l'intérieur et l'extérieur
$$
\begin{align*}
\oint \overrightarrow{B}\cdot \overrightarrow{\mathrm{d}l}&=(B_{\text{int}}-B_{\text{ext}})L&&\cr
&=NI&&\cr
\end{align*}
$$
Avec $N$ le nombre de spire sur la longueur $L$.
On définit la densité linéique de spires:
<!-- basicblock-start -->
Def. Densité linéique de spires::
$$
n=\frac{N_{\text{tot}}}{L_{\text{tot}}}
$$
<!-- basicblock-end -->
D'où:
$$
B_{\text{int}}-B_{\text{ext}}=\mu_{0}nI.
$$

On ADMET $B_{\text{ext}}=0$.
D'où:
$$
\overrightarrow{B}=\begin{cases}
\overrightarrow{0}&\text{ à l'extérieur} \cr
\mu_{0}nI\overrightarrow{e_{z}}&\text{ à l'intérieur}
\end{cases}
$$

**Conséquence:**
Cela nous permet de développer un modèle pour la bobine.