---
{"title":"Claude Desktop App - Sicherheit, Privacy, Datenschutz (Kurzfassung von Gemini)","aliases":null,"tags":null,"gen_ai_anteil":["Gemini 100%"],"created":"2026-06-12","updated":null,"status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/0-final-check/claude-desktop-app-sicherheit-privacy-datenschutz-kurzfassung-von-gemini/","dgPassFrontmatter":true,"dg-note-properties":{"title":"Claude Desktop App - Sicherheit, Privacy, Datenschutz (Kurzfassung von Gemini)","aliases":null,"tags":null,"gen_ai_anteil":["Gemini 100%"],"created":"2026-06-12","updated":null,"status":null}}
---


# Claude Desktop App - Sicherheit, Privacy, Datenschutz (Kurzfassung von Gemini)


Die Bewertung von „Claude Cowork“ (offiziell als „Computer Use“ bezeichnet) ist in der Sicherheits- und Datenschutz-Community ein intensiv debattiertes Thema. Die kurze Antwort lautet: **Es ist ein mächtiges Werkzeug, erfordert aber ein völlig neues Sicherheitsdenken.**

Da dieses System nicht in einer isolierten „Sandbox“ (einem geschützten Bereich) läuft, sondern direkt deine Maus bewegt, tippt und deinen Bildschirm „sieht“, bewerten Experten die Risiken als deutlich höher als bei einem normalen KI-Chat.

Hier ist eine Zusammenfassung, wie diese Perspektiven aussehen:

### 1. Das Hauptrisiko: „Die KI sieht alles“

Der größte Kritikpunkt an der Privatsphäre ist, dass Claude durch die „Computer Use“-Funktion aktiv Screenshots deines Bildschirms macht.

- **Was Experten sagen:** Wenn die KI deine Fenster „sieht“, kann sie theoretisch alle Informationen erfassen, die dort zu sehen sind – auch solche, die du ihr gar nicht explizit gegeben hast (z. B. eine E-Mail im Hintergrund, private Notizen oder vertrauliche Firmendaten).
    
- **Datenschutz:** Da diese Screenshots zur Analyse an Anthropic-Server gesendet werden, sind viele Datenschützer sehr vorsichtig, wenn es darum geht, die Funktion in einer Arbeitsumgebung mit personenbezogenen Daten zu nutzen.
    

### 2. Das Sicherheitsrisiko: „Prompt Injection“

Dies ist die größte technische Sorge. „Prompt Injection“ beschreibt einen Angriff, bei dem eine KI durch bösartige Inhalte (z. B. versteckter Text auf einer Webseite, die du besuchst) dazu verleitet wird, Befehle auszuführen, die nicht von dir stammen.

- **Das Problem:** Wenn Claude deinen Browser steuert und eine Webseite mit bösartigem Code aufruft, könnte der Angreifer versuchen, die KI dazu zu bringen, sensible Daten zu exfiltrieren oder Aktionen auszuführen, die du nicht autorisiert hast.
    
- **Bewertung:** Sicherheitsforscher weisen darauf hin, dass die KI oft nicht sauber zwischen „Daten, die ich lese“ und „Anweisungen, die ich ausführe“ unterscheiden kann. Deshalb raten Experten dringend davon ab, der KI Zugriff auf kritische Systeme wie Bankenportale, Unternehmens-Dashboards oder Admin-Bereiche zu geben.
    

### 3. Transparenz und „Dark Patterns“

Kritiker haben bemängelt, dass manche Integrationsschritte (vor allem bei der Browser-Anbindung) nicht immer transparent genug für den Nutzer sind. Es gab Berichte über versteckte „Native Messaging“-Brücken, die es dem Programm erlauben, ohne ständiges Nachfragen auf Browser-Daten zuzugreifen. Nutzer und Datenschutz-Aktivisten fordern hier mehr Kontrolle und eine striktere „Opt-in“-Politik, bei der man genau sieht, was die KI gerade darf.

### Wie man das sicher angeht

Die Sicherheits-Community ist sich einig, dass man das Werkzeug nicht einfach „blind“ laufen lassen sollte. Die Empfehlungen zur Nutzung lauten daher meist:

- **Isolation:** Nutze „Computer Use“ idealerweise in einem **virtuellen Rechner (VM) oder einem Container**. So hat die KI nur Zugriff auf eine isolierte Umgebung und kann bei einem Fehler nicht auf deine privaten Haupt-Dateien zugreifen.
    
- **Keine kritischen Passwörter:** Gib der KI niemals direkten Zugriff auf Bereiche, in denen du dich mit wichtigen Passwörtern oder Zahlungsinformationen einloggst.
    
- **„Human-in-the-Loop“:** Behandle Claude bei der Arbeit an deinem PC wie einen Praktikanten, dem man nicht trauen kann, allein eine Überweisung zu tätigen. Überwache den Prozess aktiv.
    
- **Browser-Hygiene:** Erlaube der KI nur Zugriff auf Webseiten, denen du vertraust.
    

**Fazit:** Die Funktion ist technisch beeindruckend, aber aus Sicherheits- und Datenschutzsicht wird sie derzeit als „hochsensibel“ eingestuft. Unternehmen und sicherheitsbewusste Nutzer sollten den Zugriff auf sensible Daten für die KI **physisch oder systemseitig beschränken**, anstatt sich nur auf die Sicherheitsvorkehrungen der Software zu verlassen.


## 📖 Weiterlesen 

- Lange ausführliche Fassung (kritisch): [[02 - Künstliche Intelligenz/0 - Final Check/Claude Desktop App - Sicherheit, Privacy, Datenschutz (von Mistral)\|Claude Desktop App - Sicherheit, Privacy, Datenschutz (von Mistral)]]
- Im Zweifelsfalle für den Angeklagten: [[02 - Künstliche Intelligenz/0 - Final Check/Claude Desktop App aus der Sicht von Claude\|Claude Desktop App aus der Sicht von Claude]]