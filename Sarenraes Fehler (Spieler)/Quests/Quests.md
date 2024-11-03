
```dataview
TABLE WITHOUT ID link(file.name) AS "Quest Name", questStatus AS "Status", questGiver AS "Quest Giver", questLocationObtained AS "Location", questSessionObtained AS "Session", questLootAvail AS "Available Rewards"
from  #Sarenraes_Fehler/Quest 
where questStatus = "In Progress"
```

