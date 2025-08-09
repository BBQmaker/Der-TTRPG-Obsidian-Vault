---
aliases:
  - Frostfall
autor: "[[Sarenraes Fehler (Spieler)/Personen/PCs/Arne Therod Torvaldson.md|Arne Therod Torvaldson]]"
typ:
  - Abenteuer
status:
  - vollständig
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
> Ein Typisches Marsch lied der Ulfen. Eins von viele aber ein von den wenigen die Platzhalten überstanden haben

## 🗣️ Verse
> Frostfall
>_(Ulfen-Stabreim-Marsch)_
>
Frost fällt, Fels fliegt, Füße marschieren,  
Sturmstoß, Steinspalt, Stiere wir schreien.  
Heda, Helden! Hämmernd die Herzen,  
Waldwind weckt uns, weit hallt der Ruf.
>
Raben rufen, Riegel zerspringen,  
Blutbrand bricht in bittere Nacht.  
Heda, Helden! Hämmernd die Herzen,  
Schwertschlag, Schildklang, Schicksal erwacht.
> 
Hochhall’n Hörner, Hänge erzittern,  
Schneesturm schneidet, Scharen steh’n fest.  
Heda, Helden! Hämmernd die Herzen,  
Bergbrand brüllt uns, Bahn in den Krieg!
>
**Refrain (nach jeder Strophe, gerufen)**  
**Heda! Heda! Hoch die Schilde!**  
**Heda! Heda! Härte im Blut!**

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
