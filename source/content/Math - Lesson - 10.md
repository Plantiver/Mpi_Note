---
deck: math
---



<!-- basicblock-start oid="Obs8ljm9V8lx9421H4Y9cJTS" -->
Th. convergence dominée discret::
- $\forall t\in J,\;f_{n}(t)\underset{ n }{ \to }l(t)\in \mathcal{C}^{0}_{(m)}(J)$
- $\forall n\in \mathbb{N},\;f_{n}\in \mathcal{C}^{0}_{m}(J)$
- $\forall n\in \mathbb{N},\;\forall t\in J,\;|f_{n}(t)|\leq\varphi(t)\in \mathcal{L}^{1}(J)$
$$
l\in \mathcal{L}^{1}(J)\text{ et }\lim_{ n \to +\infty } \int_{J}f_{n}(t)\mathrm{d}t=\int_{J}l(t)\mathrm{d}t.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsnyYz9yLQprE3ovX6SB3tW" -->
Th. convergence dominée::
- $\forall t\in J,\;f(x,t)\underset{ x\to a }{ \to }l(t)$
- $\forall x \in I,\;f(x,\cdot)\in \mathcal{C}^{0}_{m}(J)$
- $\forall (x,t)\in I\times J,\;|f(x,t)|\leq\varphi(t)\in \mathcal{L}^{1}(J)$
$$
l\in \mathcal{L}^{1}(J)\text{ et }\lim_{ x \to a } \int_{J}f(x,t)\mathrm{d}t=\int_{J}l(t)\mathrm{d}t.
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsOJjqEPV2fv5f1qlleR0p8" -->
Th. continuité sous l'intégrale::
- $\forall t\in J,\;f(\cdot,t)\in \mathcal{C}^{0}(I)$
- $\forall x \in I,\;f(x,\cdot)\in \mathcal{C^{0}_{m}}(J)$
- $\forall(x,t)\in I\times J,\;|f(x,t)|\leq\varphi(t)\in \mathcal{L}^{1}(J)$
$$
g:\begin{cases}
I&\to \mathbb{K} \\
x&\to \int_{J}f(x,t)\mathrm{d}t
\end{cases}\in \mathcal{C}^{0}(I)
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsizuWirdmwX8JtqDNMsy11" -->
Th. Leibniz intégrale faible::
- $\forall t\in J,\;f(\cdot,t)\in \mathcal{C}^{1}(I)$
- $\forall x \in I,\;f(x,\cdot)\in \mathcal{L}^{1}(J)\text{ et }\frac{ \partial f }{ \partial x }(x,\cdot)\in \mathcal{L}^{1}(J)$
- $\forall(x,t)\in I\times J,\;|\frac{ \partial f }{ \partial x }(x,t)|\leq\varphi(t)\in \mathcal{L}^{1}(J)$
$$
g:\begin{cases}
I&\to \mathbb{K} \\
x&\to \int_{J}f(x,t)dt
\end{cases}\in \mathcal{C}^{1}(I)\text{ et }g'(x)=\int_{J}\frac{ \partial f }{ \partial x } (x,t)\mathrm{d}t
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObslPvOFF2qjzph23G9YrIXs" -->
Th. Leibniz intégrale fort::
- $\forall t\in J,\;f(\cdot,t)\in \mathcal{C}^{n}(I)$
- $\forall k\in[0,n],\;\forall x \in I,\;\frac{ \partial ^{k} f }{ \partial x^{k} }(x,\cdot)\in \mathcal{L}^{1}(J)$
- $\forall(x,t)\in I\times J,\;|\frac{ \partial ^{n} f }{ \partial x^{n} }(x,t)|\leq\varphi(t)\in \mathcal{L}^{1}(J)$
$$
g:\begin{cases}
I&\to \mathbb{K} \\
x&\to \int_{J}f(x,t)dt
\end{cases}\in \mathcal{C}^{1}(I)\text{ et }\forall k\in[0,n],\;g^{(k)}(x)=\int_{J}\frac{ \partial ^{k} f }{ \partial x^{k} } (x,t)\mathrm{d}t
$$
<!-- basicblock-end -->

