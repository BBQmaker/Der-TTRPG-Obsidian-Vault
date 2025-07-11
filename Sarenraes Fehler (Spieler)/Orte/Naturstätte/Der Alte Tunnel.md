---
Region: "[[Oberes Unterreich]]"
ErstentdeckunginSitzung: "[[001 -Operation Otto- Journal]]"
Assoziation:
  - keine
OrtStatus:
  - Verlassen
OrtTyp:
  - Ruine
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

Wir betreten dieses Gebiet im Rahmen unseres Ziels [[Otto Retten]].
Wir werden nach kurzer Zeit auf einige blutige Spuren aufmerksam - offenbar gehören sie Otto und noch einer weiteren Person.

Nach sechs weiteren Kilometern machen wir eine bemerkenswerte Entdeckung: die geschmolzenen Überreste eines ehemals großen und humanoiden Konstrukts.


nach 2h weg
Ein quadratischer Raum, mit einem Einsturz wo die Entführer lang sind.
eine anders loch ist auch da.

[[Urima Radiomus]] findet eine alte Goldmünze mit unbekannten wappen und zwei gekreuzete Schwertern

der rechte gang führt zur [[Stinkende Höhle]]
Linker gang ist unbekannt.

führt zu [[Unterirdische Labor Ruine]]


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
