---
aliases:
  - Akademie von Vrin
Region: "[[Sarenraes Fehler (Spieler)/Orte/Region/Die Oberfläche.md|Die Oberfläche]]"
Ortstatus:
  - Verlassen
InitialeentdeckunginSitzung: "[[Sarenraes Fehler (Spieler)/Sitzungs Journals/014 -Die Akademie- Journal.md|014 -Die Akademie- Journal]]"
tags:
  - Sarenraes_Fehler/Ort/Ruine
---
> [!infobox|no-t]
> # ⚒️ `=this.file.name`
> | |   |
> |---|---|
> |aliases | `INPUT[inlineList:aliases]` |
> |Region | `INPUT[suggester(optionQuery(#Sarenraes_Fehler/Ort/Region)):Region]` |
> | Ortstatus |`INPUT[inlineListSuggester(option(Verlassen), option(Infiziert), option(Bewohnt)):Ortstatus]` | 
> |Initiale entdeckung | `INPUT[suggester(optionQuery(#Sarenraes_Fehler/Abenteuer/Session_Journal)):InitialeentdeckunginSitzung]` |

## 🌄 Beschreibung
> [!info|no-t]
> Hier Beschreibung #Sarenraes_Fehler/To_Do 

## 📅 Geschehnisse
>
>Hier Ablauf, Funde, Encounter verlinken und besondere Ereignisse oder Veränderungen dokumentieren.


## 🐓Encounter
> [!danger|no-t]
> ```dataview
TABLE WITHOUT ID 
link(file.name) as "Encounter", OrtdesEncounters as "Ort", EncounteredInSession.Sitzungsnummer as "Sitzungsnummer"
from #Sarenraes_Fehler/Encounter  
WHERE OrtdesEncounters = link(this.file.name) AND file.name != "TemplateOrt"
SORT Sitzungsnummer ASC

## 🗺️ Benachbarte Orte
>
> Benachbarte Orte hier.

## 📌 Anmerkungen
> [!anmerkung|no-t]
> Anmerkungen

## 📭 Erwähnungen 
> [!attention|no-t]
> ```dataview
TABLE WITHOUT ID link(file.name) as "Erwähnt in", NoteIcon as "Notiz Typ"
where contains(file.outlinks, this.file.link)
sort file.name

