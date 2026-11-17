
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
Dans l'idée, je ferais sans doute un petit programme dans le terminal.


---

Okay, je pense que je vais prendre exemple sur le système mis en place par wayland. Je rends le microkernel responsable uniquement de passer les informations correctement à un programme principal, le maestro. C'est lui ensuite qui s'occupe de décider quels programme tourne et comment, et de leur accorder des ressources.
J'ai donc besoin de deux choses, un protocole de communication entre mon kernel et mon maestro, et un entre mon maestro et les applications.
Je vais créer mon propre maestro, azalea, avec uniquement quelques fonctions basiques, et ne faisant aucune vérification sur les programmes à exécuter. Ensuite, je ferais quelques petits programmes à faire tourner dessus, et faire des comparaisons statistiques sur les programmes. Il faudra bien que je précise que l'intérêt particulier de cette approche est l'analyse qu'elle autorise au système sur les programmes qu'il exécute (théorie des graphes).

Je pense que je vais faire une petite app graphique de terminal, un shell, et quelques programmes qui tournent dedans.

Je pense que je vais faire une séparation claire entre les systèmes relevant du maestro, qui ont tout les droits, et ceux exécuté, qui se comportent dans leur propre espace.

Pour que deux programmes communiques l'un avec l'autre, il faudra que les events d'entrée de l'un soit ouvert aux events de sortie de l'autre, et vice-versa.
Quand on souhaite kill un programme, on arrête juste de register ses events de sortie.








---



Il faut que je travaille sur la distinction claire entre le kernel et le maestro. Je pense que je vais lister différents comportement usuels d'un ordinateur, et voir comment je veux split les taches. Dans l'idée, il faut que le kernel gère tout ce qui est relié au hardware, et se pose en couche d'abstraction au dessus de la machine. Le maestro au contraire s'occupe du coté software, et permet d'abstract les interactions complexes entre les applications. 
En soit, un maestro est assez petit, son unique rôle est de gérer les applications, et leurs autorisations, pour qu'elles n'accèdes pas directement au kernel. Il réagi à tout problème que peuvent avoir les applications, et les règle à leur place. C'est pratique.
Ainsi, il ne faut pas faire ...

Je pense que je vais créer ma présentation, fabriquer mon produit finis, et ensuite en déduire la construction que je dois faire de mon os.


---
# Présentation

Okay, je veux une page de présentation sur le rôle d'un os et d'un ordonnanceur dans la gestion des programmes, ainsi que les problématiques que cela entraîne. Appuyer sur le fait que dans beaucoup de programmes, on implémente un système de réactions à des événements, afin d'atteindre de l'exécution asynchrone.
Mon idée, implémenter cela directement au niveau de l'os, en laissant chaque programme définir ce qu'il veut faire en asynchrone, à quel moment (events).
Problématique: Un système centrée sur ce paradigme (même s'il est amateur), permet-il un gain en performance sur les architectures qu'ils ciblent.

1. Présentation de l'implémentation, justification du choix de séparation maestro/kernel (système de compositeur), présentation d'une application sous forme de schéma block.
2. Détail de deux applications de comparaison, avec un cas ou je suis avantagée, et un ou non. (still to find)
3. Retour sur ce que j'obtiens comme résultat, appuie sur le fait que c'est avantageux pour l'asynchronisme que ça offre, mais que ça oblige à tout re-coder.

Sources.

---

Okay, il faut donc que j'implémente tout ça, et deux applications à comparer.
Pour les applications, je dois pouvoir faire un petit jeu simple, et appuyer sur à quel point ça tourne bien sur mon jeu (je le fais en pygame, je gagne forcément).
Ensuite, je fais un programme qui doit faire des choses sur une grande quantité de donnée. Là, on verra comment il est soit compliqué d’acquérir les ressources, soit compliqués de s'exécuter dans un temps raisonnable.

Pour l'implémentation, il faut que je crée la possibilité pour un utilisateur de définir ses propres systèmes, events, et ressources.
Le rust, ça va être compliqué...
Bon, ce que je dois faire, c'est créer un protocole entre le kernel et le maestro, pour que l'un comme l'autre puisse interagir. Depuis le kernel, je dois passer les interrupts au maestro, et du coté du maestro, je dois transmettre ses demandes au kernel pour qu'il les exécutes.
Okay, je vais créer une famille d'event qui ne peuvent être échangé qu'entre le kernel et le maestro, et qui, quand émise par le maestro, déclenche immédiatement des réactions de la part du kernel, et d'autre part, ne peuvent être reçu que par le maestro quand émise par le kernel.

Ensuite, il faut que je me débrouille pour laisser assez de place aux programmes pour s'exécuter, et quand même les contrôler au travers du maestro.

Les utilités principales que je veux ici pour mon maestro vont être de transmettre des informations entre le kernel et des programmes qui s'exécutent, et aussi faire leur demande s'ils en ont. Par exemple, si un programme a besoin d'un bout de mémoire, d'accéder à l'écran, ou de lancer un autre programme. Normalement, la suite d'exécution des événements est totalement géré par l'ordonnanceur dans le kernel, donc pas besoin de s'occuper de ça, mais il faut quand même demander au kernel de charger/décharger ces différents systèmes.




---

Il me faut un système de permissions, avec chaque programmes ayant différentes de celles-ci, et permettant ou non d'accéder à ces ressources ou appelles systèmes.
Par exemple, un programme doit demander l'autorisation avant de nécessiter l'écran, le lancement d'un autre programme, ou encore l'établissement d'une connexion avec un autre programme.

Chaque autorisation se transmet ou non par défaut à tout processus engendré, et certaines peuvent être rajoutée. Ensuite, tout systèmes requérant certaines ressources qu'ils n'ont pas d'autorisations pour accéder ne pourra pas être appelés, et les events demandant des choses qui n'ont pas été autorisé pour ce programmes ne seront pas aboutis par le maestro.

Il faut juste que je trouve un moyen pour que le kernel et le maestro puisse faire ça.

---

Mon objectif est qu'un programme puisse tout simplement enchaîner ses systèmes sans problèmes avec le monde extérieur. Il faut qu'à chaque fois qu'un truc se passe, il puisse exactement le faire.

exemple
```rust
!sys hello_world(Event::start _) {
    send Event::write("Hello World");
}
```
```rust
!sys ls(Event::start e) {
    let args(s) = e;
    let files = parse(s); // supose we get rid of problems here
    files.iter(|s->send Ls::Event::Search(s)|);
}

!sys search(Ls::Event::Search s, Ressources::CurrentPath p) {
    match s {
    ".."::s' => search(s',p.upper()),
    a::"/"::s' => search(s',p.down(a)),
    s' with s'.lentgth()!=0 => search("",p.down(s')),
    "" => send Event::write(p.list_files().to_str())
    };
}
```

Bon, cela me semble un peu étrange à écrire, mais cohérent. On garde les systèmes comme des fonctions, on leur permet juste de capter des events.

---

La gestion des ressources est ma principale problématique. Que suis-je censée en faire, qu'est-ce donc qu'une ressource. Dans l'idéal, chaque programmes doit être capable de créer ses propres ressources, et les transmettre comme voulu d'un système à un autre. Le seul problème, c'est que j'ai aussi besoin de les rendre transférable d'un programme à un autre, en particulier depuis la maestro.


































