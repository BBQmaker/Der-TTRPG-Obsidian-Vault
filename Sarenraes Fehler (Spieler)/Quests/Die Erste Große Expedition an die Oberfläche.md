---
QuestStatus: Erfolgreich abgeschlossen
QuestInSitzungErhalten: "[[003 -Der erste Atemzug- Journal]]"
Questgeber: "[[Der Hohe Rat von Vermis]]"
QuestanOrtErhalten: "[[Ratsgebäude]]"
Questbelohnung: Ruhm und Ehre
QuestInSitzungAbgeschlossen: "[[006 -Die Stahlzunge- Journal]]"
NoteIcon: quest
tags:
  - Sarenraes_Fehler/Quest
---
> [!infobox]+
> ## Quest Details
> Type |  Daten |
>  --- | --- |
> Status | `INPUT[inlineSelect(option(Nicht begonnen), option(Begonnen), option(Erfolgreich abgeschlossen), option(Fehlgeschlagen)):QuestStatus]` |
> Quest Geber | `INPUT[suggester(optionQuery(#Sarenraes_Fehler/Personen/NPC)):Questgeber]` |
> Quest Erhalten in | `INPUT[suggester(optionQuery(#Sarenraes_Fehler/Ort)):QuestanOrtErhalten]` |
> In Session Erhalten | `INPUT[suggester(optionQuery(#Sarenraes_Fehler/Session_Journal)):QuestInSitzungErhalten]` |
> Belohnung | `INPUT[inlineSelect(option(Geld), option(Ruhm und Ehre), option(Luft und Liebe), option(Magische Gestände)):Questbelohnung]` |
> In Session Abgeschlossen | `INPUT[suggester(optionQuery(#Sarenraes_Fehler/Session_Journal)):QuestInSitzungAbgeschlossen]` |
# `=this.file.name`
## 📝 Beschreibung
Beschreibe hier die Quest. Wer hat sie gegeben, worum geht es, und warum ist sie wichtig? #Sarenraes_Fehler/To_Do

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