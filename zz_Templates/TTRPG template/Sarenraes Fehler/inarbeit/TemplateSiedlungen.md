---
aliases: 
OrtTyp:
  - Großstadt
  - Stadt
  - Kleinstadt
  - Dorf
  - Gehöft
  - Außenposten
  - Hof
Staatsform:
  - Monarchie
  - Republik
  - Oligarchie
  - Räterepublik
Anführer: 
Region: 
population: 0
Bevölkerung:
  - Menschen
  - Zwerge
  - Elfen
  - Tieflinge
  - Gnome
  - Half Elf
  - Half Orc
  - Halfling
  - Ratfolk
  - Catfolk
  - Grippli
  - Oread
  - Aasimar
  - Drow
NoteIcon: Siedlungen
tags:
  - "#Sarenraes_Fehler/Ort/Siedlung"
---
> [!infobox]
> # `=this.file.name`
> Type |  Stat |
> ---|---|
> Siedlungstyp | `=this.OrtTyp` |
> Staatsform | `=this.Staatsform` |
> Anführer | `=this.Anführer` |
> Region | `=this.Region` |
> Population | `=this.population` |
> Bevölkerung | `=this.Bevölkerung` |

## 🗺️ Beschreibung
{{Kurze Beschreibung des Ortes, Atmosphäre, Klima, Eindruck beim Ankommen}}

## 🧑‍🤝‍🧑 Wichtige Personen
- NSC 1 – {{z. B. Bürgermeisterin, wortkarg und streng}}
- NSC 2 – {{z. B. Wirt, redselig und neugierig}}
- NSC 3 – {{z. B. Wächterkommandant, misstrauisch}}

## 🏠 Wichtige Orte
- 🏨 **Gasthaus**: Name – {{z. B. "Zur rostigen Pfanne", berüchtigt für schlechtes Bier}}
- 🛒 **Marktplatz / Läden**: {{besondere Händler? Seltene Waren?}}
- ⛪ **Tempel / Heilige Orte**: {{welche Götter oder Rituale?}}
- 🏚️ **Besondere Gebäude**: {{z. B. altes Herrenhaus, geheime Höhle unter dem Brunnen}}

## ⚔️ Bedrohungen & Konflikte
- 👹 **Monster / Kreaturen**: {{was bedroht den Ort?}}
- 🕵️ **Intrigen / Machtspiele**: {{wer kämpft im Hintergrund um Einfluss?}}
- 🧨 **Offene Probleme**: {{z. B. Armut, Seuche, Spionage}}

## 📜 Geschichte & Legenden
{{Besondere Ereignisse, lokale Mythen, historische Persönlichkeiten}}

## 🧩 Notizen
- 🗒️ {{eigene Theorien, Kartenverweise, Gerüchte, Hinweise aus Spielsitzungen}}

## 📭 Erwähnungen 
```dataview
TABLE WITHOUT ID link(file.name) as "Erwähnt in", NoteIcon as "Notiz typ"
where contains(file.outlinks, this.file.link)
sort file.name
```