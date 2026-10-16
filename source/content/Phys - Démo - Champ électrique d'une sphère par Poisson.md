#todo do the thing
**Énoncé:**

**Idée:**

**Démo:**

Reprenons la sphère uniforme chargée en volume:
En sphérique:
$$
\begin{align*}
\dot{\Delta} V&=\frac{1}{r^{2} }\frac{ \partial  }{ \partial r } \left( r^{2}\frac{ \partial V }{ \partial r }  \right)+\frac{1}{r^{2}\sin\theta}\frac{ \partial  }{ \partial \theta } \left( \sin\theta \frac{ \partial V }{ \partial \theta }  \right)+\frac{1}{r^{2}\sin\theta}\frac{ \partial^{2}V }{ \partial \varphi^{2} } &&\cr
\end{align*}
$$
Par les invariances:
$$
\frac{1}{r^{2} }\frac{ \partial  }{ \partial r } \left( r^{2}\frac{ \partial V }{ \partial r }  \right)=-\frac{\rho}{\varepsilon_{0} }
$$
- $r<R$:
$$
\begin{align*}
\frac{ \partial  }{ \partial r } \left( r^{2}\frac{ \partial V }{ \partial r }  \right)=&-\frac{\rho r^{2} }{\varepsilon_{0} }&&\cr
r^{2}\frac{ \partial V }{ \partial r } =&-\frac{\rho r^{3} }{3\varepsilon_{0} }+A&&\cr
\end{align*}
$$
Or $\overrightarrow{E}(0)=\overrightarrow{0}$, donc $A=0$
$$
V(r)=-\frac{\rho r^{2} }{6\varepsilon_{0} }+B
$$
- $r>R$
$$
\begin{align*}
\frac{1}{r^{2} }\frac{ \partial  }{ \partial r }\left( r^{2}\frac{ \partial V }{ \partial r }  \right) &=0&&\cr
r^{2}\frac{ \partial V }{ \partial r } &=C&&\cr
\frac{ \partial V }{ \partial r } &=\frac{C}{r^{2} }&&\cr
V(r)&=-\frac{C}{r}+D&&\cr
\end{align*}
$$
En choisissant l'origine des potentiels à l'$\infty$, on retrouve la même chose...
C'est possible de faire la même chose pour le cylindre. Mais bon...


**Conséquence:**
