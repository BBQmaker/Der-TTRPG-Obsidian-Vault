---
Region: "[[Oberes Unterreich]]"
ErstentdeckunginSitzung: "[[002 -Kytone, Engel und andere Probleme- Journal]]"
Assoziation:
  - keine
OrtStatus:
  - Belebt
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
von [[Stinkende Höhle]]
von [[Der Alte Tunnel]]



Wir beobachten Reliefs an den Wänden, welche wir nicht einordnen können.


> [!NOTE] Fund
> Scroll von [[Nap Stack]]
eine [[Mystery box]] in einem Geheimfach

Nach einer mittleren Wegstrecke, bei der wir einen leichten Höhenanstieg beobachten, gelangen wir in einen großen Raum, der wie ein Labor eingerichtet ist. Wir werden von einem Outsider attackiert, es kommt zum [[Kyton Encounter]].

> [!NOTE] Fund: Labor
> 200gp
2 Scrolls: Comprehend Languages
2 Ölige Flüssigkeiten
ein glas mit dem Blut eines Outsiders

Im Anschluss entdecken wir einen Abschnitt, der offenbar als eine Art Gefängnis dient.

> [!NOTE] Fund: Gefängnis
> Schwarzer Schlüsselbund

Zudem entdecken wir mehrere Gefangene:
zwei zerschundene, maskulin aussehende Personen, eine kleine [[Azata]] namens [[Herulith]] sowie eine zerschundene Elfe( [[Allynna Ilivaris]]).

Direkt nach dem Gefängnis kommen wir in eine Bibliothek, aus der wir einige Bücher zur weiteren Untersuchung mitnehmen.


> [!NOTE] Fund: Bibliothek
> Mehre Anatomie Bücher 
Unter anderem Bücher von der Anatomie von Engel

Bevor wir die Bibliothek verlassen und voranschreiten können, belauschen wir ein Gespräch, welches aus den bisher unerkundeten Gebieten der Anlage zu uns dringt. In diesem scheint eine uns noch unbekannte Entität ([[Mysteriöse Stimme]]) den Verantwortlichen für diese Anlage zu rügen, bevor das Gespräch beendet wird. Wir schreiten in den nächsten Raum und beginnen den [[Boss Kyton Encounter]].


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
