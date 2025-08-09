---
aliases: 
autor:
typ:
status:
Sitzungsbezug:
Ortbezug:
Encounterbezug:
NoteIcon: Ballade
tags:
  - "#Sarenraes_Fehler/Objekt/Ballade"
---
> [!infobox|no-t right]
> #  🎶 `=this.file.name`
> |    |    |
> |--- |  --- |
> | autor| `INPUT[suggester(optionQuery(#Sarenraes_Fehler/Personen)):autor]`|
> | Typ| `INPUT[inlineSelect(option(Historisch), option(Fiktiv), option(Abenteuer)):typ]`|
> | status| `INPUT[inlineSelect(option(vollständig), option(unvollständig)):status]` |
> #### Bezug
> |    |    |
> |--- |  --- |
> | Sitzung| `INPUT[suggester(optionQuery(#Sarenraes_Fehler/Session_Journal)):Sitzungsbezug]`|
> | Ort| `INPUT[suggester(optionQuery(#Sarenraes_Fehler/Ort)):Ortbezug]`|
> | Encounter| `INPUT[suggester(optionQuery(#Sarenraes_Fehler/Encounter)):Encounterbezug]`|


## 📝 Inhalt & Thema
> [!info|no-t]
> Worum geht es? Heldentaten, Tragödie, Mythos, Warnung?

## 🗣️ Verse
> *„Sarenrae weinte blut'gen Glanz,  
> als ihre Gläub'gen brachen den Tanz …“*


## 🎓 Bezug/Bedeutung 
> [!abstract|no-t]
> Bezug/Bedeutung der Ballade im Kontext
>- Sitzung: `=this.Sitzungsbezug`
>- Ort: `=this.Ortbezug`
>- Encounter: `=this.Encounterbezug`

## 📌 Anmerkungen
> [!anmerkung|no-t]
> Zusätzliche Hinweise, oder Kommentare zur Ballade
> ... .

## 📭 Erwähnungen 
> [!attention|no-t]
> ```dataview
TABLE WITHOUT ID link(file.name) as "Erwähnt in", NoteIcon as "Notiz typ"
where contains(file.outlinks, this.file.link)
sort file.name
