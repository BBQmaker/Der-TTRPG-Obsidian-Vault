---
Sitzungsdatum: 2025-06-28
sessionstatus:
  - geschehen
Sitzungsnummer: "011"
NoteIcon: journal
tags:
  - Sarenraes_Fehler/Session_Journal
---
# `=this.file.name`
## 📜Kurzzusammenfassung


## ## 🎭 Charakterliste 
[[Die Furiosen Vier]] -->
([[Arne Therod Torvaldson]], [[Rucielo Gam]], [[Selena Vynstein]], [[Urima Radiomus]])

## 🗺️ Orte besucht
Hier alle besuchte Ort auflisten.

Initiale Entdeckung von Orten
```dataview
TABLE WITHOUT ID link(file.name) as "Orte", Region as "Region", OrtTyp as "Ort Typ", OrtStatus as "Ort Status" 
from #Sarenraes_Fehler/Ort  
WHERE ErstentdeckunginSitzung = link(this.file.name)
SORT Sitzungsnummer ASC
```

## ⚔️ Kämpfe & Herausforderungen
Hier alle Encounter Auflisten.

```dataview
TABLE WITHOUT ID link(file.name) as "Encounter", EncounterTyp as "Encounter Typ", OrtdesEncounters as "Ort des Encounters"
from #Sarenraes_Fehler/Encounter   
WHERE EncounteredInSession = link(this.file.name)
SORT Sitzungsnummer ASC
```

## 📚 Sitzungsübersicht
So ist es geschehen! im Großen Detail!

## 🎲 Meta-Kommentare
Encounter war mal wieder unbalanced! etc.