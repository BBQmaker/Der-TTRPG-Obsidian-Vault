---
questObtained: 2024-04-03
QuestStatus: In Bearbeitung
Questgeber: "[[Rucielo Gam]]"
QuestOrtErhalten: "[[Die Große Stadt]]"
questSessionObtained: "[[Session Journal 02.11.2024|02.11.2024]]"
Questbelohnung: unklar
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
> QuestOrtErhalten | `INPUT[suggester(optionQuery(#Category/Settlement)):QuestOrtErhalten]` |
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