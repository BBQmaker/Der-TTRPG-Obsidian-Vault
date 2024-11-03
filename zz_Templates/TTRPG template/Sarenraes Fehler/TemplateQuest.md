---
questObtained: 2024-04-03
QuestStatus: In Bearbeitung
Questgeber: 
questLocationObtained: 
questSessionObtained: 
Questbelohnung: 
tags:
  - Sarenraes_Fehler/Quest
---
> [!infobox]+
> # `=this.file.name`
> ###### Quest Details
> Type |  Stat |
> ---|---|
> Date Obtained | `INPUT[datePicker:questObtained]` |
> Status | `INPUT[inlineSelect(option(Not Started), option(In Progress), option(Complete)):questStatus]` |
> Quest Giver | `INPUT[suggester(optionQuery(#npc)):questGiver]` |
> Quest Location | `INPUT[suggester(optionQuery(#Category/Settlement)):questLocationObtained]` |
> Session Obtained | `INPUT[suggester(optionQuery(#journal)):questSessionObtained]` |
> Available Loot | `INPUT[suggester(optionQuery(#item)):questLootAvail]` |
> Acquired Loot | `INPUT[suggester(optionQuery(#item)):questLookEarned]` |

# `=this.file.name`
Beschreiben Sie hier die quest.

## Ziel der Quest
List the objectives here.

## Belohnungen
Führen Sie die Belohnungen hier auf


## Anmerkungen















.