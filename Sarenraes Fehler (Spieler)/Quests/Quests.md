### Quests Übersicht
```dataview
TABLE WITHOUT ID link(file.name) AS "Quest Name", QuestStatus AS "Status", Questgeber AS "Quest Geber", QuestOrtErhalten AS "Location", QuestSessionObtained AS "Session", Questbelohnung AS "Questbelohnung"
from #Sarenraes_Fehler/Quest 
where file.name != "TemplateQuest" AND file.name != "Tags"
```
