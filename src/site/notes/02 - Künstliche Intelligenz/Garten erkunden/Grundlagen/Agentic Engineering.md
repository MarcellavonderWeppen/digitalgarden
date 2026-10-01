---
{"title":"Agentic Engineering","aliases":null,"tags":null,"gen_ai_anteil":null,"created":"2026-06-18","updated":"2026-09-29","status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/garten-erkunden/grundlagen/agentic-engineering/","dgPassFrontmatter":true,"dg-note-properties":{"title":"Agentic Engineering","aliases":null,"tags":null,"gen_ai_anteil":null,"created":"2026-06-18","updated":"2026-09-29","status":null}}
---


# Agentic Engineering

> [!quote] You can outsource the thinking. You cannot outsource the understanding.
> <small>_- frei nach Andrej Karpathy_[^zitat]</small>

Nachdem Andrej Karpathy 2025 den Begriff [[02 - Künstliche Intelligenz/1 - Work on now/Vibecoding\|Vibecoding]] geprägt hatte, lieferte er Anfang 2026 mit _Agentic Engineering_ das „seriöse Gegenstück“ nach:

- Vibecoding hebt die Untergrenze an
- Agentic Engineering hebt die Obergrenze an

Mit anderen Worten: Vibecoding macht Programmieren für alle zugänglicher, aber Agentic Engineering stellt sicher, dass professionelle, produktionsreife Software trotz des Einsatzes unzuverlässiger KI-Agenten ihre Qualität behält.

## Auslöser

Karpathy nennt den Dezember 2025 als seinen persönlichen Wendepunkt: Über die Feiertage testete er agentische Coding-Tools intensiver, ließ sich immer größere Code-Abschnitte erzeugen – und konnte sich irgendwann nicht mehr erinnern, wann er den erzeugten Code zuletzt korrigiert hatte. Spätestens da war klar: Das geht über Vibecoding hinaus.


## Merkmale von Agentic Engineering

- **Der Mensch als Dirigent** ([[Human-in-the-Loop\|Human-in-the-Loop]]): Man schreibt den Code nicht mehr mühsam Zeile für Zeile selbst. Stattdessen orchestriert der Mensch KI-Systeme: Er verteilt Aufgaben, gibt die Richtung vor, prüft Ergebnisse und gibt sie am Ende frei.
- **Oft ein ganzes Team aus KI-Spezialisten (Multi-Agenten):** Statt eines einzelnen Chatbots arbeiten häufig mehrere KI-Agenten Hand in Hand. Einer plant das Projekt, ein anderer schreibt den Code und ein dritter sucht gezielt nach Fehlern – wie in einer echten Software-Firma.
- **Fehlersuche in Dauerschleife (Selbstkorrektur):** Bevor der Mensch das Ergebnis sieht, lässt die KI das Programm im Hintergrund testweise laufen. Stürzt es ab, liest die KI die Fehlermeldung und repariert den Code so lange eigenständig, bis er läuft und die Tests besteht.
- **KI mit echtem Werkzeugkasten (Tool-Nutzung):** Die Agenten schreiben nicht nur Texte. Sie können Programme eigenständig starten, Dateien auf dem Computer anlegen und digitale Prüfwerkzeuge benutzen, um die Qualität zu sichern.
- **Der Fokus verschiebt sich:** Als Programmierer überlegt man nicht mehr: _„Welche Codezeile tippe ich als Nächstes ein?“_, sondern: _„Was soll das System am Ende können und wie stabil muss es sein?“_
- **Keine Abkürzung für Anfänger:** Auch wenn die KI die meiste Arbeit macht – um so ein System zu steuern, braucht man tiefes Fachwissen. Man muss genau wissen, wie gute Software aufgebaut ist und wie man Fehler erkennt, sonst verliert man bei den riesigen Mengen an KI-Code sofort den Überblick.

## 📺 Aus der YouTube Academy

- Die charmante „Alberta in Tech“ geht der Frage nach: [Do Google engineers actually vibe code?](https://www.youtube.com/watch?v=PbsocBPkoUc) Man munkelt, sie habe früher selbst bei Google gearbeitet.

[^zitat]: Karpathy zitiert hier einen Tweet. [Quelle](https://www.mindstudio.ai/blog/karpathy-sequoia-talk-5-predictions-agentic-engineering)