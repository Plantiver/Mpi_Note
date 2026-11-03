
Heyyy, Je vais faire plein de trucs, mais ça va juste être un peu compliqué.

Donc, construire un OS...

Donc...
Cet Os fonctionne avec des systèmes, créé à chaque appel, capturant des ressources pour leur durée de vie, et les relachant quand ils disparaissent.
Chaque system prend en paramètre un event et des ressources, et travaille dessus de manière honnète.
Ainsi, j'ai besoin d'encoder de manière unique chaque event et ressources, pour pouvoir vérifier rapidement si un système est executable, et donc l'ordonnancer.

Pour traiter ces system de manière spéciale, il faut qu'ils soient placés à la compilation dans un segment spéciale, que mon os ira lire à l'exécution. Ainsi, quand un fichier est executé, je  parse l'exécutable elf, je récupère les différents system de ce fichier, que je rajoute à ma file d'exécution. Je traite les autres fonctions dedans comme un fichier source.

Il faut que je construise d'avantage les différentes [[Tipe - Architecture]].
Il faut que je trouve un moyen de représenter les [[Tipe - Event et Component]].


Au niveau des spécifications:
- un Os en x86-64, parce que sinon ça risque d'être un peu compliqué (très peu de doc)



About the [[Tipe - Kernel]]
[[Tipe - Présentation]]


Okay, apparemment c'est un peu trop brouillon et pas assez concret. J'ai besoin de trouver de bonne métrique. Ensuite, je dois faire des [[Tipe - Benchmark]].

Je vais simplifier le tout, et arrêter de parler des ecs à chaque fois, parce que c'est de moins en moins le cœur du sujet. 
Il faut que je commence à implémenter, pour avoir quelque chose de concret sur quoi m'appuyer, une démo qui tourne sur qemu serait pas mal.

Nouvelle séance, celle du 29/09.
J'ai pu un peu plus parler de mon Tipe avec Mme Mirliaz, et il semble que ce soit jouable, mais il faut que je trouve de bon exemple sur lesquelles faire fonctionner mes test. J'aurais besoin de trouver un logiciel comparatif entre une machine "classique", et la mienne. Pour cela, je pense notamment à un programme echo, un programme donut, et l'idéal serait un compilateur, mais cela signifie le porter, ce qui est, ici, plutôt compliqué. Le fait que je sois obligée de tout recoder moi même, sans pouvoir me baser sur du code déjà fait, est assez embêtant, mais j'imagine que c'est le prix à payer quand on crée un architecture de zéro. Si j'arrive à faire une ui, cela pourra être vraiment génial, mais c'est beaucoup de boulot. De toute façons, j'ai encore beaucoup à définir pour les protocoles de communication entre système/process.

Parmi les trucs ambitieux, mais qui feront grandement avancer le projet, il y a:
- Finir la lib pour les composants et les events
- Les lires et les registers sur le kernel
- lancer un système sur le kernel
- déchiffrer un système depuis un fichier elf
- faire un terminal
- faire une fenêtre qui tourne
- faire une ui

[[Tipe - Process]]

[[Tipe - Entity]]



Alors...
Je voudrais scinder les choses en juste ce que je veux en faire, et pas forcément l'implémentation derrière, pour comme ça avoir un plan des différentes choses que j'ai à écrire.
Donc, le noyau se lance sur un coeur, initialise tout les trucs à initialiser, et se met ensuite à ordonnancer des programmes.
J'ai besoin de:
- [ ] une fonction pour choisir le système suivant
- [ ] une fonction pour récupérer toutes les ressources d'un systèmes et l'initialiser
- [ ] une fonction pour exécuter toutes les modifs faites par un systèmes
- [ ] une fonction pour émettre de nouveaux events et débloquer les systèmes concernées
- [ ] une fonction pour ajouter un système
- [ ] une fonction pour enlever un système
- [ ] mettre en place des interrupts qui déclenchent des events
- [x] une fonction pour transformer un fichier elf en process
- [x] une fonction pour load tout les systèmes d'un process
- [x] une fonction pour unload un process




okay, le système de query ne va pas être simple à mettre en place.
Il faut, à la compilation, que je transforme une fonction avec une annotation "système" en une fonction avec des arguments valides, et une structure pour renfermer ce système.

Okay, je dois pas définir une structure à chaque fois, car je ne peux pas recompiler à chaque fois, mais plutôt une structure pour les représenter, dans laquelle je vais stocker les informations que je récupère quand je parse le fichier elf.
Donc, il faut que je définisse un trait que devront implémenter les différents trucs avec une fonction pour les transformer en mon type, et c'est mon type seulement que je stockerais sur mon Os.



---
Okay, discussion avec Mirliaz, il faut d'avantage que je précise ce que je veux faire.
Je dois me concentrer sur faire quelque chose de fonctionnelle, qui laisse lieu à une petite implémentation pour comparer avec un autre os.
Tout ce dont j'ai besoin, c'est deux petits programmes, un qui tournera bien sous linux, un qui tournera bien sous Crusty.
Bon, le problème c'est qu'il faut que je puisse transposer facilement de l'un à l'autre pour faire une comparaison fair.
Dans l'idée, je ferais sans doute un petit programme dans le terminal