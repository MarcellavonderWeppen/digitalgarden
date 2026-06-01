---
{"title":"Morpheus Video zu KI und OpenSource","aliases":null,"tags":null,"gen_ai_anteil":["Gemini 80%"],"created":"2026-05-26","updated":null,"status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/2-veroeffentlicht/morpheus-video-zu-ki-und-open-source/","dgPassFrontmatter":true,"dg-note-properties":{"title":"Morpheus Video zu KI und OpenSource","aliases":null,"tags":null,"gen_ai_anteil":["Gemini 80%"],"created":"2026-05-26","updated":null,"status":null}}
---


# Morpheus Video zu KI und OpenSource

Sehr lohnenswertes Video zum Thema [[02 - Künstliche Intelligenz/2- Veröffentlicht/KI und Open Source\|KI und Open Source]]:

📺 [Die Open Source Community bricht zusammen](https://www.youtube.com/watch?v=yi1QiqlB1Q4) von _The Morpheus_

Im Folgenden die Zusammenfassung - ausdrücklich zum neugierig machen, nicht als Ersatz für das selber Gucken. Morpheus bringt immer wieder nachdenkliche und treffende Perspektiven in die ganze KI-Thematik. Meiner Meinung nach der beste deutschsprachige Content-Creator zum Thema. 

## Zusammenfassung des Videos 

In diesem Video von _The Morpheus_ wird eine tiefgreifende, strukturelle Krise der Open-Source-Community beleuchtet. Das Video argumentiert, dass das Fundament der digitalen Welt – das zu 70 bis 90 % aus offenem, frei zugänglichem Code besteht – derzeit unter dem Einfluss von künstlicher Intelligenz und chronischer Überlastung der Entwickler wegbricht.

Hier sind die Kernpunkte und Mechanismen, die im Video detailliert erklärt werden:

### 1. Das XZ-Utils-Dilemma als Warnschuss

Das Video startet mit dem realen Vorfall vom 29. März 2024 `[00:00:00]`. Ein Microsoft-Entwickler entdeckte durch eine minimale Verzögerung von einer halben Sekunde eine staatlich gesponserte Hintertür in dem kleinen Open-Source-Programm _XZ Utils_. Die Software wurde von einem einzigen, völlig erschöpften und unbezahlten Entwickler (Lasse Collin) in seiner Freizeit gepflegt `[00:02:42]`. Ein Angreifer nutzte diese Erschöpfung aus, schlich sich als helfender Kollege ein und schleuste die Backdoor ein. Wäre sie unentdeckt geblieben, hätten Angreifer Zugriff auf einen Großteil der weltweiten Server-Infrastruktur gehabt.

### 2. Warum KI die "Skalenökonomie" von Open Source umkehrt

Bisher funktionierte Open Source über einen selbstverstärkenden Kreislauf: Software baut auf Software auf, wodurch die Entwicklung für alle schneller und günstiger wird `[00:05:41]`. Open-Source-Entwickler wurden zwar selten mit Geld bezahlt, dafür aber mit **Aufmerksamkeit und Sichtbarkeit** (Jobangebote, Vorträge, Prestige) `[00:11:27]`.

Durch den Boom von KI-Tools (wie ChatGPT oder GitHub Copilot) ändert sich das radikal:

- **Verlust der Sichtbarkeit:** Entwickler fragen direkt die KI nach Code-Lösungen, anstatt die Dokumentation des Projekts zu besuchen oder auf Plattformen wie _Stack Overflow_ zu interagieren `[00:10:24]`. Die Nutzung der Tools steigt zwar, aber der Traffic und die Belohnung für die Ersteller brechen ein (am Beispiel des Web-Tools _Tailwind_ gezeigt, dessen Doku-Traffic um 40 % sank) `[00:09:38]`.
    
- **Die Prüfungs-Asymmetrie:** Durch KI ist es extrem billig geworden, Code-Beiträge oder Bug-Reports zu generieren, aber es bleibt genauso teuer und zeitaufwendig für die menschlichen Betreuer (Maintainer), diese zu prüfen `[00:15:18]`. Der Entwickler von _Curl_ musste beispielsweise sein Bug-Bounty-Programm fast einstellen, weil über 95 % der Einreichungen KI-generierter Spam und Halluzinationen waren `[00:13:35]`.
    

### 3. Transparenz wird zur Angriffsfläche

Ein weiterer Paradigmenwechsel betrifft die Sicherheit `[00:15:39]`. Jahrelang galt das Prinzip: _"Viele Augen sehen viele Fehler"_ (offener Code ist sicherer). Im April 2026 erklärte die Firma _Cal.com_ (eine Open-Source-Alternative zu Calendly) dieses Prinzip für tot und wechselte zu Closed Source (_"Cal.com goes closed source"_) `[00:16:08]`. Die Begründung: KI-Systeme können öffentlichen Code in einer Geschwindigkeit nach Schwachstellen scannen, die für menschliche Verteidiger unmöglich einzuholen ist. Offener Code wird so zum Bauplan für Angreifer.

### 4. Menschliche Ausbeutung und Frustration

Die digitale Infrastruktur basiert laut dem Video darauf, dass kontinuierlich "ausgebrannte Pfleger durchgeschleust werden" `[00:21:37]`. Entwickler tragen die rechtliche und technische Verantwortung für Code, von dem Milliardenkonzerne abhängen, werden bei Fehlern wie Zulieferer blockiert, bei der Bezahlung aber wie reine Hobbyisten behandelt `[00:21:55]`. Hinzu kommt eine zunehmende Toxizität und Anspruchshaltung von Nutzern in den Kommentaren `[00:20:42]`.

Zusätzlich sorgt für Unmut, dass Plattformen wie GitHub (Microsoft) die unbezahlte Arbeit von Open-Source-Entwicklern ungefragt nutzen, um ihre kommerziellen KI-Modelle (Copilot) zu trainieren, ohne den Entwicklern eine Opt-Out-Möglichkeit für öffentliche Daten zu geben `[00:22:56]`.

### 5. Lösungsansätze nach Elinor Ostrom

Um das Problem zu lösen, zieht der Betreiber des Kanals die Arbeit der Wirtschaftsnobelpreisträgerin Elinor Ostrom über Gemeingüter (wie Fischerei oder Wälder) heran `[00:29:17]`. Open Source ist ein digitales Gemeingut. Während riesige Projekte wie Linux feste Strukturen haben und überleben `[00:30:12]`, fehlen kleinen Projekten die Mechanismen gegen Trittbrettfahrer.

Folgende strukturelle Lösungen werden diskutiert:

1. **Staatliche Förderung:** Initiativen wie die deutsche _Sovereign Tech Agency_ zeigen gute Ansätze `[00:34:09]`, sind jedoch finanziell im Vergleich zu den dreistelligen Millionenbeträgen, die der Staat für Closed-Source-Lizenzen (z. B. Microsoft) ausgibt, verschwindend gering `[00:35:14]`.
    
2. **Das "Spotify für Open Source"-Modell:** KI-Anbieter, deren Modelle genau wissen, welchen Code sie ausgeben, sollten einen Teil ihrer Abo-Einnahmen automatisiert und nutzungsbasiert an die Entwickler der jeweiligen Code-Bausteine ausschütten `[00:36:12]`.
    
3. **Kommerzielle Zwischenlizenzen:** Modelle, die den Code für normale Nutzer offenlassen, aber große Konzerne oder die kommerzielle Nutzung verpflichtend monetarisieren `[00:33:08]`.
    

**Fazit des Videos:** Wenn sich an den Strukturen nichts ändert, wird die Open-Source-Welt nicht mit einem großen Knall enden, sondern die digitale Infrastruktur wird durch den schleichenden Verlust ihrer Betreuer langsam, fehlerhafter und unsicherer `[00:39:14]`.