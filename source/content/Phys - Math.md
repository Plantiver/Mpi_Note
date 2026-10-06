---
deck: phys
---




# Analyse vectorielle

### Opérateur nabla
<!-- basicblock-start oid="ObsQs4dxCozdUidfFJoM87Ta" -->
Def. Opérateur nabla::
$$
\overrightarrow{\nabla}=\begin{pmatrix}
\frac{ \partial  }{ \partial x }  \cr
\frac{ \partial  }{ \partial y }  \cr
\frac{ \partial  }{ \partial z } 
\end{pmatrix}
$$
<!-- basicblock-end -->

### Opérateur gradient
<!-- basicblock-start oid="ObseS13l3QgyjzwoweoHEr4M" -->
Def. Opérateur gradient::
$$
\overrightarrow{grad}f=\overrightarrow{\nabla}f
$$
<!-- basicblock-end -->

### Opérateur divergence
<!-- basicblock-start oid="ObsyduipQ7uZ9NBPZbSHBHSf" -->
Def. Opérateur divergence::
$$
\mathrm{div}\overrightarrow{f}=\overrightarrow{\nabla}\cdot \overrightarrow{f}
$$
<!-- basicblock-end -->

### Opérateur rotationnel
<!-- basicblock-start oid="Obsj06n3JnMPAKM1896l9JgQ" -->
Def. Opérateur rotationnel::
$$
\overrightarrow{rot}\overrightarrow{f}=\overrightarrow{\nabla}\wedge \overrightarrow{f}
$$
<!-- basicblock-end -->

### Opérateur Laplacien
<!-- basicblock-start oid="ObsZF0qqNB0pyKkt5ZsOXaQ4" -->
Def. Laplacien::
$$
\dot{\Delta}=\overrightarrow{\nabla}^{2}
$$
<!-- basicblock-end -->

### La différentielle
<!-- basicblock-start oid="Obs0SWEnJ3SOowUzU31DK5yQ" -->
Def. La différentielle::
$$
df=(\overrightarrow{\mathrm{grad} }f)\cdot \overrightarrow{dl}=\frac{ \partial y }{ \partial x }\mathrm{d}x+\frac{ \partial f }{ \partial y }\mathrm{d}y+\frac{ \partial f }{ \partial z }\mathrm{d}z  
$$
<!-- basicblock-end -->

### Développement limité
<!-- basicblock-start oid="ObsFqP8mxQ351ofJFjyzU8Tn" -->
Prop. Dév Limité de $f$ en $M$ proche de $O$::
$$
f(M)\simeq f(O)+\overrightarrow{OM}\cdot (\overrightarrow{\mathrm{grad} }f)(O)
$$
<!-- basicblock-end -->

### Gradient en cilyndrique
<!-- basicblock-start oid="ObsuDNGXnvGGTKyyE1ex9eiD" -->
Prop. Gradient en cylindrique::
$$
\overrightarrow{ \mathrm{grad} }f=\frac{ \partial f }{ \partial r } \overrightarrow{e_{r} }+\frac{1}{r}\frac{ \partial f }{ \partial \theta } \overrightarrow{u_{\theta} }+\frac{ \partial f }{ \partial z } \overrightarrow{u_z}
$$
<!-- basicblock-end -->

### Divergence en sphérique
$$
\mathrm{div}\overrightarrow{E}=\frac{1}{r^{2} }\frac{ \partial r^{2}E_{r} }{ \partial r } +\frac{1}{r\sin\varphi}\frac{ \partial E_{\theta} }{ \partial \theta } +\frac{1}{r\sin}\frac{ \partial \sin\theta E_{\varphi} }{ \partial \varphi } 
$$

### Flux d'un champ
<!-- basicblock-start oid="ObsY5eoU8nrV34tH2QaubLww" -->
Def. Flux d'un champ $\overrightarrow{A}$ sur une surface orientée $\overrightarrow{S}$::
$$
\varphi=\iint_{S}\overrightarrow{A}\cdot \overrightarrow{\mathrm{d}S}
$$
<!-- basicblock-end -->



















