---
aliases: 
LiteraturTyp:
  - Sachbuch
  - Roman
  - Tagebuch
  - Notiz
  - Aufzeichnung
autor: 
ErhaltenamOrt: 
sprache:
  - Gemeinsprache
  - Zwergisch
  - Elfisch
  - Gnomisch
status:
  - vollständig
  - fragment
  - übersetzung
  - zensiert
NoteIcon: Literatur
tags:
  - "#Sarenraes_Fehler/Objekt/Literatur"
---
# 📖 `=this.file.name`
## 📧Kurzbeschreibung
Kurz beschreibung über den Inhalt und über den zustand sowie den Autor

## ✍️ Autor & Hintergrund
- **Autor**: `=this.autor`
- **Über den Autor**: `z. B. Priester der Sarenrae, Historiker, Ketzer`
- **Motivation oder Zielsetzung**: `z. B. Aufklärung, Propaganda, Reue, Satire`

## 🖋️ Inhalt
Beschreibe hier , worum es in dem Werk geht. Handelt es sich um eine religiöse Polemik, eine historische Aufzeichnung, ein Heldenepos, eine verbotene Anleitung?

## 📚 Sonstige Attribute
- **Verbreitung**: lokal / regional / überregional / einzigartig
- **Zustand**: gut erhalten / beschädigt / fragmentarisch
- **Fundort** : `=this.ErhaltenamOrt`



## 📭 Erwähnungen 
```dataview
TABLE WITHOUT ID link(file.name) as "Erwähnt in", NoteIcon as "Notiz typ"
where contains(file.outlinks, this.file.link)
sort file.name
```
