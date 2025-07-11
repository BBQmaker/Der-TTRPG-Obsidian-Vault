---
aliases: 
NoteIcon: region
tags:
  - Sarenraes_Fehler/Ort/Region
---
# 🌍`=this.file.name`
## 🧭Kurzbeschreibung
Liegt Über [[Oberes Unterreich]]

## 🧭Beschreibung
Beschreibung hier!

## 🏰 Siedlungen
```dataview
TABLE WITHOUT ID 
link(file.name) as "Siedlung"
from #Sarenraes_Fehler/Ort/Siedlung    
WHERE Region = link(this.file.name)  AND ( file.name != "tags" OR file.name != "TemplateSiedlungen" )
SORT Sitzungsnummer ASC
```
## 🌾 Naturstätte
```dataview
TABLE WITHOUT ID 
link(file.name) as "Naturstätte"
from #Sarenraes_Fehler/Ort/Naturstätte     
WHERE Region = link(this.file.name) AND ( file.name != "tags" OR file.name != "TemplateNaturstätte" )
SORT Sitzungsnummer ASC
```
## 🏔️ Geografische Merkmale
```dataview
TABLE WITHOUT ID 
link(file.name) as "Geografische Merkmale"
from #Sarenraes_Fehler/Ort/GeografischeMerkmale      
WHERE Region = link(this.file.name) AND ( file.name != "tags" OR file.name != "TemplateGeografischeMerkmale" )
SORT Sitzungsnummer ASC
```

## 🗺️ Karten und Illustrationen
Karten oder Illustrationen hier.
🗺️ [Regionenkarte]
