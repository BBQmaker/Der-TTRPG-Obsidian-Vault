---
aliases: 
Spezies:
  - Mensch
  - Ratfolk
  - Ulfen
  - Slyp
  - Zwerg
  - Elf
  - Gnome
  - Half Elf
  - Half Orc
  - Halfling
OrtderErstenBegegnung: 
BekannteAufenthaltsOrte: 
InitialbegegnetinSession: 
AssoziierteGruppe: 
Alter:
  - Kind
  - Junger Erwachsener
  - Mittleres Alter
  - Fortgeschrittenes Alter
Geschlechtsidentität:
  - Weiblich
  - Männlich
  - nicht-binär
  - unbekannt
Disposition:
  - Alliiert
  - Freundlich
  - Neutral
  - Angespannt
  - Feindlich
Status:
  - Lebendig
  - Verstorben
  - Verschollen
tags:
  - Sarenraes_Fehler/Personen/NPC
---
> [!infobox]+
> # `=this.file.name`
> ## NPC Details
> Merkmale |  Daten |
> ---|---|
> Spezies | `=this.Spezies` |
> Alter | `=this.Alter` |
> Assoziierte Gruppe | `=this.AssoziierteGruppe` | 
> Spezies | `=this.Spezies` |
> Geschlechtsidentität | `=this.Geschlechtsidentität` |
> Status | `=this.Status`|
> Letzter Bekannter Aufenthalts Ort | `=this.Letzter_Bekannter_Aufenthalts_Ort` |

## 👁️‍🗨️ Aussehen
- 📏 **Größe & Statur**: {{groß/klein, kräftig/schlank etc.}}
- 👕 **Kleidung & Ausrüstung**: {{was trägt die Figur normalerweise}}
- 🧿 **Äußerliche Merkmale**: {{z.B. Narben, Tätowierungen, auffällige Kleidung}}

## 🎭 Soziale Merkmale
- 🎭 **Erster Eindruck**: {{Wie wirkte die Person beim ersten Treffen?}}
- 🛡️ **Rolle/Beruf**: {{Wache, Händler, Informant, Feind etc.}}
- 🧍 **Generelles Verhalten**: {{ruhig, aufbrausend, schüchtern, theatralisch etc.}}

## 🔗Allianzen & Zugehörigkeiten
- 🧬Familienbande
- 🏛️Mitgliedschaft in Fraktion/Institution
- 🤝Verbündet oder Freunde


## 🧩 Sonstiges / Notizen
- 🗒️ {{Eigene Theorien, Metainfos, Hinweise auf Täuschung etc.}}



## 🌄 Bekannte Aufenthalts Orte
```dataview
TABLE WITHOUT ID link(file.name) as "Bekannte Aufenthalts Orte", OrtTyp as "Ort Typ", Region
where contains(link(file.name), this.BekannteAufenthaltsOrte) or contains(link(file.name), this.OrtderErstenBegegnung)
sort file.name
```

## 📭 Erwähnungen 
```dataview
TABLE WITHOUT ID link(file.name) as "Erwähnt in", NoteIcon as "Notiz typ"
where contains(file.outlinks, this.file.link)
sort file.name
```