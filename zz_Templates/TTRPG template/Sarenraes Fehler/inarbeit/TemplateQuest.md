---
QuestObtained: 
QuestStatus: Not Started
Questgeber: 
QuestOrtErhalten: 
QuestSessionObtained: 
Questbelohnung: 
NoteIcon: quest
tags:
  - Sarenraes_Fehler/Quest
---
> [!infobox]+
> # `=this.file.name`
> ## Quest Details
> Type |  Stat |
> ---|---|
> Erhalten am | `INPUT[datePicker:QuestObtained]` |
> Status | `INPUT[inlineSelect(option(Not Started), option(In Progress), option(Complete)):QuestStatus]` |
> Quest Geber | `INPUT[suggester(optionQuery(#Sarenraes_Fehler/npc)):Questgeber]` |
> Quest Erhalten in | `INPUT[suggester(optionQuery(#Sarenraes_Fehler/Ort)):QuestOrtErhalten]` |
> In Session Erhalten | `INPUT[suggester(optionQuery(#Sarenraes_Fehler/Session_Journal)):QuestSessionObtained]` |
> Belohnung | `INPUT[suggester():Questbelohnung]` |
# `=this.file.name`
Beschreiben Sie hier die quest.

## Ziel der Quest
Führen Sie hier die Ziele auf.

## Belohnungen
Führen Sie die Belohnungen hier auf.

## Anmerkungen
Hier Anmerkungen.

