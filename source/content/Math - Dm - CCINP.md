

$$
a_{n}=\frac{\mu ^{n}+\lambda ^{n}}{2}
$$

avec
$$
\mu,\lambda=\frac{1\pm \sqrt{ t }}{2}
$$
d'où:
$$
a_{n}=\frac{1}{2^{n+1}}\left( \sum_{k=0}^{n}\binom{n}{k}\sqrt{ t }^{k}+\sum_{k=0}^{n}\binom{n}{k}(-\sqrt{ t })^{k} \right).
$$

donc, pour $k$ impair, ça disparaît
donc:
$$
a_{n}=\frac{1}{2^{n+1}}\sum_{k=0}^{|n/2|}\binom{n}{2k}2\sqrt{ t }^{2k}.
$$
$$
a_{n}=\frac{1}{2^{n}}\sum_{k=0}^{|n/2|}\binom{n}{2k}t^{k}.
$$
autre vois:
$$
\begin{align*}
a_{n}&=\frac{1}{2}((1+\sqrt{ t })^{n}+(1-\sqrt{ t })^{n})&&\cr
&=(1+\sqrt{ t })\sum_{k=0}^{n-1}(1+\sqrt{ t })^{k}(i(1-\sqrt{ t }))^{n-k-1}&&\cr
&= &&\cr
\end{align*}
$$


$$
a^{n}+b^{n}=a^{n}-(-b^{n})\not=a^{n}-(-b)^{n}=(a+b)\sum_{k=0}^{n-1}a^{k}(-b)^{n-k-1}
$$

pour $t\leq1$:
$$
a_{n}\leq\frac{1}{2^{n}}\sum_{k=0}^{|n/2|}\binom{n}{2k}=\frac{1}{2^{n}}2^{n-1}=\frac{1}{2}.
$$
donc pour $t\leq1$, $a_{n}$ CV.

Pour $b_{n}$:
$$
\begin{align*}
b_{n}&=\frac{1}{2\sqrt{ t }}&&\cr
\end{align*}
$$

### 9
$$
|\lambda,\mu| = \frac{1}{2}\sqrt{ 1-t }
$$
$$
|a_{n}|\leq \frac{1}{2}\left( 2\left( \frac{1}{2}\sqrt{ 1-t } \right)^{n} \right)
$$
$$
|a_{n}|\leq \frac{1}{2^{n}}\sqrt{ 1-t }^{n}=\left( \frac{\sqrt{ 1-t }}{2} \right)^{n}
$$


donc $a_{n}$ CV si $t> -3$. et alors, $\lim_{ n \to \infty }a_{n}=0$.
pour l'égalité et le reste: ...

et
$$
b_{n}=\frac{\lambda ^{n}+\mu ^{n}}{2i\sqrt{ -t }}.
$$
donc
$$
\begin{align*}
|b_{n}|&\leq \frac{1}{2\sqrt{ -t }}2\left( \frac{1}{2}\sqrt{ 1-t } \right)^{n}&&\cr
&\leq \frac{1}{\sqrt{ -t }}\left( \frac{\sqrt{ 1-t }}{2} \right)^{n}&&\cr
\end{align*}
$$

et donc pareil que l'autre...

d'après la question 7) de LOLO (thks so much $<3$ ), pour $t=-3$, ça fonctionne pas...

### 10)
D'après moi, $D=]-3;1]$, et donc:
$$
L(t)=\begin{cases}

\end{cases}
$$








