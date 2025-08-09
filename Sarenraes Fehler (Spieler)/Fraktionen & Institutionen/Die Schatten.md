---
typ:
  - fraktion
InitialebegegnunginSession: 
Status:
  - Aktiv
HaltungzuSpieler:
  - 🤝 neutral
  - negativ
tags:
  - Sarenraes_Fehler/Fraktionen_Institutionen
---
# 🏛️` =this.file.name`
#Sarenraes_Fehler/To_Do 
## 🧾 Überblick
- 🏷️ **Name**: {{offizieller Name oder Spitzname}}
- 🗺️ **Ort / Einflussgebiet**: [[Ort oder Region]]
- ⚖️ **Ausrichtung**: {{z. B. religiös, militärisch, kriminell, wirtschaftlich}}
- 🧠 **Erster Eindruck**: {{Was denkt dein SC über diese Fraktion?}}

## 🗣️ Beziehung zu uns
- 🤝 **Haltung zu unserer Gruppe**: 🤝 neutral / ❤️ freundlich / 💀 feindlich / 🌀 unklar  
- 🎯 **Interesse an uns**: {{Was wollen sie von uns? Warum interessieren sie sich für uns?}}
- ⚠️ **Gefahren / Chancen**: {{Was können sie uns bieten oder antun?}}

## 🧑‍🤝‍🧑 Bekannte Mitglieder
- 👑 **Anführer:in**: NSC – {{Was wissen wir über sie?}}
- 👥 **Weitere Kontakte**:  
  - NSC 1 – {{Rolle, Verhalten}}
  - NSC 2 – {{Verbindung zu uns?}}

## 📆 Was bisher geschah
- 🧭 **Erster Kontakt**: {{Wann, wo, wie?}}  
- 📜 **Zusammenfassungen**:  
  - {{Sitzung 5: Wir trafen ihren Späher im Wald}}  
  - {{Sitzung 8: Bot uns Schutz gegen Bezahlung an}}

## 🤫 Gerüchte & Theorien
- 🕵️ **Was wir gehört haben**:  
  - {{z. B. Sie arbeiten mit Untoten?}}
  - {{Ein Mitglied soll ein Ex-Adliger sein?}}

## 🧩 Eigene Notizen
- 🗒️ {{Vermutungen, geplante Aktionen, Erinnerungsstützen für deinen SC}}

## 📭 Erwähnungen 
```dataview
TABLE WITHOUT ID link(file.name) as "Erwähnt in", NoteIcon as "Notiz typ"
where contains(file.outlinks, this.file.link)
sort file.name
```