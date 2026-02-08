---
aliases: []
NoteIcon: region
tags:
  - Sarenraes_Fehler/Ort/Region
---
# 🌍`=this.file.name`
## 🧭Kurzbeschreibung
Heimatland der Ulfen
#Sarenraes_Fehler/To_Do 

## 🧭Beschreibung
Das Heimatland der Ulfen zeichnet sich aus durch die Dualität von dem Harschen bergigen Norden mit Weiten unbesiedelten gebieten wo sich Winter wölfe, Mamuts, Jotunneber und viele andere Tiere Leben. und das Fruchtbare Tiefland was von Viele Kleine Flüssen in Bäche Durchzogen wird die Fast alle in den Großen Fluss Eiren Münden. Das Fruchtbare Tiefland ist Gezeichnet von Hügel und Tälern. 

### Subregionen
#### Flodfjell
Flodfjell
„Flussberge“, ein Name, der sowohl die Flüsse als auch die Berge hervorhebt.
Die Felsige Küsten Region mit 

#### Erenvaldr
Erenvaldr - das Tiefland, das Fruchtbarste gebiet in Ulvarngard wo die meisten Ulfen leben hier findet sich
Hier leben die Meisten Ulfen der Region. Weiter Wiesen und Hügel Zeichenen das land aus die durch eine flüssen durchschnitten ist. die meinsten flüssen haben ihren ursprung in den Berg die Ernvaldr begrenzen und die meinsten flüsse Fließen früher oder später in den Mächstige und wichtigsten fluss der region Der Eiren.
Unzählichen siedlungen befinden sich im diesem Tal und hier befindet sich auch der Haupt sitzt der <Platzhalten>

#### Vetrarskogen
Vetrarskogen – „Herrschaftswald“ oder „Herrschafts des Waldes, symbolisch für Macht und Erhabenheit.

#### Skarnheim
Skarnheim - "Die Nordlichts Region" ist Gezeichnet von Kälte Bergen und Viele Magischen Bestien die hier ihre Heimat haben

#### Tjarnfjell
Tjarnfjell – „Berg der Teiche“, ein poetischer Name, der die wasserreichen Ebenen und Berge kombiniert.

#### Vintermark
Es heißt Hinter Skarnheim liegt die Region die man Vintermark nennt. die ist Sagen umwoben obwohl es eigne Ulfen gab die behauptet habe Vintermark Bereist zu haben ist es zweifelhaft ob die Region existiert oder ob diese Ulfen nur die nördlichste teile Skarnheim verwechseln.
Es heißt das in Vintermark leben troz der Unwirklichen Klima bedingungen immer noch Ulfen oder Nahe verwandte der Ulfen

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


## 📭 Erwähnungen 
```dataview
TABLE WITHOUT ID link(file.name) as "Erwähnt in", NoteIcon as "Notiz typ"
where contains(file.outlinks, this.file.link)
sort file.name
```