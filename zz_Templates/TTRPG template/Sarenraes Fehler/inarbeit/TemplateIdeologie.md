---
aliases: 
typ:
  - Philosophie
  - Religion
  - Kult
tags:
  - "#Sarenraes_Fehler/Lore/Ideologien"
---
# `=this.file.name`

## 📝 Grundprinzip
Kurze Zusammenfassung: Was glaubt oder vertritt diese Ideologie?

## 🗣️ Leitsätze oder Glaubenssätze
- „...“
- „...“

## 🧠 Beschreibung
Beschreibung!

## ⚖️ Einfluss & Konflikte
Wo ist sie verbreitet, und mit wem steht sie im Konflikt?

## 🔗 Verknüpfte Fraktionen & Personen
- Fraktion X
- Prophet Y

## 📭 Erwähnungen 
```dataview
TABLE WITHOUT ID link(file.name) as "Erwähnt in", NoteIcon as "Notiz typ"
where contains(file.outlinks, this.file.link)
sort file.name
```