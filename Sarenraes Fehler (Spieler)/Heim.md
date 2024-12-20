```dataview
TABLE WITHOUT ID 
link(file.name) as "Journal",
Sitzungsnummer aS "Nummer",
Sitzungsdatum as "Sitzungsdatum",
sessionstatus as "Sitzungsstatus"
from #Sarenraes_Fehler/Session_Journal  
WHERE file.name != "TemplateJournal"
SORT Sitzungsnummer ASC

```

```dataview  
TABLE WITHOUT ID link(file.name) AS "Character Name", Player, Class, Race, level, Role  
from "1-Party"  
where (Role = "Player")  
where (Status = "Active")  
```

#  NPCs

```dataview  
TABLE WITHOUT ID link(file.name) AS "NPC Name", Gender, Race, Age, Location, AssociatedGroup  
FROM "3-Mechanics/NPCs"
WHERE (NoteIcon = "npc") 
SORT file.mtime DESC
LIMIT 10
```

#  Locations

```dataview  
TABLE WITHOUT ID link(file.name) AS "Location Name", type, Government, Community-Size, size, population  
FROM "2-World"
WHERE (NoteIcon = "Settlement")  
SORT file.mtime DESC
LIMIT 10
```


# Recently Modified Notes
```dataview
TABLE WITHOUT ID
    link(file.path, file.folder + " / " + file.name) AS "Note",
    file.mtime AS "Last modified"
FROM "/"
WHERE file.mtime >= date(today) - dur(30 days)
AND file.name != this.file.name
    AND !contains(file.path, "z_Assets")
    AND !contains(file.path, "Inline Scripts")
    AND !contains(file.path, "z_Templates")
    AND !contains(file.path, "daily notes")
    AND !contains(file.path, "BRAT")
SORT file.mtime DESC
LIMIT 10
```

![[Vault Bericht]]


