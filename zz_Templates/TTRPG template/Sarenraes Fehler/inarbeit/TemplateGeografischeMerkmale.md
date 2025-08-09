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
# 🌍 `=this.file.name`

## 🗺️ Allgemeine Informationen
- **Typ**: `=this.Typ`
- **Region**: `=this.Region`
- **Subregion**: `=this.Subregion`
- **Koordinaten / Lage**: z.B. nordwestlich von X
- **Größe / Ausdehnung**: z.B. 30 km lang, 10 km breit

## 📖 Beschreibung
> Kurze, atmosphärische Beschreibung des Ortes. Was sieht, hört, riecht man dort? Gibt es besondere Merkmale?

## 🧭 Bedeutung für die Welt

## 📭 Erwähnungen 
```dataview
TABLE WITHOUT ID link(file.name) as "Erwähnt in", NoteIcon as "Notiz typ"
where contains(file.outlinks, this.file.link)
sort file.name
```