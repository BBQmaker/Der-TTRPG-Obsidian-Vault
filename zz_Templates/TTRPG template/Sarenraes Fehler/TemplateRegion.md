---
aliases: 
Ebene: 
InitialeentdeckunginSitzung: 
tags:
  - Sarenraes_Fehler/Region/Über
---

> [!infobox|no-t]
> # 🗺️ `=this.file.name`
> | |   |
> |---|---|
> |aliases | `INPUT[inlineList:aliases]` |
> |Ebene | `INPUT[text:Ebene]` |
> |Initiale entdeckung| `INPUT[suggester(optionQuery(#Sarenraes_Fehler/Session_Journal)):InitialeentdeckunginSitzung]` |

## 🌄 Beschreibung
> [!info|no-t]
> Hier Beschreibung

## 📌 Anmerkungen
> [!anmerkung|no-t]
> Historische Hintergründe, Plot-Hooks, Metainfos für den SL.

## 📭 Erwähnungen 
> [!attention|no-t]
> ```dataview
TABLE WITHOUT ID link(file.name) as "Erwähnt in", NoteIcon as "Notiz Typ"
where contains(file.outlinks, this.file.link)
sort file.name
