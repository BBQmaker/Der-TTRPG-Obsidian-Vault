---
aliases: 
Status: 
Spezies: 
Alter: 
Disposition: 
AssoziierteGruppe: 
OrtderErstenBegegnung: 
SitzungderErstenBegegnung: 
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
> hier Beschreibung

## 👁️‍🗨️ Äußerliche Merkmale
> [!info|no-t]
>  z.b Größe & Statur, Kleidung & AusrüstungSonstige Merkmale

## 🎭 Soziale Merkmale
> [!info|no-t]
> z.b Erster Eindruck, Rolle/Beruf, Generelles Verhalten

## 🔗Allianzen & Zugehörigkeiten
> [!info|no-t]
> Hier Allianzen & Zugehörigkeiten!

## 📌 Anmerkungen
> [!anmerkung|no-t]
> Eigene Theorien, Metainfos, Hinweise auf Täuschung etc.

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