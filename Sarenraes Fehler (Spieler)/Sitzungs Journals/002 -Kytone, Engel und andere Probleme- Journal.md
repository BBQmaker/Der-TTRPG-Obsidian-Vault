---
Sitzungsdatum: 2024-11-30
sessionstatus:
  - geschehen
Sitzungsnummer: "002"
NoteIcon: journal
tags:
  - Sarenraes_Fehler/Session_Journal
---
# `=this.file.name`
## 📜Kurzzusammenfassung
Hier Kurzzusammenfassung!

## ## 🎭 Charakterliste 
[[Die Furiosen Vier]] 
[[Allynna Ilivaris]]
[[Herulith]]

## 🗺️ Orte besucht
[[Stinkende Höhle]]
[[Unterirdische Labor Ruine]]

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
- Party noch immer in der Ruine
- Knacken im Ohr wie bei Druckausgleich
- Encounter mit einem kleinen Kyton, dieser wurde niedergestreckt
- Encounter mit einem großen Kyton nach Belauschung des Gesprächs mit seinem Herrn und Meister

## 🎲 Meta-Kommentare
Encounter war mal wieder unbalanced! etc.

