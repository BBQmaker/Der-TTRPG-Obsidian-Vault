---
aliases: 
Typ:
  - Humanoid
  - Aberration
  - Fey
  - "Magical Beast\r"
  - "Monstrous Humanoid\r"
  - Outsider
  - Plant
  - Undead
NoteIcon: Volk
tags:
  - Sarenraes_Fehler/Lore/Volk
---
# 🧬 `=this.file.name`

## 🌍 Herkunft & Siedlungsgebiete
Wo stammt dieses Volk ursprünglich her, und wo lebt es heute?  
Z. B. „Stammt aus den Eiswüsten im Norden, heute verstreut über mehrere Regionen.“

## 📖 Geschichte & Mythos
Wie sieht die Ursprungserzählung oder historische Entwicklung aus?  
Gibt es legendäre Ahnen, Katastrophen, Völkerwanderungen?

## 🗣️ Sprache & Namenskonventionen
- Hauptsprache(n): `...`
- Schriften oder Runensysteme: `...`
- Namensmuster: `z. B. alle Namen enden auf -or bei Männern`

## 🙏 Religion & Weltbild
- Hauptglaube: `[[Gottheit oder System]]`
- Kosmologie, Rituale, Tabus
- Verhältnis zu Magie oder Geistern

## 🧑‍🤝‍🧑 Gesellschaft & Kultur
- Familienstruktur, Rollenbilder
- Traditionen & Feste
- Kleidung, Kunst, Musik, Handwerk
- Umgang mit anderen Völkern

## 🧱  Siedlungen
Wie bauen sie? Wo leben sie? Was zeichnet ihre Städte, Dörfer oder Lager aus?

## 📚 Bekannte Persönlichkeiten
- `[[Anführer/in]]`
- `[[Held/in der Vergangenheit]]`
- `[[Berühmter Magier]]`

## 🗺️ Wichtige Orte
- `[[Hauptstadt oder Zentrum]]`
- `[[Heiliger Ort]]`
- `[[Verlassene Heimatregion]]`

## 📝 Anmerkungen
Zusätzliche Beobachtungen, z. B. für SL-Hinweise oder regionale Abweichungen.


## 📭 Erwähnungen 
```dataview
TABLE WITHOUT ID link(file.name) as "Erwähnt in", NoteIcon as "Notiz typ"
where contains(file.outlinks, this.file.link)
sort file.name
```