---
OrtdesEncounters: 
EncounteredInSession: 
EncounterTyp:
  - Major
  - Minor
  - Boss
  - Sozial
AusgangdesEncounters:
  - TOD!
  - Schwere Verluste
  - Nahtoderfahrung
  - Sieg
  - Souveräner Sieg
EncounteraufLVL: 
NoteIcon: encounter
tags:
  - Sarenraes_Fehler/Encounter
---
# `=this.file.name`
## 📝 Kurzzusammenfassung
Kurzzusammenfassung hier! 

## 🐾 Kreaturen Daten
> *Liste hier die Kreaturen auf, die am Encounter beteiligt sind:* 
> - **Kreatur 1**: 🐺 Beschreibung oder Verlinkung zu Kreatur1 
> - **Kreatur 2**: 🐉 Beschreibung oder Verlinkung zu Kreatur2

## 🗺️ Ort
> Beschreibung des Orts, an dem der Encounter stattfindet.
> 

## 📖 Verlauf
> Erwähnenswerte Ereignisse während des Encounters
> Auslöser? ; Nahtoderlebnis? ; Tote?

## 📌 Anmerkungen
> Zusätzliche Hinweise, oder Kommentare zum Encounter
> ... .



## 📭 Erwähnungen 
```dataview
TABLE WITHOUT ID link(file.name) as "Erwähnt in", NoteIcon as "Notiz typ"
where contains(file.outlinks, this.file.link)
sort file.name
```