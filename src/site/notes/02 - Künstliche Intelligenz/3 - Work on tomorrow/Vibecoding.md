---
{"title":"Vibecoding","aliases":null,"tags":null,"gen_ai_anteil":["Claude 60%"],"created":"2026-06-17","updated":null,"status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/3-work-on-tomorrow/vibecoding/","dgPassFrontmatter":true,"dg-note-properties":{"title":"Vibecoding","aliases":null,"tags":null,"gen_ai_anteil":["Claude 60%"],"created":"2026-06-17","updated":null,"status":null}}
---


# Vibecoding

> [!quote] Englisch ist die heißeste neue Programmiersprache.
> _- Andrej Karpathy (2023)_

Vibecoding bezeichnet einen KI-gestützten Programmieransatz, bei dem man das Modell den Code generieren lässt, indem man das gewünschte Ergebnis in Alltagssprache beschreibt. Entscheidungen fallen nach Gefühl und Geschwindigkeit, nicht nach Architektur-Prinzipien.

Der Begriff geht auf [[02 - Künstliche Intelligenz/3 - Work on tomorrow/Andrej Karpathy\|Andrej Karpathy]] zurück, der ihn im Februar 2025 mit einem beiläufigen Tweet prägte. Er beschrieb eine neue Art zu programmieren, bei der man sich ganz den Vibes (dem Gefühl) hingibt:

> *Give in to the vibes, …, and forget that the code even exists.*[^quelle]

## Wofür eignet sich Vibecoding?

- Schnelle Prototypen und MVPs (Minimum Viable Products)
- Spielerei, Lernen und Ausprobieren – auch ohne Programmierkenntnisse

Das sah Karpathy übrigens genauso: Im selben Tweet merkte er an, vibe-gecodete Ergebnisse seien ganz passabel für „throwaway weekend projects“ – also Wegwerf-Wochenendprojekte mit niedrigem Einsatz.

Die spätere Lesart „man muss nicht programmieren können und baut damit produktionsreife Software“ kam von anderen – ein Missverständnis, das bis heute anhält.

Befeuert wurde das von einer Startup- und Hype-Welle rund um Plattformen wie Lovable und Bolt, die das Bauen ganzer Anwendungen ohne Programmierkenntnisse aktiv vermarkteten. Aus dieser Diskrepanz zwischen Versprechen und Realität entstand ein Großteil der späteren Probleme.

## Die Problematik

Wenn Code unter Zeitdruck entsteht, leidet die Qualität – egal, ob ein Mensch ihn schreibt oder eine KI.

In der IT-Welt gibt es dafür einen etablierten Begriff: **Technical Debt** (Technische Schulden). Er bezeichnet den Mehraufwand, der entsteht, wenn man schnellen, unsauberen oder unstrukturierten Code schreibt, den man später mühsam aufräumen muss. Wer im „Vibe“ programmiert, übersieht schnell Details, die für langfristige Stabilität, Wartbarkeit und Erweiterbarkeit entscheidend sind.

### Cognitive Debt („Kognitive Schulden“)

Mit dem Aufkommen von KI tritt jedoch ein neues, weitaus gefährlicheres Phänomen hinzu: **Cognitive Debt**.

Der Begriff wurde Anfang 2026 durch die Informatik-Professorin Margaret-Anne Storey bekannt. In der Softwareentwicklung beschreibt er eine schleichende Wissenserosion: Kognitive Schulden entstehen, wenn **das menschliche Team das Verständnis darüber verliert, wie der Code im Detail funktioniert** – und zwar selbst dann, wenn die KI sauberen, funktionierenden Code generiert hat.

Das Problem ist unsichtbar, bis das System bricht und die Entwickler wie Archäologen vor ihrer eigenen Software stehen.

### Cybersecurity – ein Job mit Zukunft

Vibe-Code genügt im Allgemeinen den Ansprüchen an sicheren Code nicht. KI-Modelle lernen in der ersten [[02 - Künstliche Intelligenz/4 - very soon/Training von LLMs\|Trainingsphase]], das wahrscheinlichste nächste Wort vorherzusagen. In einer späteren Phase werden sie dafür belohnt, dass ihr Code läuft und Tests besteht. Ob er auch sicher ist, spielt dabei eine untergeordnete Rolle. Das Ergebnis ist Code, der plausibel wirkt und den Nutzer zufriedenstellt – es funktioniert ja zunächst einmal alles.

Weil KI-generierter Code optisch oft sauber wirkt, verleitet er zu blindem Vertrauen. Doch die Modelle betrachten Code meist isoliert und übersehen komplexe Sicherheits-Wechselwirkungen im Gesamtsystem. Schlimmer noch: Da sie mit historischem Code trainiert wurden, replizieren sie alte, bekannte Sicherheitslücken in rasantem Tempo – ganz unbemerkt vom Entwickler im „Vibe“.

Je mehr ungeprüfter, rasch generierter KI-Code in Produktion geht, desto größer wird die Angriffsfläche. Kognitive und technische Schulden werden zu offenen Einfallstoren.

Für Cybersecurity-Spezialisten sind das gute Neuigkeiten: Sie dürften auf absehbare Zeit nicht arbeitslos werden.

## 📖 Weiterlesen

- Wenn erfahrene Programmierer mit KI-Agenten arbeiten, dabei aber Architektur und Qualität bewusst selbst verantworten, spricht man heute nicht mehr von Vibecoding, sondern von [[02 - Künstliche Intelligenz/Garten erkunden/Grundlagen/Agentic Engineering\|Agentic Engineering]].
- Jeder kann jetzt Webdesign? Nein! Meine Perspektive als Webdesignerin zu vibe-gecodeten Websites: [[02 - Künstliche Intelligenz/Garten erkunden/Verschiedenes/Warum KI (noch) keine guten Websites baut\|Warum KI (noch) keine guten Websites baut]]
- Laien und mittelmäßige Programmierer können heute in Sekundenschnelle Code produzieren. Prüfen müssen ihn aber Menschen mit echtem Verständnis – und das ist mühsam. Das hat zu einer Krise der Open-Source-Bewegung geführt. Mehr dazu im Artikel zu [[02 - Künstliche Intelligenz/5 - soon (veröffentlicht)/Morpheus Video zu KI und OpenSource\|Morpheus Video zu KI und OpenSource]]

## 📺 Aus der YouTube Academy

- [AI Cognitive Debt: The Crisis Nobody Sees Coming](https://www.youtube.com/watch?v=Tk0hIOAwf6M) erklärt das Konzept von „Cognitive Debt“ im Detail. Sehr empfehlenswert.
- Man könnte meinen, ich wäre gegen Vibecoding. Bin ich nicht. Aber – man sollte halt wissen, was man tut. Dieser kompakte Powerkurs liefert die Grundlagen und macht richtig Lust aufs Ausprobieren 😋: [Vibe Coding Fundamentals In 33 minutes](https://www.youtube.com/watch?v=iLCDSY2XX7E) 

[^quelle]: Andrej Karpathy auf X, 2. Februar 2025: [x.com/karpathy/status/1886192184808149383](https://x.com/karpathy/status/1886192184808149383)