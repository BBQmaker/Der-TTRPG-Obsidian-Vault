---
QuestStatus:
  - Nicht begonnen
  - Erfolgreich abgeschlossen
  - Fehlgeschlagen
  - Begonnen
QuestInSitzungErhalten: 
Questgeber: 
QuestanOrtErhalten: 
Questbelohnung: 
QuestInSitzungAbgeschlossen: 
NoteIcon: quest
tags:
  - Sarenraes_Fehler/Quest
---
> [!infobox]+
> # `=this.file.name`
> ## Quest Details
> Type |  daten |
>  --- | --- |
> Status | `INPUT[inlineSelect(option(Nicht begonnen), option(Begonnen), option(Erfolgreich abgeschlossen), option(Fehlgeschlagen)):QuestStatus]` |
> Quest Geber | `INPUT[suggester(optionQuery(#Sarenraes_Fehler/Personen/NPC)):Questgeber]` |
> Quest Erhalten in | `INPUT[suggester(optionQuery(#Sarenraes_Fehler/Ort)):QuestOrtErhalten]` |
> In Session Erhalten | `INPUT[suggester(optionQuery(#Sarenraes_Fehler/Session_Journal)):QuestSessionObtained]` |
> Belohnung | `INPUT[suggester():Questbelohnung]` |
# `=this.file.name`
## 📝 Beschreibung
Beschreibe hier die Quest. Wer hat sie gegeben, worum geht es, und warum ist sie wichtig?

## 🎯 Ziel der Quest
- Ziel 1
- Ziel 2
- Optional: Bonusziel

## 🧭 Verlauf
- ✅ Etwas erledigt
- ☐ Noch offen
- ☐ Kritische Entscheidung steht bevor

## 🎁 Belohnungen
Führen Sie die Belohnungen hier auf.

## 🔍 Hinweise & Anmerkungen
- Informationen, offene Fragen, besondere Regeln oder Hinweise zur Durchführung.
- Z. B. „Kann nur bei Nacht abgeschlossen werden“, „Erfordert Dolmetscher“, etc.


## 📭 Erwähnungen 
```dataview
TABLE WITHOUT ID link(file.name) as "Erwähnt in", NoteIcon as "Notiz typ"
where contains(file.outlinks, this.file.link)
sort file.name
```