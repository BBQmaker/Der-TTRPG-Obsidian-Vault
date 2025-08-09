---
EncounterTyp: Sozial
EncounterLVL: 5
AusgangdesEncounters: 
OrtdesEncounters: 
EncounteredInSession:
Ausgang:
NoteIcon: encounter
tags:
  - Sarenraes_Fehler/Encounter
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
> wie begegnen einem Aeon und erhalten  Visonen

## 🐾 Kreaturen Daten
> - 1 Aeone

## 🗺️ Ort
> Tief in der Wildnis auf einem Unbenannten weg
> 

## 📖 Verlauf
> wie begegnen einem Aeon 
> wir nähern uns ihm
> wir sehen eine zerstörte überwucherte stadt mit einem Monolithen
> wir sehen den Monolithen Zerbrechen vision endet hier
> Urima frag den Aeon nach details 
> details folgen #Sarenraes_Fehler/To_Do 

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