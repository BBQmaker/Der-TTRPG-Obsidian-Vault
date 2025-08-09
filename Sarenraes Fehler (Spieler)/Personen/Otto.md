---
aliases:
  - Otto "der Großherzige"
Status: Verstorben
Spezies: Mensch
Alter: Erwachsener
Disposition: Alliiert
AssoziierteGruppe: "[[Sarenraes Fehler (Spieler)/Fraktionen & Institutionen/Bachbuben.md|Bachbuben]]"
OrtderErstenBegegnung: "[[Sarenraes Fehler (Spieler)/Orte/Naturstätte/Unterirdische Labor Ruine.md|Unterirdische Labor Ruine]]"
SitzungderErstenBegegnung: "[[Sarenraes Fehler (Spieler)/Sitzungs Journals/001 -Operation Otto- Journal.md|001 -Operation Otto- Journal]]"
tags:
  - Sarenraes_Fehler/Personen/NPC
---
> [!infobox|no-t]
> # 🧑‍🤝‍🧑`=this.file.name`
> | |   |
> |---|---|
> |aliases | `INPUT[inlineList:aliases]` |
> |Status | `INPUT[inlineSelect(option(Lebendig), option(Verstorben), option(Verschollen)):Status]`|
> |Spezies | `INPUT[text:Spezies]` |
> |Alter | `INPUT[inlineSelect(option(Kind), option(Junger Erwachsener), option(Erwachsener), option(fortgeschr. Alter), option(Greis), option(Alterslos)):Alter]` |
> |Disposition | `INPUT[inlineSelect(option(Alliiert), option(Freundlich), option(Neutral),option(Angespannt), option(Feindlich)):Disposition]` |
> |Assoziierte Gruppe | `INPUT[suggester(optionQuery(#Sarenraes_Fehler/Lore/Fraktionen_Institutionen)):AssoziierteGruppe]`| 
> |Ort der Ersten Begegnung | `INPUT[suggester(optionQuery(#Sarenraes_Fehler/Ort)):OrtderErstenBegegnung]` |
> |Sitzung der Ersten Begegnung | `INPUT[suggester(optionQuery(#Sarenraes_Fehler/Session_Journal)):SitzungderErstenBegegnung]` |

## Beschreibung
> [!info|no-t]
> Otto "der Großherzige", ist ein geschätzter Freund und Bekannter von [[Rucielo Gam]]. Allseits beliebt und stets mit einem Lächeln auf den Lippen ist Otto ein gern gesehener Gast des [[Der Fließende Bach]].  
>Als ein entschlossener [[Rucielo Gam]] die kompetentesten und beeindruckendsten Personen, die er kannte, zusammenrief und ihnen mitteilte, dass dieses strahlende Licht der Nachbarschaft entführt worden sei, war die Entscheidung schnell gefällt, alles daranzusetzen, ihn zu retten.

## 👁️‍🗨️ Äußerliche Merkmale
> [!info|no-t]
>  z.b Größe & Statur, Kleidung & AusrüstungSonstige Merkmale #Sarenraes_Fehler/To_Do 

## 🎭 Soziale Merkmale
> [!info|no-t]
> z.b Erster Eindruck, Rolle/Beruf, Generelles Verhalten #Sarenraes_Fehler/To_Do 

## 🔗Allianzen & Zugehörigkeiten
> [!info|no-t]
> Otto "der Großherzige", ist ein geschätzter Freund und Bekannter von [[Rucielo Gam]]. Er ist auch einer der wichtigsten Mitglieder der [[Bachbuben]]
> Außerdem ist ein guter Bekannter von der [[Die Furiosen Vier|Furiosen Vier]] und alle dessen mitglieder [[Arne Therod Torvaldson]], [[Selena Vynstein]], [[Urima Radiomus]] und der bereits genannte [[Rucielo Gam]].

## 📌 Anmerkungen
> [!anmerkung|no-t]
> Jetzt ist er tot. wir haben versagt ihn zu Retten 

## 🌄 Bekannte Aufenthalts Orte
> [!info|no-t]
> ```dataview
TABLE WITHOUT ID link(file.name) as "Bekannte Aufenthalts Orte", OrtTyp as "Ort Typ", Region
from #Sarenraes_Fehler/Ort 
where contains(file.outlinks, this.file.link)
sort file.name

## 📭 Erwähnungen 
> [!attention|no-t]
>```dataview
TABLE WITHOUT ID link(file.name) as "Erwähnt in", NoteIcon as "Notiz typ"
where contains(file.outlinks, this.file.link)
sort file.name