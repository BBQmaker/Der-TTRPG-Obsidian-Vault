---
aliases: 
Spieler:
  - Marvin
  - Paul
  - Richard
  - Lasse
Klasse: 
Spezies: 
level: 5
Status:
  - Active
PCKnownLanguages:
  - Common
NoteIcon: Spieler
tags:
  - Sarenraes_Fehler/Personen/Spielercharakter
---
# `=this.file.name`

## 🎭 Allgemeine Informationen 
- **Spieler**: `=this.Spieler`
- **Spezies**: `=this.Spezies`
- **Klasse**: `=this.Klasse`
- **Stufe**: `=this.Level`
- **Status**: `=this.Status`

### 💎Charakter Vorstellung


### 👥 Äußerlichkeiten



## 📖 Hintergrundgeschichte 
> Schreibe hier die Hintergrundgeschichte des Charakters. Wie ist der Charakter aufgewachsen? Was motiviert ihn? Gibt es besondere Ereignisse, die ihn geprägt haben?

## 🗒️ Notizen 
> Platz für Spielnotizen, Plot-Hooks oder spezifische Details, die im Spiel wichtig werden könnten.


## 📭 Erwähnungen 
```dataview
TABLE WITHOUT ID link(file.name) as "Erwähnt in", NoteIcon as "Notiz typ"
where contains(file.outlinks, this.file.link)
sort file.name
```