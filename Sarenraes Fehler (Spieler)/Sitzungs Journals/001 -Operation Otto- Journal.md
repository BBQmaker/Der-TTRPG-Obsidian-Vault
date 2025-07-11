---
Sitzungsdatum: 2024-11-02
sessionstatus:
  - geschehen
Sitzungsnummer: "001"
NoteIcon: journal
tags:
  - Sarenraes_Fehler/Session_Journal
vollständig: ja
---
# `=this.file.name`
## 📜Kurzzusammenfassung
Rucielo Gams Freund Otto ist verschwunden! Gemeinsam mit drei Freunden wagt er sich in die Höhlen außerhalb der Stadt, um ihn zu retten.

## ## 🎭 Charakterliste 
[[Die Furiosen Vier]] -->([[Arne Therod Torvaldson]] [[Rucielo Gam]] [[Selena Vynstein]] [[Urima Radiomus]])
[[Otto]]

## 🗺️ Orte besucht
[[Vermis]]

Initiale Entdeckung von Orten
```dataview
TABLE WITHOUT ID link(file.name) as "Orte", Region as "Region", OrtTyp as "Ort Typ", OrtStatus as "Ort Status" 
from #Sarenraes_Fehler/Ort  
WHERE ErstentdeckunginSitzung = link(this.file.name)
SORT Sitzungsnummer ASC
```

## ⚔️ Kämpfe & Herausforderungen
```dataview
TABLE WITHOUT ID link(file.name) as "Encounter", EncounterTyp as "Encounter Typ", OrtdesEncounters as "Ort des Encounters"
from #Sarenraes_Fehler/Encounter   
WHERE EncounteredInSession = link(this.file.name)
SORT Sitzungsnummer ASC
```

## 📚 Sitzungsübersicht
Wir haben Otto gesucht der Freund von Richards Charakter er wurde verschleppt von unbekannten Kreaturen wir habe spuren durch eine Stinkige höhle. wir haben gegen Ratten gekämpft dann gegen einen Großen Vielfraß und schließlich gegen Oozes

## 🎲 Meta-Kommentare
Erste Session Woop Woop!