---
Region: 
tags:
  - Sarenraes_Fehler/Ort/Naturstätte
OrtStatus:
  - Belebt
  - Verlassen
OrtTyp:
  - Ruine
  - Naturgebiet
  - Höhle
---
# 🗺️ `=this.file.name`
## 📋 Allgemeine Informationen 
- **📍 Name:** {{Ortsname}} 
- **🌍 Region:** {{Region oder Land}} 
- **🏙️ Typ:** {{Ortstyp (z. B. Ruine, Naturgebiet, Höhle)}} 
- **👥 Bevölkerung:** {{Bevölkerungsanzahl oder Beschreibung (z. B. "menschenleer", "kleines Dorf", "große Stadt")}} 
- **🗺️ Karte:** [[Link oder Beschreibung einer Karte, falls vorhanden]] 
- **⚙️ Status:** {{Status, z. B. belebt, verlassen, im Krieg}}

## 🏞️ Beschreibung 
{{Beschreibe den Ort: Architektur, Landschaft, Atmosphäre, wichtige Details. Zum Beispiel: Ist es ein lebhafter Marktplatz, eine düstere Ruine, oder ein ruhiger Wald?}}


## 🏛️ Wichtige Orte im Ort -
- **📌 Ort 1:** {{Name und Beschreibung des Ortes, z. B. Ruine, Naturgebiet, Höhle, Ruine}} 
- **📌 Ort 2:** {{Name und Beschreibung eines weiteren wichtigen Ortes}} 
- **📌 Ort 3:** {{Weitere wichtige Orte oder Gebäude}}

## 🤝 Wichtige Personen  -
- **👤 Person 1:** {{Name, Rolle/Funktion (z. B. Bürgermeister, Priester, Anführer einer Räuberbande), Beschreibung}} 
- **👤 Person 2:** {{Name, Rolle, Beschreibung}} 
- **👤 Person 3:** {{Weitere wichtige Personen}}


Von und hin


Ablauf
funde






## Encounter
```dataview
TABLE WITHOUT ID 
link(file.name) as "Encounter", OrtdesEncounters as "Ort", EncounteredInSession.Sitzungsnummer as "Sitzungsnummer"
from #Sarenraes_Fehler/Encounter  
WHERE OrtdesEncounters = link(this.file.name) AND file.name != "TemplateOrt"
SORT Sitzungsnummer ASC
```

