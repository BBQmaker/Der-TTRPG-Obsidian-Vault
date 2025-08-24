---
aliases:
Region: "[[Sarenraes Fehler (Spieler)/Orte/Region/Die Oberfläche.md|Die Oberfläche]]"
Ortstatus:
  - Verlassen
InitialeentdeckunginSitzung:
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
> 
>[[Skelett Encounter]]
>
>Zweiter Stock:
>Ein wenig Größer als die Wendel Treppe
>4 Türen
>Die Vermoderte Tür
>
>Laboratorium wo An Leichen herum experimentiert wurden
>
>Mehre Käfige im Raum 1,60 hoch und 1M lang und breit
>
>Die Reste von eine Art Schlafzimmer 
>ein Seltsames Loch in der Decke
>Ein Skelett inklusive Rüstung liegt in der Mitte des Raumes
>
>Wir sehe Düstere Stelle im Wald
>
>Leiche von [[Oskar]]
>Stab
>Fullplate Rüstung Masterwerk ist auch Magisch
>	-Unbekannt Faint
>	-Unbekannt moderate
>	-Railing    Faint 
>Langschwert Meisterwerk Dies ist Magisch
>	- Encantment Faint
>	- Evokation Moderat
>	-
>Haufen Bücher 
>Finden -> [[Tagebuch von Unbekannt]]

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

