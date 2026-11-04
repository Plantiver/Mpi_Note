---
deck: phys
---
#todo : do the thing
# Énoncé

# Idée

# Démo
**Conductivité électrique**:
On admet que les interactions entre les électrons et les atomes d'un conducteur se modélisent par une force de Drude:
$$
\overrightarrow{F}=-\frac{m_{e} }{\tau}\overrightarrow{v}
$$
- Loi de frottement fluide
- $m_{e}$ est la masse de l'électron
- $\tau$ est le temps de relaxation du cristal
Un electron dans un conducteur subit $2^{quelque chose}$ loi de Newton:
$$
m_{e}\frac{\mathrm{d} \overrightarrow{v} }{\mathrm{d}t} = -\frac{m_{e} }{\tau}\overrightarrow{v}-e \overrightarrow{E}
$$
RSF:
$$
j\omega m_{e} \overrightarrow{v}+\frac{m_{e} }{\tau} \overrightarrow{v} = -e \overrightarrow{E}
$$
$$
\overrightarrow{v}=-\frac{e \tau}{m_{e} }\frac{\overrightarrow{E} }{1+j\omega \tau}
$$
or: $\overrightarrow{j}=-en \overrightarrow{v}$
donc: $\overrightarrow{j}=\frac{ne^{2}\tau}{m_{e} }\cdot \frac{\overrightarrow{E} }{1+j\omega \tau}$

on définit la conductivité complexe:
$$
\sigma (\omega)=\frac{\sigma_{0} }{1+j\omega \tau}
$$
avec $\sigma_{0}=\frac{ne^{2}\tau}{m_{e} }$ la conductivité statique.

Si $f<<10^{14}$Hz
<!-- basicblock-start oid="ObsSFTj3D4cHETXdsXKUlDrM" -->
Loi. D'Ohm locale::
$$
\overrightarrow{j}=\sigma_{0}\overrightarrow{E}
$$
<!-- basicblock-end -->

Prenons un conducteur cylindrique de longueur $L$ soumis à un champs $\overrightarrow{E}$ constant et uniforme.

$$
\begin{align*}
\overrightarrow{E}&=-\overrightarrow{ \mathrm{grad} }V&&\cr
&=-\frac{\mathrm{d}V}{\mathrm{d}x}\overrightarrow{e_{x} }&&\cr
&=-\frac{V(L)-V(0)}{L}\overrightarrow{e_{x} }&&\cr
&=&&\cr
\end{align*}
$$


# Conséquence
