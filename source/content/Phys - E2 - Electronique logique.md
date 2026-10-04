---
deck: phys
---



# I - La logique combinatoire
Def. L'ensemble des opérations logiques pour lesquelles l'état de sortie dépend uniquement des variables d'entrée.

## 1 - Les portes logiques fondamentales
On considère deux états:
- HAUT / 1 / 5V / VRAI
- BAS    / 0 / 0V / FAUX
Les portes logiques sont des interrupteurs commandés en tension.
Toutes les portes sont considérés comme idéales, i.e.
- un courant d'entrée nul
- une impédence d'entrée infini.

Pour travailler -> besoin de l'[[Algèbre de Boole]]

### 1 - La porte Not:
Représentation ANSI/IEC:
-  1.

| e   | ~e  |
| --- | --- |
| 0   | 1   |
| 1   | 0   |

### 2 - La porte And
Représentation ANSI/IEC:
- 2.

| a   | b   | a.b |
| --- | --- | --- |
| 0   | 0   | 0   |
| 0   | 1   | 0   |
| 1   | 0   | 0   |
| 1   | 1   | 1   |
|     |     |     |
### 3 - La porte Or
- 3.

| a   | b   | a+b |
| --- | --- | --- |
| 0   | 0   | 0   |
| 0   | 1   | 1   |
| 1   | 0   | 1   |
| 1   | 1   | 1   |
|     |     |     |

## 2 - Propriété générales des opérateurs
### I - L'algèbre de Boole
Pour démontrer une égalité, on montre l'égalité des tables de vérités.
$$\forall a, a.0=0$$
$$\forall a, a+1=1$$
$$\forall a, a.1 = a$$
$$\forall a, a+0 = a$$
### II - Autres portes
- La porte Nor
- La porte Nand
- La porte Xor
- La porte Xnor

### III - Lois de morgan
$$\overline{a+b} = \overline a \cdot\overline b$$
$$\overline{a\cdot b} = \overline a+\overline b$$
Démo:

| a   | b   | $\overline a\cdot\overline b$ | $\overline a+\overline b$ | $\overline{a+b}$ | $\overline{a\cdot b}$ |
| --- | --- | ----------------------------- | ------------------------- | ---------------- | --------------------- |
| 0   | 0   | 1                             | 1                         | 1                | 1                     |
| 0   | 1   | 0                             |                           |                  |                       |
|     |     |                               |                           |                  |                       |
|     |     |                               |                           |                  |                       |
Porte Nand:
Elle permet la construction de toute les autres:
- **Not** par Nand(a,a)
- **And** par Not(Nand(a,b))
- **Or** par Nand(Not(a), Not(b))

# II - Logique séquentielle et stabilité
## 1 - Rétroaction et circuits astables

*Schéma avec 3 not en série bouclée*
En réalité, les portes ont un temps de réponse $\tau$. Et donc ici, $e(t+3\tau)=\overline{e(t)}$. On observe une oscillation.
On parle de système astable: Il n'exsite pas d'état logique stable.
Def: Logique séquentielle: L'état de sortie dépend des variables d'entrée et des états précédents de la sortie.
Il s'agit des systèmes bouclés, où ka sortie est réinjectée en entrée.

## 2 - Un exemple de circuit monostable: le convertisseur tension-fréquence.
- 4.
Filtre
- 5.
En complexe:
$$v = \frac{R}{R+\frac{1}{jC\omega}}n$$
$$(jRC\omega+1)v = jRC\omega n$$
On repasse en temporel:
$$RC\frac{dv}{dt}+v = RC\frac{du}{dt}$$
Or, $n(t)$ est la tension en sortie de porte logique. En dehors des bascule $n$ est continue, $\frac{du}{dt} = 0$.
On pose $\tau=RC$:
- $\tau (\frac{dv}{dt}) +v=0$
- $v(t) = Ae^{-t/\tau}$
Où $A$ est à determiner en fonction des C.I.

Notions:
- L'état HAUT est à la tension $e_0$
- L'état BAS est à la tension 0V
- La bascule des portes se fait à $\frac{e_{0}}{2}$
En réalité:
- $e>\frac{e_{0}}{2}$: Etat Haut
- $e<\frac{e_{0}}{2}$: Etat Bas

### Cas 1
On suppose $e(t)=e_{0}$ "depuis longtemps".
Si un état stable est atteint, le condensateur est déchargé, $n(t) = v(t) = 0$.
Si $v(t)=0$ alors $s(t)=e_{0}$
Donc, en entrée, 6.
Donc, $n=0$, et le condensateur est bien déchargé.
Donc cet état est stable, s'il est atteint.

### Cas 2
$e(t)$ bascule à $0$.
Table de vérité -> un 0 en entrée impose une sortie à 1.
donc: $n(t<0)=0$ et $n(t=0)=e_{0}$, et ce pour toute valeur de l'autre entrée.
Mais la tension aux bornes d'un condensateur est une fonction continue du temps. Donc $u_{c} = n-v$ est continue, et ainsi $n(0^+)=v(0^+)=e_{0}$.
Or $v(t) = A\cdot e^{-t/\tau}$, avec $A(t>0)=e_{0}$.

Lorsque $v(t_{b})=\frac{e_{0}}{2}$ . $e_{0}e^{-t_{b}/\tau}=e_{0}$ . $t_{b} = \frac{\ln(2)}{\tau}$, ce qui bacule la porte pendant $t_{b}$.
Rq: Les temps de bascule des portes sont négligés.

Voir schéma...
On parle de système monostable:
- L'état de sortie  $s=1$ est stable
- L'état de sortie $s=0$ est instable et dure toujours la même durée.



---


<!-- basicblock-start oid="ObsA1b2c3d4e5f6g7h8i9j0" -->
Def. Logique combinatoire::
$$
s = f(e_1, e_2, \dots, e_n)
$$
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsUFGbjqZPIOwQkVW39T6fk" -->
Def. Modèle de la porte logique::
- Impédance d'entrée infini
- Courants d'entrée nuls
- Réalise une opération logique sur les entrées, renvoyé en sortie, supposé exacte.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsTl8KsWHF4EAN6tmlfl70g" -->
Prop. Les portes à connaitre::
- La porte NOT
- La porte AND
- La porte OR
<!-- basicblock-end -->

<!-- basicblock-start oid="Obsyhv6tdc2JbyzgmxCJYMJT" -->
Prop. Loi de Morgan::
- $\overline{a+b}=\overline a\cdot\overline b$
- $\overline{a\cdot b}=\overline{a}+\overline{b}$.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsbCWug8GG5fNiAwy5BpBob" -->
Prop. Réalisation effective d'un circuit::
Tout circuit peut être réalisé exclusivement avec des portes NAND.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsoEp2tcajKmZvzlaDjihbJ" -->
Def. Système astable::
Un système bouclé qui ne possède pas d'état stable.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsFHm5WkmXQqwQA01JkRNDu" -->
Def. Système séquentielle::
Système dont la sortie est utilisée comme entrée.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsIezdKcq6JgzRthJ7yRl5R" -->
Def. Système monostable::
Système avec un unique état stable, et qui y revient en un temps caractéristique si perturbé.
<!-- basicblock-end -->

#work
<!-- basicblock-start oid="Obs3REQIkaAR9pfD3BMz38wH" -->
Def. Système bistable::
Système séquentielle avec deux états stable, dont l'on peut passer de l'un à l'autre via une commande.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsyM9M9QNRvJuNNb8DwnJWY" -->
Def. Mémoire $RS$::
- Système permettant de stocker une information
- Si $R$ appuyé, alors $Q=0$
- Si $S$ appuyé, alors $Q=0$
- Sinon, $Q^{+}=Q^{-}$.
- Pas de cas prévu pour $R$ et $S$ simultané.
<!-- basicblock-end -->

<!-- basicblock-start oid="ObsJZvxep5piQgfBvR3ingpG" -->
Prop. Les différentes mémoires $RS$::
- Inscription prioritaire
- Effacement prioritaire
- Conservatrice
- Inverseuse
<!-- basicblock-end -->


