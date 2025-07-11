---
Region: "[[Die Oberfläche]]"
ErstentdeckunginSitzung: "[[004 -Im finsteren Turm- Journal]]"
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
auf [[Die Oberfläche]]
[[Skelett Encounter]]

Zweiter Stock:
Ein wenig Größer als die Wendel Treppe
4 Türen
Die Vermoderte Tür

Laboratorium wo An Leichen herum experimentiert wurden

Mehre Käfige im Raum 1,60 hoch und 1M lang und breit

Die Reste von eine Art Schlafzimmer 
ein Seltsames Loch in der Decke
Ein Skelett inklusive Rüstung liegt in der Mitte des Raumes

Wir sehe Düstere Stelle im Wald

Leiche von [[Oskar]]
Stab
Fullplate Rüstung Masterwerk ist auch Magisch
	-Unbekannt Faint
	-Unbekannt moderate
	-Railing    Faint 
Langschwert Meisterwerk Dies ist Magisch
	- Encantment Faint
	- Evokation Moderat
	-
Haufen Bücher 
Finden -> [[Tagebuch von Unbekannt]]


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
