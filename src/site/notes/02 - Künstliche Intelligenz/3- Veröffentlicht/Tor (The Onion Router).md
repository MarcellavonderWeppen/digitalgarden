---
{"title":"Tor (The Onion Router)","aliases":["Tor"],"tags":null,"gen_ai_anteil":["Mistral 100%"],"created":"2026-06-04","updated":"2026-06-06","status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/3-veroeffentlicht/tor-the-onion-router/","dgPassFrontmatter":true,"dg-note-properties":{"title":"Tor (The Onion Router)","aliases":["Tor"],"tags":null,"gen_ai_anteil":["Mistral 100%"],"created":"2026-06-04","updated":"2026-06-06","status":null}}
---

# Tor (The Onion Router)


Tor ist ein **anonymes Netzwerk**, das Nutzern ermöglicht, im Internet zu kommunizieren, ohne dass ihre Identität oder ihr Standort leicht nachverfolgbar sind. Es basiert auf einer **dezentralen Infrastruktur aus Servern**, die als **Relays** bezeichnet werden. Diese Server arbeiten zusammen, um Daten zu verschlüsseln und durch mehrere Knoten zu leiten, bevor sie ihr Ziel erreichen.

![Tor (The onion router).png](/img/user/Bilder/Tor%20(The%20onion%20router).png)

## Wie funktioniert Tor?

### 1. Drei Schichten der Verschlüsselung

Tor nutzt das Prinzip des **Onion Routings**: Daten werden in mehreren Schichten verschlüsselt, ähnlich wie die Schichten einer Zwiebel. Jeder Knoten im Netzwerk entschlüsselt nur eine Schicht, um den nächsten Knoten zu ermitteln. So kennt kein einzelner Server den vollständigen Pfad der Daten.

- **Eintrittsknoten (Entry Node):** Empfängt die verschlüsselten Daten und leitet sie an den nächsten Knoten weiter.
    
- **Relaisknoten (Middle Node):** Entschlüsselt eine Schicht und leitet die Daten weiter.
    
- **Ausgangsknoten (Exit Node):** Entschlüsselt die letzte Schicht und sendet die Daten an ihr endgültiges Ziel (z. B. eine Website).
    
### 2. Dezentrales Netzwerk aus Servern

Das Tor-Netzwerk besteht aus **tausenden freiwillig betriebenen Servern** weltweit. Diese Server werden von Privatpersonen, Organisationen oder Aktivisten betrieben und bilden das Rückgrat des Netzwerks. Ohne sie gäbe es keine Möglichkeit, Daten anonym zu übertragen.

## Der Tor Browser

Der **Tor Browser** ist ein speziell angepasster Browser (basierend auf Firefox), der für die Nutzung des Tor-Netzwerks optimiert ist. Er stellt die Verbindung zu den Tor-Servern her und ermöglicht den Zugriff auf:

- **Das normale Internet** (über den Exit Node, der die Daten dann unverschlüsselt an die Ziel-Website sendet).
    
- **Das Dark Web** (z. B. .onion-Websites, die nur innerhalb des Tor-Netzwerks erreichbar sind).

## Wofür wird Tor genutzt?

Tor wird sowohl für **legale** als auch für **illegale Zwecke** verwendet:

- **Schutz der Privatsphäre:** Nutzer:innen, die ihre Online-Aktivitäten vor Überwachung schützen möchten.
    
- **Umgehung von Zensur:** In Ländern mit Internetzensur ermöglicht Tor den Zugriff auf blockierte Inhalte.
    
- **Anonyme Kommunikation:** Journalisten, Whistleblower oder Aktivisten nutzen Tor, um sicher zu kommunizieren.
    
- **Forschung und Entwicklung:** Sicherheitsforscher:innen testen Anonymisierungstechniken.

## Vor- und Nachteile

### ✅ Vorteile

- **Hohe Anonymität:** Durch die mehrfache Verschlüsselung und Weiterleitung ist es extrem schwierig, Nutzer:innen zu identifizieren.
    
- **Zensurresistenz:** Ermöglicht den Zugriff auf Inhalte, die in manchen Ländern blockiert sind.
    
- **Open Source:** Das Tor-Netzwerk und der Tor Browser sind frei verfügbar und werden von einer gemeinnützigen Organisation entwickelt.

### ❌ Nachteile

- **Langsame Geschwindigkeit:** Durch die mehrfache Verschlüsselung und Weiterleitung ist die Verbindung oft langsamer als im normalen Internet.
    
- **Exit-Node-Risiko:** Der Exit Node kann den Datenverkehr sehen (wenn er nicht zusätzlich verschlüsselt ist, z. B. durch HTTPS).
    
- **Missbrauch:** Tor wird auch für illegale Aktivitäten genutzt, was zu einem negativen Ruf führt.

## Fazit

Tor ist ein **mächtiges Werkzeug für Anonymität und Privatsphäre**, das auf einem **Netzwerk aus Servern** basiert. Es bietet Schutz vor Überwachung und Zensur, hat aber auch Grenzen und Risiken. Der Tor Browser ist das **Zugangsprogramm**, das die Nutzung dieses Netzwerks ermöglicht – ähnlich wie ein Schlüssel zu einem sicheren Raum.