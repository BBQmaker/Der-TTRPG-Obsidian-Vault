---
aliases: 
Pantheon: Core Deities
Typ: 
Areas_of_Concern: 
Alignment: 
Domains: 
Realm: 
Symbol: 
Sacred_Animal: 
Sacred_Colors: 
NoteIcon: Gottheit
tags:
  - "#Sarenraes_Fehler/Lore/Gottheit"
---
> [!infobox|no-t right]
> # 🕊️`=this.file.name`
><img src="image">
>
> |    |    |
> |--- |  --- |
> | Titel & Aliases|`INPUT[inlineList:aliases]` |
> | Typ|`INPUT[inlineSelect(option(Covenant), option(Deity)):Typ]` |
> | Pantheon|`INPUT[inlineList:Pantheon]` |
> | Realm|`INPUT[inlineList:Realm]` |
> | Alignment|`INPUT[inlineList:Alignment]` |
> | Areas of Concern|`INPUT[inlineList:Areas_of_Concern]`|
> | Domains|`INPUT[inlineList:Domains]`|
> | Symbol|`INPUT[inlineList:Symbol]`|
> | Sacred Animal|`INPUT[inlineList:Sacred_Animal]`|
> | Sacred Colors|`INPUT[inlineList:Sacred_Colors]`

## 📒 Beschreibung
> [!info|no-t]
>Generelle Beschreiung der Gottheit

## ✨ Dogma
> [!info|no-t]
>Generelle Beschreiung der des Dogma der Gottheit

- ### ✅ Edicts
> [!success|no-t]
> Edicts der Gottheit

- ### ❌ Anathema
> [!failure|no-t]
> Anathema der Gottheit

## 🧎 Erscheinung
> [!info|no-t]
> Das Aussehen oder die Erscheinung der Gottheit

## ⚖️ Beziehungen
> [!info|no-t]
> Beziehungen der Gottheit. Feinde, Verbündete, etc.

## 📰Geschichte
> [!info|no-t]
> Geschichte der Gottheit etc.

## 🔮 Göttliche Vorsehung
> [!divine|no-t]
> Göttliche Belohnungen, Gaben oder Geschenke

## 🧙 Diener:innen
> [!person|no-t]
> Diener:innen der Gottheit

## 📝 Anmerkungen
> [!anmerkung|no-t]
> Anmerkungen, Notizen oder Sonstiges


## 📭 Erwähnungen 
> [!attention|no-t]
> ```dataview
TABLE WITHOUT ID link(file.name) as "Erwähnt in", NoteIcon as "Notiz typ"
where contains(file.outlinks, this.file.link)
sort file.name
