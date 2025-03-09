---
Region: 
Assoziation: keine
OrtStatus:
  - Belebt
  - Verlassen
OrtTyp:
  - Ruine
  - Naturgebiet
  - Höhle
tags:
  - Sarenraes_Fehler/Ort/Naturstätte
---
# 🗺️ `=this.file.name`
## 📋 Allgemeine Informationen 
- **📍 Name:** `=this.file.name`
- **🌍 Region:** `=this.Region`
- **🏙️ Typ:** `=this.OrtTyp`
- **👥 Bevölkerung:** {{Bevölkerungsanzahl oder Beschreibung (z. B. "menschenleer", "kleines Dorf", "große Stadt")}} 
- **🗺️ Karte:** [[Link oder Beschreibung einer Karte, falls vorhanden]] 
- **⚙️ Status:** `=this.OrtStatus`

## 🏞️ Beschreibung 
{{Beschreibe den Ort: Architektur, Landschaft, Atmosphäre, wichtige Details. Zum Beispiel: Ist es ein lebhafter Marktplatz, eine düstere Ruine, oder ein ruhiger Wald?}}


## 🗺️ Benachbarte Orte 
{{Liste von Orten in der Nähe, die möglicherweise relevant sind, z. B. ein angrenzender Wald, ein Dorf, ein Gebirgspfad.}} 
- **➡️ Richtung & Entfernung:** {{Wie gelangt man dorthin? (z. B. "2 Stunden Fußweg nach Norden.")}}

## 🗒 Unterorte
{{Liste von Unterorten oder besonderen Bereichen innerhalb dieses Ortes, z. B. ein verstecktes Tal, ein unterirdischer Tunnel, ein Heiligtum.}}

## 📅Timeline/Ablauf
{{Hier Ablauf, Funde, Encounter verlinken und besondere Ereignisse oder Veränderungen dokumentieren.}}


## 🐓Encounter
```dataview
TABLE WITHOUT ID 
link(file.name) as "Encounter", OrtdesEncounters as "Ort", EncounteredInSession.Sitzungsnummer as "Sitzungsnummer"
from #Sarenraes_Fehler/Encounter  
WHERE OrtdesEncounters = link(this.file.name) AND file.name != "TemplateOrt"
SORT Sitzungsnummer ASC
```


## 📜 Sonstige Notizen 
{{Zusätzliche Anmerkungen, die den Ort betreffen.}}
