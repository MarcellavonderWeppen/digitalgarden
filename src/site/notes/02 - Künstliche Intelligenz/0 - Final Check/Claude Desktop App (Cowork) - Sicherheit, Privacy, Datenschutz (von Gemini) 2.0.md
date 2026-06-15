---
{"title":"Claude Desktop App (Cowork) - Sicherheit, Privacy, Datenschutz (von Gemini) 2.0","aliases":null,"tags":null,"gen_ai_anteil":["Gemini 80%","Claude 20%"],"created":"2026-06-15","updated":null,"status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/0-final-check/claude-desktop-app-cowork-sicherheit-privacy-datenschutz-von-gemini-2-0/","dgPassFrontmatter":true,"dg-note-properties":{"title":"Claude Desktop App (Cowork) - Sicherheit, Privacy, Datenschutz (von Gemini) 2.0","aliases":null,"tags":null,"gen_ai_anteil":["Gemini 80%","Claude 20%"],"created":"2026-06-15","updated":null,"status":null}}
---



# Claude Desktop App (Cowork) - Sicherheit, Privacy, Datenschutz (von Gemini) 2.0


Die Einführung von **Claude Cowork** und der darin integrierten Fähigkeit **„Computer Use“** wird in der Sicherheits- und Datenschutz-Community intensiv debattiert. Die Technologie bietet enorme Erleichterungen bei der Wissensarbeit, erfordert jedoch eine differenzierte Risikobewertung. Man darf hierbei das Gesamtsystem nicht mit seiner riskantesten Funktion gleichsetzen.

## Die Architektur: Sandbox vs. Host-Zugriff

Um die Sicherheit richtig einzuschätzen, muss man zwischen dem Produkt und der spezifischen Funktion unterscheiden:

- **Claude Cowork (Standardmodus):** Wenn Claude lokale Dateien analysiert oder Code ausführt, läuft dieses System in einer isolierten, geschützten virtuellen Umgebung (Linux-VM). Das Host-Betriebssystem bleibt geschützt.
    
- **Die Funktion „Computer Use“:** Erst wenn Claude eine Aufgabe nicht über direkte Schnittstellen (Connectors) lösen kann, greift es auf „Computer Use“ zurück. In diesem Modus verlässt die KI die Sandbox, um den Bildschirm visuell zu erfassen und Maus sowie Tastatur des Host-Rechners zu steuern.
    

Daraus ergeben sich drei zentrale Diskussionspunkte in der Fachwelt:

### 1. Das Privatsphäre-Risiko: Visuelle Erfassung und Gegenmaßnahmen

Wenn der „Computer Use“-Pfad aktiv ist, fertigt Claude fortlaufend Screenshots des Bildschirms an, um zu verstehen, wo es hinklicken muss. Diese Bilder werden zur Analyse an die Server von Anthropic übermittelt.

- **Das Risiko:** Befinden sich sensible Daten im Hintergrund (z. B. offene Chatfenster, private Notizen oder Kundenakten), werden diese theoretisch mit erfasst.
    
- **Die Schutzplanken:** Die KI agiert nicht völlig ungefiltert. Anthropic nutzt Per-App-Berechtigungen (der Nutzer muss den Zugriff für jede Anwendung explizit freigeben) und blockiert standardmäßig kritische Bereiche wie Krypto-Wallets oder Trading-Plattformen über eine konfigurierbare Blockliste.
    

### 2. Das größte Sicherheitsrisiko: Prompt Injection

Die technisch größte Sorge von Sicherheitsforschern betrifft sogenannte „Indirect Prompt Injections“.

- **Das Problem:** Wenn Claude über „Computer Use“ den Browser steuert und eine manipulierte Webseite aufruft, kann darauf versteckter, bösartiger Text platziert sein. Da KI-Modelle oft schwer zwischen „Daten, die ich lesen soll“ und „Befehlen, die ich ausführen soll“ unterscheiden können, könnte ein Angreifer die KI dazu bringen, im Hintergrund unautorisierte Aktionen auszuführen.
    
- **Reale Relevanz:** Dieses Risiko ist real. Anthropic dokumentiert dies selbst und wies in Analysen darauf hin, dass ungehärtete Systeme (wie Claude for Chrome in frühen Tests) ohne Gegenmaßnahmen anfällig für solche Angriffe sein können. Experten raten daher strikt davon ab, der KI Zugriff auf Admin-Bereiche oder Banking-Portale zu erlauben.
    

### 3. Die „Native Messaging“-Kontroverse

Im Frühjahr 2026 sorgten Berichte des Datenschutzforschers Alexander Hanff für Diskussionen. Er stellte fest, dass die Claude Desktop-App für macOS eine Native-Messaging-Brücke in den Verzeichnissen mehrerer Chromium-Browser hinterlegt.

- **Die Kritik:** Es wurde bemängelt, dass dieser Schritt im Hintergrund und ohne explizites Opt-In für jeden einzelnen installierten Browser geschieht.
    
- **Die Einordnung:** Native Messaging ist ein legitimes Standard-Feature von Chromium, um Desktop-Apps mit Browser-Erweiterungen zu verbinden. Dennoch kritisieren Datenschützer den Mangel an Transparenz bei der Installation, da potenziell Berechtigungen im Voraus erteilt werden.
    

## Empfehlungen für eine sichere Nutzung

Die Sicherheits-Community und Anthropic selbst empfehlen einen risikobewussten Umgang nach dem Prinzip „Zero Trust“:

- **Zusätzliche Isolation für Computer Use:** Wer die visuelle Steuerung („Computer Use“) intensiv nutzt, sollte die gesamte Claude Desktop-App idealerweise innerhalb einer separaten Virtuellen Maschine (VM) betreiben. So bleibt ein potenzieller Ausbruch auf diese VM beschränkt.
    
- **Konsequente Nutzung der Blocklisten:** Sensible Anwendungen (Banking, Passwörter, HR-Tools) sollten konsequent für die KI gesperrt werden.
    
- **Human-in-the-Loop (Überwachung):** Claude sollte bei der Interaktion mit dem PC wie ein neuer Praktikant behandelt werden. Kritische Prozesse müssen aktiv vom Nutzer überwacht werden; Autopiloten ohne Aufsicht sind bei Host-Zugriffen tabu.
    

## Fazit

Claude Cowork ist dank seiner VM-Sandbox für die meisten Datei- und Codeoperationen gut abgesichert. Das eigentliche Risiko konzentriert sich auf die Funktion **Computer Use**. Diese ist technisch beeindruckend, durchbricht jedoch die Sandbox zum Host-System hin. Durch die Kombination aus den von Anthropic eingebauten App-Sperren und einer bewussten Überwachung durch den Nutzer lässt sich das Werkzeug in einem kontrollierten Rahmen jedoch produktiv einsetzen.