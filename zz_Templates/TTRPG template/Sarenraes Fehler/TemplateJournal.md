---
Sitzungsdatum: 2025-01-01
Sessionstatus: Nicht geschehen
Sitzungsnummer:
Spielercharaktere: []
GruppenLvL:
NoteIcon: journal
tags:
  - Sarenraes_Fehler/Abenteuer/Session_Journal
---
> [!infobox|no-t right]
> # 📖`=this.file.name`
> |    |    |
> |--- |  --- |
> | Sitzungsdat.|`INPUT[datePicker:Sitzungsdatum]` |
> | Status | `INPUT[inlineSelect(option(Nicht geschehen), option(Geschehen)):Sessionstatus]`|
> | Sitzungsnr.| `INPUT[number:Sitzungsnummer]` |
> | Spielerchar.| `INPUT[inlineListSuggester(optionQuery(#Sarenraes_Fehler/Personen/Spielercharakter)):Spielercharaktere]` |
> |GruppenLvL| `INPUT[number:GruppenLvL]` |

## 📜Kurzzusammenfassung
> [!summary|no-t]
> Hier Kurzzusammenfassung!

## 🗺️ Orte besucht
>Hier alle besuchte Ort auflisten.
>
>### 🗻 Initiale Entdeckung von Orten
>> [!hint|no-t]
>> ```dataview
TABLE WITHOUT ID link(file.name) as "Orte", Region as "Region", OrtTyp as "Ort Typ", OrtStatus as "Ort Status" 
from #Sarenraes_Fehler/Ort  
WHERE InitialeentdeckunginSitzung = link(this.file.name)
SORT Sitzungsnummer ASC

## ⚔️ Kämpfe & Herausforderungen
> [!danger|no-t]
> ```dataview
TABLE WITHOUT ID link(file.name) as "Encounter", EncounterTyp as "Encounter Typ", OrtdesEncounters as "Ort des Encounters"
from #Sarenraes_Fehler/Encounter   
WHERE EncounteredInSession = link(this.file.name)
SORT Sitzungsnummer ASC

## 📚 Sitzungsübersicht
> So ist es geschehen! im Großen Detail!

## 🎲 Meta-Kommentare
> [!faq|no-t]
>Encounter war mal wieder unbalanced! etc.

## 📭 Erwähnungen 
> [!attention|no-t]
> ```dataview
TABLE WITHOUT ID link(file.name) as "Erwähnt in", NoteIcon as "Notiz typ"
where contains(file.outlinks, this.file.link)
sort file.name