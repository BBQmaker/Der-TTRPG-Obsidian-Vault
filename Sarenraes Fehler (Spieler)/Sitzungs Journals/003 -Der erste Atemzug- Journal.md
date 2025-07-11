---
Sitzungsdatum: 2024-12-28
sessionstatus:
  - geschehen
Sitzungsnummer: "003"
NoteIcon: journal
tags:
  - Sarenraes_Fehler/Session_Journal
---
# `=this.file.name`
## 📜Kurzzusammenfassung
Hier Kurzzusammenfassung!

## ## 🎭 Charakterliste 
[[Die Furiosen Vier]] -->
([[Arne Therod Torvaldson]] [[Rucielo Gam]] [[Selena Vynstein]] [[Urima Radiomus]])

## 🗺️ Orte besucht

[[Die Oberfläche]]
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