---
EncounterTyp: Major
EncounterLVL: 6
AusgangdesEncounters:
OrtdesEncounters:
EncounteredInSession:
Ausgang: unbestimmt
NoteIcon: encounter
tags:
  - Sarenraes_Fehler/Abenteuer/Encounter
---
> [!infobox|no-t right]
> #  🐉 `=this.file.name`
> |    |    |
> |--- |  --- |
> | Typ| `INPUT[inlineSelect(option(Major), option(Minor), option(Boss), option(Sozial)):EncounterTyp]`|
> | Sitzung| `INPUT[suggester(optionQuery(#Sarenraes_Fehler/Session_Journal)):Sitzungsbezug]`|
> | Ort| `INPUT[suggester(optionQuery(#Sarenraes_Fehler/Ort)):Ortbezug]`|
> | LVL| `INPUT[number:EncounterLVL]` |
> | Ausgang | `INPUT[inlineSelect(option(TOD!), option(Schwere Verluste), option(nahtoderfahrung ), option(Sieg), option(Souveräner Sieg), option(unbestimmt)):Ausgang]`|

## 📝 Kurzzusammenfassung
> [!summary|no-t]
> Kurzzusammenfassung hier! 

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
> [!anmerkung|no-t]
> Zusätzliche Hinweise, oder Kommentare zum Encounter
> ... .


## 📭 Erwähnungen 
> [!attention|no-t]
> ```dataview
TABLE WITHOUT ID link(file.name) as "Erwähnt in", NoteIcon as "Notiz typ"
where contains(file.outlinks, this.file.link)
sort file.name