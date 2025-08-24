---
QuestStatus: Nicht begonnen
QuestInSitzungErhalten: 
Questgeber: 
QuestanOrtErhalten: 
Questbelohnung: 
QuestInSitzungAbgeschlossen: 
NoteIcon: quest
tags:
  - Sarenraes_Fehler/Quest
---
> [!infobox|no-t right]
> ## `=this.file.name`
> # Details
> Type |  Daten |
>  --- | --- |
> Status | `INPUT[inlineSelect(option(Nicht begonnen), option(Begonnen), option(Erfolgreich abg.), option(Fehlgeschlagen)):QuestStatus]` |
> Questgeber  | `INPUT[suggester(optionQuery(#Sarenraes_Fehler/Personen/NPC)):Questgeber]` |
> Quest Erhalten in | `INPUT[suggester(optionQuery(#Sarenraes_Fehler/Ort)):QuestanOrtErhalten]` |
> In Session Erhalten | `INPUT[suggester(optionQuery(#Sarenraes_Fehler/Session_Journal)):QuestInSitzungErhalten]` |
> In Session Abgeschlossen | `INPUT[suggester(optionQuery(#Sarenraes_Fehler/Session_Journal)):QuestInSitzungAbgeschlossen]` |
## 📝 Beschreibung
> [!summary|no-t]
> Beschreibe hier die Quest. Wer hat sie gegeben, worum geht es, und warum ist sie wichtig?

## 🎯 Ziel der Quest
> [!check|no-t]
> - Ziel 1
> - Ziel 2
> - Optional: Bonusziel

## 🧭 Verlauf
> [!summary|no-t]
>- ✅ Etwas erledigt
>- ☐ Noch offen
>- ☐ Kritische Entscheidung steht bevor

## 🎁 Belohnungen
> [!schatz|no-t]
> Führen Sie die Belohnungen hier auf.

## 🔍 Hinweise & Anmerkungen
> [!anmerkung|no-t]
>- Informationen, offene Fragen, besondere Regeln oder Hinweise zur Durchführung.
>- Z. B. „Kann nur bei Nacht abgeschlossen werden“, „Erfordert Dolmetscher“, etc.


## 📭 Erwähnungen 
> [!attention|no-t]
>```dataview
TABLE WITHOUT ID link(file.name) as "Erwähnt in", NoteIcon as "Notiz typ"
where contains(file.outlinks, this.file.link)
sort file.name