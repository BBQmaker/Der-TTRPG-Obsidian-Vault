---
aliases: 
NoteIcon: region
tags:
  - Sarenraes_Fehler/Ort/Region
---
# 🌍`=this.file.name`
## 🧭Kurzbeschreibung
Das Obere Unterreich, liegt bis zu 5 Km Tiefe, wird von diversen Völkern bewohnt und von noch mehr Gefährlichen Monstern. 

## 🧭Beschreibung
Als Oberes Unterreich gelten jene Bereiche, die direkt von der Oberfläche bis zu einer Tiefe von 3 Meilen hinab reichen. Sie werden von den unterschiedlichsten Rassen bevölkert. Dazu zählen Drow, Zwerge, Riesen, alle Arten von Goblins, Orks, Tiefengnome, Werratten und Chitines. Bewohner der unteren Teile des Unterreichs dringen auch recht oft in diese Gebiete vor, sei es um Handel zu treiben, oder auf der Jagd. Hier wird man auch am Ehesten noch Oberweltler finden, die eine Höhle, oder eine verlassene Mine erkunden und vielleicht auf Tunnel stießen, die in andere Bereiche des Unterreichs vordringen.


## 🗺️ Karten und Illustrationen
Karten oder Illustrationen hier.
🗺️ [Regionenkarte]

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


