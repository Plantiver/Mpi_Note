```dataview
table choice(contains(file.tags, "#todo"),"no","yes") as Achieved
where contains(file.name, "Info - Démo - ")
sort ascending
```
