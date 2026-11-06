On se place dans $\mathcal{R_{géo}}$ non galiléen vu dans $\mathcal{R_{hél}}$ considéré galiléen.
Système: {masse $m$ d'eau sur Terre}

Par la seconde loi de Newton:
$$
m\overrightarrow{a}=\overrightarrow{f}+m\overrightarrow{g}+\overrightarrow{F_{ie}}+\overrightarrow{F_{ic}}
$$
avec
$$
\begin{align*}
\overrightarrow{F_{ie}}=&-m\overrightarrow{a_{e}}&&\cr
\overrightarrow{F_{ic}}=&\overrightarrow{0}\text{ (pas de rotation)}&&&\cr
\end{align*}
$$
Or $\mathcal{R_{géo}}$ est en translation elliptique dans $\mathcal{R_{hél}}$.
Donc:
$$
\overrightarrow{a_{e}}=\overrightarrow{a}(G/\mathcal{R_{hél}}).
$$
Si on applique la 2nd loi de Newton à la Terre, on a:
$$
M_{T}\overrightarrow{a}(G/\mathcal{R_{hél}})=\overrightarrow{F}_{\text{graviationnel}\to\text{Terre}}
$$

**Effet de la Lune uniquement:**
Le système $M$ est attiré par la Lune, donc:
$$
\overrightarrow{f}+\overrightarrow{F_{ie}}=m(\overrightarrow{\alpha}(M)-\overrightarrow{\alpha}(G))
$$
avec $\overrightarrow{\alpha}$ le champ gravitationnel de la Lune:
$$
\overrightarrow{F}_{\text{Lune}\to\text{Terre}}=M\overrightarrow{\alpha}.
$$
Donc
$$
M_{T}\overrightarrow{a}(G/\mathcal{R_{hél}})=M_{T}\overrightarrow{\alpha}(G).
$$
De plus, par théorème de Gauss gravitationnel
$$
\overrightarrow{\alpha}(M)=\mathscr{G}\frac{M_{L}}{ML^{3}}\overrightarrow{ML}.
$$
On appelle force différentielle de marées
$$
\begin{align*}
\overrightarrow{F}_{\text{marées}}&=\overrightarrow{f}_{\text{Lune}\to\text{système}}+\overrightarrow{F_{ie}}&&\cr
&=m(\overrightarrow{\alpha}(M)-\overrightarrow{\alpha}(G))&&\cr
&=m\mathscr{G}M_{L}\left( \frac{\overrightarrow{ML}}{ML^{3}}-\frac{\overrightarrow{GL}}{GL^{3}} \right)&&\cr
\end{align*}
$$
$$
\overrightarrow{GL}=(R_{T}+d_{TL})\overrightarrow{e_{x}}
$$
Et l'on a $d_{TL}>>R_{T}$.
Donc
$$
\begin{align*}
\overrightarrow{ML}&=\overrightarrow{MG}+\overrightarrow{GL}&&\cr
&=R_{T}(-\cos\lambda \overrightarrow{e_{x}}-\sin\lambda \overrightarrow{e_{y}})+a\overrightarrow{e_{x}}&&\cr
|ML|^{2}&=R_{T}^{2}\sin ^{2}\lambda+(a-R_{T}\cos\lambda)^{2}&&\cr
&=R_{T}^{2}\sin ^{2}\lambda+a^{2}-2aR_{T}\cos\lambda+R_{T}^{2}\cos ^{2}\lambda &&\cr
&=R_{T}^{2}-2aR_{T}\cos\lambda+a^{2}&&\cr
&=a^{2}\left( 1-2\frac{R_{T}}{a}\cos\lambda+\left( \frac{R_{T}}{a} \right)^{2} \right)&&\cr
\end{align*}
$$
Or $R_{T}<<a$ donc
$$
\begin{align*}
\frac{1}{ML^{3}}&=\frac{1}{\left[ a^{2}\left( 1-\frac{2R_{T}}{a}\cos\lambda \right) \right]^{3/2} }&&\cr
&=\frac{1}{a^{3}}\left( 1+\frac{3R_{T}}{a}\cos\lambda \right)&&\cr
\end{align*}
$$
Donc
$$
\begin{align*}
\frac{\overrightarrow{ML}}{ML^{3}}-\frac{\overrightarrow{GL}}{GL^{3}}&=\frac{(a-R_{T}\cos\lambda)\overrightarrow{e_{x}}-R_{T}\sin\lambda \overrightarrow{e_{y}}}{a^{3}}\left( 1+\frac{3R_{T}}{a}\cos\lambda \right)-\frac{1}{a^{2}}\overrightarrow{e_{x}}&&\cr
&=\frac{1}{a^{2}}\left[ \left[ \left( 1-\frac{R_{T}}{a}\cos\lambda \right)\left( 1+\frac{3R_{T}}{a}\cos\lambda \right)-1 \right]\overrightarrow{e_{x}}-\frac{R_{T}}{a}\sin\lambda\left( 1+\frac{3R_{T}}{a}\cos\lambda \right)\overrightarrow{e_{y}} \right] &&\cr
&=\frac{1}{a^{2}}\left[ \frac{2R_{T}}{a}\cos\lambda \overrightarrow{e_{x}}-\frac{R_{T}}{a}\sin\lambda \overrightarrow{e_{y}} \right] &&\cr
&=\frac{R_{T}}{a^{3}}\left[ 2\cos\lambda \overrightarrow{e_{x}}-\sin\lambda \overrightarrow{e_{y}} \right] &&\cr
\end{align*}
$$
Donc la force de marée est
$$
\overrightarrow{F}_{\text{marée}}=m\mathscr{G}M_{L}\frac{R_{T}}{a^{3}}(2\cos\lambda \overrightarrow{e_{x}}-\sin\lambda \overrightarrow{e_{y}})
$$
Joli schéma...
Les points alignées sur $GL$ sont fortement attirés : cela arrive deux fois par jour avec la rotation de la Terre. Donc, le cycle des marées dure environ 12 h.

On définit $g_{\text{marée}=\mathscr{G}M_{L}\frac{R_{T}}{a^{3}}}$.
$$
\left( \frac{g_{\text{marée}}}{g} \right)_{\text{lune}}=5,7\cdot10^{-8}
$$
$$
\left( \frac{g_{\text{marée}}}{g} \right)_{\text{soleil}}=2,6\cdot10^{-8}
$$
$$
\left( \frac{g_{\text{marée}}}{g} \right)_{\text{autre}}\sim10^{-10}
$$
On a donc, selon l'alignement de la Terre, de la Lune, et du Soleil, des effets qui se compensent ou se renforcent.














