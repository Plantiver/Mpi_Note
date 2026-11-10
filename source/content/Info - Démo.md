---
deck: demo
---

```dataview
table choice(contains(file.tags, "#todo"),"no","yes") as Achieved
where contains(file.name, "Info - Démo - ")
sort file.name ASC
```

<!-- basicblock-start oid="ObsxZySeU8YqXFqF1Tc1vxXR" -->
Demo. Lemme de l'étoile::...
<!-- basicblock-end -->
<!-- basicblock-start oid="ObsswjoO0eiDGfuobVnkmSyK" -->
Demo. Non-contextualité des langages réguliers
<!-- basicblock-end -->
