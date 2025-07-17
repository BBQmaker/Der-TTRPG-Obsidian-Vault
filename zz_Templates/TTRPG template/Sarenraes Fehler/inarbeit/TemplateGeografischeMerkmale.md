---
aliases: 
Typ:
  - Anderes
  - Berg
  - Fluss
  - Wald
  - Sumpf
  - Wüste
  - See
  - Insel
  - Höhle
  - Tal
  - Gebirge
  - Magischer Ort
Region: 
Subregion:
---
# `=this.file.name`

### 🗺️ Allgemeine Informationen
- **Typ**: 
- **Region**: 
- **Koordinaten / Lage**: 
- **Größe / Ausdehnung**: 

### 📖 Beschreibung
Kurze, atmosphärische Beschreibung des Ortes. Was sieht, hört, riecht man dort? Gibt es besondere Merkmale?





## 📭 Erwähnungen 
```dataview
TABLE WITHOUT ID link(file.name) as "Erwähnt in", NoteIcon as "Notiz typ"
where contains(file.outlinks, this.file.link)
sort file.name
```