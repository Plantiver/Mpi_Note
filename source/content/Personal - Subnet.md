Okay, je vais ici essayer de définir un protocole de communication pour créer une surcouche sur internet.
On considère trois types d'entités:
- Les utilisateurs
- Les machines
- Les ips

Sur chaque ip, il peut y avoir plusieurs machines, et sur chaque machine, plusieurs utilisateurs.
On va construire un réseau de communication entre les machines à travers l'internet standard, et ensuite construire les communication entre utilisateurs sur ce sur réseaux.

Chaque machine acquiert un identifiant unique, ainsi qu'une clé publique et privée. (On ajoute à cela une date de péremption).
Pour les générer, on va utiliser des machines déjà sur le réseau pour construire une clé privé. Chaque machine parmi un pool va alors travailler à la construction de la clé, et l'envoyer, et propager la clé publique associé à la machine.





































