# Quests Übersicht
```dataview
TABLE WITHOUT ID link(file.name) AS "Quest Name", questStatus AS "Status", questGiver AS "Quest Geber", questLocationObtained AS "Location", questSessionObtained AS "Session", questLootAvail AS "Available Rewards"
from  #Sarenraes_Fehler/Quest 
where questStatus = "In Progress"
```

