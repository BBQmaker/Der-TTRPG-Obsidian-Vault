![[Hintergrund des Sarenraes Fehler#Kurzzusammenfassung]]


Wir [[Die Furiosen Vier]] sind Bürger in der [[Vermis]]


## Sitzungs Journals
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
## PCs
```dataview  
TABLE WITHOUT ID link(file.name) AS "Name des Charakters", Spieler, Klasse, Spezies, level, Status 
from #Sarenraes_Fehler/Personen/Spielercharakter 
Where file.name != "TemplateSpielercharakter" and file.name != "Tags"
```
## Quests
```dataview
TABLE WITHOUT ID link(file.name) AS "Quest Name", QuestStatus AS "Status", Questgeber AS "Quest Geber", QuestOrtErhalten AS "Location", QuestSessionObtained AS "Session", Questbelohnung AS "Questbelohnung"
from #Sarenraes_Fehler/Quest 
where file.name != "TemplateQuest"
```
##  NPCs
```dataview  
TABLE WITHOUT ID link(file.name) AS "NPC Namen", Spezies, Alter, Letzter_Bekannter_Aufenthalts_Ort, AssoziierteGruppe, Status  
FROM #Sarenraes_Fehler/Personen/NPC 
Where file.name != "TemplateNPC" and file.name != "Tags"
SORT file.mtime DESC
```

##  Orte
```dataview  
TABLE WITHOUT ID link(file.name) AS "Ort Name" 
FROM #Sarenraes_Fehler/Ort 
WHERE file.name != "TemplateOrt" and file.name != "Tags"
SORT file.mtime DESC
```

# Quests Übersicht
```dataview
TABLE WITHOUT ID link(file.name) AS "Quest Name", QuestStatus AS "Status", Questgeber AS "Quest Geber", QuestOrtErhalten AS "Location", QuestSessionObtained AS "Session", Questbelohnung AS "Questbelohnung"
from #Sarenraes_Fehler/Quest 
where file.name != "TemplateQuest"
```


## Recently Modified Notes
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



