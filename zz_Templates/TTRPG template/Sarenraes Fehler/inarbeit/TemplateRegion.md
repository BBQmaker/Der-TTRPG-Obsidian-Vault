---
aliases: 
Regionstyp: 
DominanteEigenschaften: 
Bewohner: 
Gefahren: 
AssoziierteFraktionen: 
Ebene: 
ErsteErwähnunginSession: 
tags:
  - Sarenraes_Fehler/Region
---

> [!infobox|no-t]
> # 🗺️ `=this.file.name`
> | |   |
> |---|---|
> |aliases | `INPUT[inlineList:aliases]` |
> |Ebene | `INPUT[suggester(optionQuery(#Sarenraes_Fehler/Orte/Planar)):Ebene]` |
> |Regionstyp | `INPUT[inlineSelect(option(Wildnis), option(Stadt/Ansiedlung), option(Festung), option(Heiligtum), option(Ruinen), option(Gebirge/Schlucht), option(Gewässer/Ozean), option(Besonderes)):Regionstyp]` |
> |Dominante Eigenschaften | `INPUT[inlineList:DominanteEigenschaften]` |
> |Bewohner | `INPUT[inlineList:Bewohner]` |
> |Gefahren | `INPUT[inlineList:Gefahren]` |
> |Assoziierte Fraktionen | `INPUT[suggester(optionQuery(#Sarenraes_Fehler/Fraktionen_Institutionen)):AssoziierteFraktionen]` |
> |Erste Erwähnung | `INPUT[suggester(optionQuery(#Sarenraes_Fehler/Session_Journal)):ErsteErwähnung]` |

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
