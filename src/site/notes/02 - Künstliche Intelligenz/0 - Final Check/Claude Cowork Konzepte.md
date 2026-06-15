---
{"title":"Unbenannt","aliases":null,"tags":null,"gen_ai_anteil":["Gemini 100%"],"created":"2026-06-15","updated":null,"status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/0-final-check/claude-cowork-konzepte/","dgPassFrontmatter":true,"dg-note-properties":{"title":"Unbenannt","aliases":null,"tags":null,"gen_ai_anteil":["Gemini 100%"],"created":"2026-06-15","updated":null,"status":null}}
---


# Claude Cowork Konzepte

Quelle: [Every Claude Cowork Concept Explained for Normal People](https://www.youtube.com/watch?v=NDHWUhGzKg0)📺

Dieses Video von Brock Mesarich (Kanal: _AI for Non Techies_) erklärt die **20 wichtigsten Kernkonzepte von Claude Co-work**. Die Erklärung ist so aufgebaut, dass sie von der einfachen Datei-Organisation bis hin zu komplexen, automatisierten Workflows führt.

Hier sind die 20 Konzepte, übersichtlich in Themenbereiche unterteilt:

### 1. Die grundlegende Umgebung & Einrichtung

- **Workspace Folder (Arbeitsbereich-Ordner) `[00:01:05]`**: Ein bestimmter Ordner auf Ihrem Computer, auf den Claude Co-work direkt zugreifen kann. Dort liest, bearbeitet und erstellt das Tool Dateien (wie Python-Skripte, HTML-Dashboards oder CSV-Dateien).
    
- **Claude.md `[00:03:09]`**: Eine projektspezifische Anweisungsdatei im Markdown-Format, die in Ihrem Arbeitsordner liegt. Claude liest diese Datei zu Beginn jeder Sitzung, um die Regeln und den Kontext für genau dieses Projekt zu verstehen.
    
- **Global Instructions (Globale Anweisungen) `[00:05:06]`**: Ihre dauerhafte Identität und Verhaltensregeln, die für alle Claude-Sitzungen (sowohl im normalen Chat als auch im Co-work-Modus) gelten – im Gegensatz zur projektbasierten `claude.md`.
    
- **Memory (Gedächtnis) `[00:06:36]`**: Ein Bereich, in dem Claude über verschiedene Chats hinweg wichtige Erkenntnisse, Vorlieben und Feedback speichert, um sich langfristig an Sie anzupassen.
    
- **Context Window (Kontextfenster) `[00:07:46]`**: Der temporäre „Arbeitstisch“ eines Chats. Aktuell fasst er bis zu 1 Million Token und beinhaltet die `claude.md`, den Chatverlauf, hochgeladene Dateien und Tool-Ausgaben.
    

### 2. Grundfunktionen & Ausgaben

- **Multimodal (Multimodalität) `[00:08:31]`**: Die Fähigkeit von Claude, verschiedene Eingabeformate wie Bilder, Screenshots, PDFs und Texte zu „sehen“ und zu verarbeiten (direkte Video-Eingaben werden aktuell nicht unterstützt).
    
- **Web Search (Websuche) `[00:09:11]`**: Das Werkzeug, mit dem Claude das Internet nach aktuellen Informationen und Preisen durchsuchen kann, um das Wissenslimit (wird im Video mit Mai 2025 angegeben) zu umgehen.
    
- **Extended Thinking (Erweitertes Denken) `[00:09:41]`**: Eine Funktion, bei der Claude mehr Zeit investiert, um komplexe Logikprobleme tiefgründig zu durchdenken, was zu qualitativ besseren Antworten führt.
    
- **Artifacts (Artefakte) `[00:10:08]`**: Visuelle Ausgaben in einem separaten Fenster (wie interaktive HTML-Dashboards, Diagramme oder Präsentationen), anstatt reiner Textabsätze im Chat.
    
- **Projects (Projekte) `[00:11:23]`**: Getrennte Arbeitsbereiche innerhalb eines Accounts, die jeweils eigene Dateien, Erinnerungen und Anweisungen haben, damit verschiedene Aufgabenbereiche sauber getrennt bleiben.
    
- **Bash Tool `[00:13:44]`**: Die technische Schnittstelle, über die Claude Programmiercode direkt auf Ihrem lokalen System ausführen kann (z. B. um Dateien massenhaft umzubenennen oder Bilder anzupassen).
    

### 3. Workflows & Integrationen

- **Skills (Fähigkeiten) `[00:14:20]`**: Vorgefertigte Workflows und Anweisungen im Markdown-Format, die Claude genau vorgeben, wie eine bestimmte, mehrstufige Aufgabe fehlerfrei ausgeführt werden soll.
    
- **Slash Commands (Slash-Befehle) `[00:16:49]`**: Trigger-Wörter (wie z. B. `/morning-briefing`), die Sie in das Chatfenster eintippen, um einen bestimmten Skill sofort zu starten.
    
- **Plugins `[00:17:14]`**: Eine gebündelte Sammlung mehrerer Skills in einer einzigen Zip-Datei, die man einfach importieren oder mit Teammitgliedern teilen kann.
    
- **Connectors (Konnektoren) `[00:18:53]`**: Schnittstellen, die externe Apps (wie Google Calendar, Slack oder QuickBooks) mit Claude verknüpfen, sodass die KI eigenständig Daten in diesen Apps lesen und schreiben kann.
    
- **Claude in Chrome (Browser-Erweiterung) `[00:23:42]`**: Eine Chrome-Erweiterung, mit der Claude Webseiten aufrufen, Formulare ausfüllen oder Flüge buchen kann – besonders nützlich für Plattformen ohne direkte API-Schnittstelle.
    

### 4. Fortgeschrittene Automation & Steuerung

- **Computer Use (Computernutzung) `[00:25:08]`**: Eine Funktion, bei der Claude die Benutzeroberfläche Ihres Betriebssystems steuern darf (z. B. Apps wie Videoprogramme öffnen und Dateien per Drag-and-Drop verschieben). Laut Video noch recht langsam, aber mächtig.
    
- **Scheduled Tasks (Geplante Aufgaben) `[00:26:56]`**: Automatisierungen direkt in Co-work, die externe Tools wie n8n oder Make überflüssig machen. Sie triggern Ihre erstellten Skills vollautomatisch zu bestimmten Uhrzeiten (z. B. jeden Morgen um 9 Uhr).
    
- **Dispatch Mode (Versand-Modus) `[00:29:00]`**: Eine Schnittstelle, über die Sie Claude von unterwegs per Smartphone Befehle erteilen können, die das Tool dann zu Hause auf Ihrem Desktop-Computer ausführt (z. B. „Lade das Video in Google Drive hoch“).
    
- **Sub Agents (Sub-Agenten) `[00:30:00]`**: Das Konzept, bei dem Claude für eine komplexe Aufgabe mehrere spezialisierte KI-Arbeiter parallel einsetzt (während Agent 1 Marktforschung betreibt, zieht Agent 2 die Finanzen und Agent 3 baut die Präsentationsfolien).