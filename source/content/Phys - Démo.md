```dataview
table choice(contains(file.tags, "#todo"),"no","yes") as Achieved
where contains(file.name, "Phys - Démo - ")
sort ascending
```
