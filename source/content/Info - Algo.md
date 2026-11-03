```dataview
table choice(contains(file.tags, "#todo"), "no", "yes") as Achieved
where contains(file.name, "Info - Algo - ")
sort file.name ASC
```



ceux à faire:
- kruskal
- kosaraju sharir
- chemin augmentant d'un graphe biparti