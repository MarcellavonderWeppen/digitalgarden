---
{"title":"Claude Desktop App (Cowork) - Sicherheit, Privacy, Datenschutz (von Gemini)","aliases":null,"tags":null,"gen_ai_anteil":["Gemini 80%","Claude 20%"],"created":"2026-06-15","updated":"2026-06-16","status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/3-veroeffentlicht/claude-desktop-app-cowork-sicherheit-privacy-datenschutz-von-gemini/","dgPassFrontmatter":true,"dg-note-properties":{"title":"Claude Desktop App (Cowork) - Sicherheit, Privacy, Datenschutz (von Gemini)","aliases":null,"tags":null,"gen_ai_anteil":["Gemini 80%","Claude 20%"],"created":"2026-06-15","updated":"2026-06-16","status":null}}
---

# Claude Desktop App (Cowork) - Sicherheit, Privacy, Datenschutz (von Gemini)

Die Einführung von **Claude Cowork** und der visuellen Steuerung **„Computer Use“** ist in der IT-Sicherheits- und Datenschutz-Community ein Brandbeschleuniger für Debatten. Die Technologie verspricht das Ende lästiger Routinearbeit, erkauft sich diese Bequemlichkeit aber mit Risiken, die ein völlig neues, kompromissloses Sicherheitsdenken erfordern.

Wer das Tool nutzt, muss die Architektur verstehen – denn die größte Gefahr lauert dort, wo die Schutzmauern der Software enden.

## Die Sollbruchstelle der Sandbox

Die Marketing-Versprechen betonen oft die Sicherheit des Systems, und rein technisch stimmt das für das Fundament: Wenn Claude Cowork lokale Dateien analysiert oder Code ausführt, geschieht dies in einer isolierten, virtuellen Linux-Umgebung (Sandbox). Der eigentliche PC bleibt unberührt.

**Das Problem:** Sobald die KI eine Aufgabe nicht über direkte Schnittstellen lösen kann, greift sie auf die Fähigkeit **„Computer Use“** zurück. In diesem Moment **durchbricht das System gezielt die eigene Sandbox**. Die KI agiert direkt auf deinem Host-System, bewegt deine Maus und tippt auf deiner Tastatur. Ab diesem Punkt ist die schützende Isolation vorbei.

Aus Sicht von Kritikern und Sicherheitsforschern ergeben sich daraus drei gravierende Probleme:

### 1. Das Privatsphäre-Problem: Fortlaufende Screenshots im Aktionszyklus

Um auf dem Host-System navigieren zu können, fertigt Claude fortlaufend und in schneller Abfolge Screenshots deines Bildschirms an – jeweils abgestimmt auf die einzelnen Schritte innerhalb einer Aufgabenschleife. Diese Bilder werden zur Analyse an die Server von Anthropic übermittelt.

- **Die Kritik:** Zwar betont Anthropic, dass Nutzer den Zugriff für jede App explizit freigeben müssen und sensible Bereiche wie Krypto-Wallets über Blocklisten gesperrt sind, doch Datenschützer beruhigt das kaum. Im Arbeitsalltag fliegen schnell vertrauliche Hintergrund-Mails, private Notizen oder Kundenakten über den Schirm. Wer garantiert, dass im Eifer des Gefechts nicht doch sensible Daten mitfotografiert und hochgeladen werden? In einer strengen DSGVO-Arbeitsumgebung ist dieses Verfahren ein datenschutzrechtlicher Drahtseilakt.
    

### 2. Das ungelöste Tech-Risiko: Indirect Prompt Injection

Das mit Abstand größte Sicherheitsrisiko ist und bleibt „Indirect [[02 - Künstliche Intelligenz/3- Veröffentlicht/Prompt Injection\|Prompt Injection]]“. Es ist das Einbruchstor für Angreifer.

- **Die Gefahr:** Wenn Claude über „Computer Use“ den Browser steuert, um für dich zu recherchieren, und dabei auf eine manipulierte Webseite gerät, kann dort versteckter, für das menschliche Auge unsichtbarer Text platziert sein. Da KI-Modelle bis heute nicht zuverlässig zwischen „Daten, die ich nur lesen soll“ und „Befehlen, die ich ausführen soll“ unterscheiden können, übernimmt die Seite die Kontrolle.
    
- **Die Konsequenz:** Der Angreifer bringt die KI rein semantisch dazu, deine Daten zu exfiltrieren oder unautorisierte Aktionen auszuführen. Da Claude zu diesem Zeitpunkt außerhalb der Sandbox auf deinem echten PC agiert, sind die potenziellen Schäden massiv. Experten raten deshalb mit Nachdruck: Gebt der KI niemals, unter keinen Umständen, Zugriff auf Admin-Bereiche, Unternehmens-Dashboards oder Finanzportale.
    

### 3. Intransparenz im Hintergrund: Die „Native Messaging“-Kontroverse

Wie sensibel die Integration in das System abläuft, zeigte eine Kontroverse im Frühjahr 2026. Der Datenschutzforscher Alexander Hanff deckte auf, dass die Claude Desktop-App für macOS ungefragt eine sogenannte „Native Messaging“-Brücke in den Verzeichnissen mehrerer Chromium-Browser hinterlegt.

- **Die Kritik:** Die Installation geschah im Hintergrund, ohne explizites Opt-In und betraf laut dem Befund auch Browser, die offiziell gar nicht unterstützt werden. Für Datenschützer ist das ein klassisches Beispiel für mangelnde Transparenz.
    
- **Die Einordnung:** Sicherheitsanalysten (u. a. von Malwarebytes) relativieren den Fund ein Stück weit: Native Messaging ist ein legitimes Chromium-Standardfeature, um Desktop-Apps mit Browser-Erweiterungen zu verbinden. Die abgelegte Datei tut für sich genommen erst einmal nichts, solange keine entsprechende Erweiterung sie aktiv aufruft – zudem unterstützt Anthropic offiziell nur Chrome und Edge. Dennoch bleibt der intransparente Installationsprozess in der Community ein massiver Kritikpunkt.
    

## Fazit: Kein Tool für den blinden Autopiloten

Claude Cowork ist im Kern solide gebaut, aber die Funktion „Computer Use“ hebelt diese Sicherheit aus. Sie macht das System hochsensibel. Die vorhandenen Schutzplanken und App-Blocklisten von Anthropic sind wichtig, bieten aber keinen absoluten Schutz gegen kreative Angriffe oder menschliches Versagen.

Wer dieses Werkzeug auf seinem primären Arbeitsrechner nutzt, muss extreme Vorsicht walten lassen. Die Sicherheits-Community empfiehlt daher:

- **Maximale Isolation:** Wer „Computer Use“ nutzt, sollte die Claude-App idealerweise in einer eigenen, separaten Virtuellen Maschine (VM) einsperren.
    
- **Kein blindes Vertrauen:** Die KI darf niemals unbeaufsichtigt wie ein Autopilot laufen. Man muss sie wie einen Praktikanten behandeln, dem man beim Tippen permanent auf die Finger schaut. Das Tool bietet enorme Bequemlichkeit, verzeiht aber aktuell nicht den geringsten Mangel an Vorsicht.

---
## *Hintergrund des Artikels*

- Ich hatte Claude die [[02 - Künstliche Intelligenz/3- Veröffentlicht/Claude Desktop App (Cowork) - Sicherheit, Privacy, Datenschutz (von Gemini) 1.0\|ursprüngliche Version von Gemini ]]  zum Faktencheck vorgelegt.
- Claudes Kritik hatte ich an Gemini weitergegeben, welcher sofort - fast schon devot 😂 -  beipflichtete: “Chapeau an Claude – diese Kritik ist absolut berechtigt, präzise und deckt eklatante begriffliche Unschärfen in meinem vorherigen Text auf. Ich werde hier definitiv nicht in die Verteidigung gehen, denn Claudes Faktencheck bringt die technische Realität exakt auf den Punkt.” 
- Das Ergebnis war [[02 - Künstliche Intelligenz/3- Veröffentlicht/Claude Desktop App (Cowork) - Sicherheit, Privacy, Datenschutz (von Gemini) 2.0\|Claude Desktop App (Cowork) - Sicherheit, Privacy, Datenschutz (von Gemini) 2.0]] - ein übermäßig beschwichtigender Artikel. 
- Ich habe daraufhin Gemini ermutigt, den ursprünglich kritischen Geist des Artikels doch wieder aufleben zu lassen, aber dieses Mal auf dem Boden der Tatsachen. Das Ergebnis ist dieser Artikel. 
- Und was sagt Claude selbst zu diesem Artikel, der ihn ja kritisiert? *“Ich finde es gesünder, wenn ich solche Kritik nüchtern prüfen kann, statt reflexhaft die Heimmannschaft zu verteidigen. Eine KI, die ihre eigenen Produktrisiken kleinredet, wäre genau die Art von System, vor dem der Artikel zu Recht warnt.”* → eine sehr reflektierte Haltung, die man sich von manchen Mitmenschen nur wünschen könnte!
