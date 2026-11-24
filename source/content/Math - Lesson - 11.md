---
deck: math
---

<!-- basicblock-start oid="Obsv7huxEgrXDg1IErKn9lv7" -->
Th. convergence d'une série à terme positif::
$$
\left( \sum u_{n} \text{ CV}\right)\iff \exists M\in \mathbb{R},\;\forall p \in \mathbb{N},\;\sum_{n=0}^{p}u_{n}\leq M.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obs95wA8SCPRz1oVK2nBJmFo" -->
Th. divergence grossière::
$$
\left( \sum u_{n}\text{ CV} \right)\;\implies\;u_{n}\underset{ n }{ \to }0.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObskqI4VzRqJXValfXN3DgLf" -->
Th. série de référence::
- $\sum_{n=p}^{+\infty}a^{n}=\frac{a^{p}}{1-a}$ si $|a|< 1$
- $\sum_{n=0}^{+\infty} \frac{1}{n^{\alpha}}$ CV ssi $\alpha>1$
- Les DSE CVA sur leur rayon de convergence.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsRXUgNpmceYuKlzNBjJ9rZ" -->
Th. comparaison sur les série à termes positifs::
- $\sum v_{n}$ CV $\;\implies\;\sum u_{n}$ CV si $u_{n}=O(v_{n})$
- $\sum u_{n}\simeq \sum v_{n}$ si $u_{n}\sim v_{n}$.
<!-- basicblock-end -->

<!-- basicblock-start oid="Obs6QDZH83yuSv7GIOaO2pG9" -->
Prop. Cauchy-Schwartz du pauvre::
$$
|ab|\leq \frac{1}{2}(a^{2}+b^{2})
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsKtW9w7Dl78v8nVbAh01w4" -->
Th. règle d'Alembert::
$$
|\frac{u_{n+1}}{u_{n}}|\underset{ n }{ \to }l,\;\begin{cases}
l<1\;\implies\;\sum u_{n}\text{ CVA} \\
l>1 \;\implies\;\sum u_{n}\text{ DVG}
\end{cases}
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsyTUPgREzsQGGHy00bd5vz" -->
Th. série spéciale alternée::
$$
\begin{cases}
(u_{n})\text{ alternée} \\
|u_{n}| \searrow_{0}
\end{cases}\;\implies\;\begin{cases}
\sum u_{n}\text{ CV} \\
\mathrm{si}\left( \sum u_{n} \right)=\mathrm{si}(u_{0}) \\
|\sum u_{n}|\leq|u_{0}|
\end{cases}
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obsmssr8sCBOY6AXbETQ7VpM" -->
Th. série télescopique::
$$
u_{n}\simeq \sum(u_{n}-u_{n+1}).
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsUDXxFtAhFhLuliW6vaEUI" -->
Th. absolu convergence en dimension finie::
$$
ACV\;\implies\;CV.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsFQ6NjQ4GtiSdQ0cw1uviI" -->
Th. relation des termes généraux de série::
$$
\begin{cases}
v_{n}\geq0 \\
u_{n}=\mathscr{R}(v_{n})
\end{cases}\;\implies\;\begin{cases}
\text{Si }\sum v_{n}\text{ CV}&\sum_{n=p+1}^{+\infty}=\mathscr{R}\left( \sum_{n=p+1}^{+\infty}v_{n} \right) \\
\text{Si }\sum v_{n}\text{ DV}&\sum_{n=0}^{p}u_{n}=\mathscr{R}\left( \sum_{n=0}^{p}v_{n} \right)
\end{cases}
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="Obs0RX2rsvJGhD8Hp4esrTgC" -->
Prop. exponentielle généralisée::
- $\mathrm{Sp}A\subset \mathrm{Sp}e^{A}$, avec égalité pour $K=\mathbb{C}$
- $e^{A+B}=e^{A}\times e^{B}$
- $(e^{A})^{-1}=e^{-A}$.
<!-- basicblock-end -->

<!-- basicblock-start oid="Obsg4yo9V6pDD9I5UG34mXNT" -->
Def. ensemble dénombrable::
$$
\exists f:X\leftrightsquigarrow \mathbb{N}.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsaDxeMX4rPZZkxHhOaO2Uu" -->
Def. somme d'une famille sommable::
$$
\sum_{i\in I}a_{i}=sup_{J\subset I\text{ fini}}\left( \sum_{j\in J}a_{j} \right)
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObstWPj7LkqFVaJlJk9B5wO5" -->
Th. sommation par paquet::
$$
\bigsqcup I_{n}=I,\;\begin{cases}
p_{n}=\sum_{i\in I_{n}}a_{i}<+\infty \\
S=\sum_{n\in \mathbb{N}}p_{n}<+\infty
\end{cases}\;\implies\;\sum_{i\in I}a_{i}=S.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsCPB8osxC5I1BAbAezfwcD" -->
Th. de Fubini::
$$
\begin{cases}
p_{n}=\sum_{m\in \mathbb{N}}|a_{n,m}|<+\infty \\
\sum_{n\in \mathbb{N}}p_{n}<+\infty
\end{cases}\;\implies\;\sum_{n\in \mathbb{N}}\sum_{m\in \mathbb{N}}a_{n,m}=\sum_{m\in \mathbb{N}}\sum_{n\in \mathbb{N}}a_{n,m}.
$$
<!-- basicblock-end -->

<!-- basicblock-start -->
Th. produit de série::
$$
\begin{cases}
\sum u_{n}\text{ ACV} \\
\sum v_{n}\text{ ACV}
\end{cases}\;\implies\;\sum u_{n}v_{n}=\sum c_{n},\;c_{n}=\sum_{p+q=n}u_{p}v_{q}.
$$
<!-- basicblock-end -->

