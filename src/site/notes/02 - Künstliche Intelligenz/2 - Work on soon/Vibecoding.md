---
{"title":"Vibecoding","aliases":null,"tags":null,"gen_ai_anteil":["Claude 60%"],"created":"2026-06-17","updated":null,"status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/2-work-on-soon/vibecoding/","dgPassFrontmatter":true,"dg-note-properties":{"title":"Vibecoding","aliases":null,"tags":null,"gen_ai_anteil":["Claude 60%"],"created":"2026-06-17","updated":null,"status":null}}
---

# Vibecoding

> *“Englisch ist die heißeste neue Programmiersprache.”*
> 													*- Andrej Karpathy (2023)*

Vibecoding bezeichnet einen KI-gestützten Programmieransatz, bei dem man das Modell den Code generieren lässt, indem man das gewünschte Ergebnis in Alltagssprache beschreibt. Entscheidungen fallen nach Gefühl und Geschwindigkeit, nicht nach Architektur-Prinzipien.

Der Begriff geht auf [[02 - Künstliche Intelligenz/2 - Work on soon/Andrej Karpathy\|Andrej Karpathy]] zurück, der ihn im Februar 2025 in einem beiläufigen Tweet prägte. Er beschrieb eine neue Art zu programmieren, bei der man sich ganz den Vibes (dem Gefühl) hingibt: 

>*"Give in to the vibes, …, and forget that the code even exists"*.


## Wofür eignet sich Vibecoding?

- Schnelle Prototypen, MVPs (Minimum Viable Products) und Wegwerf-Skripte
- Spielerei, Lernen, Ausprobieren in unbekanntem Terrain
- Niedrige Einstiegshürde - auch für Menschen ohne Programmierkenntnisse

## Karpathys Einordnung - und was daraus wurde

Genau diese Eignung deckte sich mit Karpathys eigener Einschätzung: Im selben Tweet schränkte er ein, vibe-gecodete Ergebnisse seien nicht schlecht für “throwaway weekend projects" - also Wegwerf-Wochenendprojekte mit niedrigem Einsatz. 

Die spätere Lesart "man muss nicht programmieren können und baut damit produktionsreife Software" kam dagegen nicht von ihm, sondern von anderen - ein Missverständnis, das bis heute anhält. 

Befeuert wurde das von einer Startup- und Hype-Welle rund um Plattformen wie Lovable und Bolt, die das Bauen ganzer Anwendungen mit wenig bis gar keinem Code aktiv vermarkteten. Aus dieser Diskrepanz zwischen Anspruch und Praxis entstand ein Großteil der späteren Probleme.

## Die Problematik

Wenn Code unter Zeitdruck entsteht, leidet die Qualität – das gilt für Menschen wie für künstliche Intelligenz gleichermaßen. 

In der IT-Welt gibt es dafür einen etablierten Begriff: **Technical Debt** (Technische Schulden). Er bezeichnet den Mehraufwand, der entsteht, wenn man schnellen, unsauberen oder unstrukturierten Code schreibt, den man später mühsam aufräumen muss. Wer im „Vibe“ programmiert, übersieht schnell Details, die für langfristige Stabilität, Wartbarkeit und Erweiterbarkeit entscheidend sind.

### Cognitive Debt (“Kognitive Schulden”)

Mit dem Aufkommen von KI kommt jedoch ein neues, weitaus gefährlicheren Phänomen hinzu: **Cognitive Debt**. 

Geprägt von der Informatik-Professorin Margaret-Anne Story Anfang 2026, beschreibt der Begriff eine schleichende Wissenserosion. Kognitive Schulden entstehen, wenn KI fehlerfreien, sauberen und funktionierenden Code generiert, aber **das menschliche Team das geteilte Verständnis darüber verliert, wie dieser Code im Detail funktioniert**. Der Code ist nicht schlecht – er ist schlicht unverstanden. 

Das Problem ist unsichtbar, bis das System bricht und die Entwickler wie Archäologen vor ihrer eigenen Software stehen.

(Sehr empfehlenswertes Video dazu ganz unten!)
### Cybersecurity - ein Job mit Zukunft

Vibe-Code genügt im Allgemeinen den Ansprüchen an sicheren Code nicht. KI-Modelle optimieren  nicht auf Sicherheit, sondern auf die statistische Wahrscheinlichkeit des nächsten Wortes. Sie generieren Code, der plausibel wirkt, funktioniert und den Nutzer schnell zufriedenstellt. 

Weil KI-generierter Code optisch oft sauber wirkt, verleitet er zu blindem Vertrauen. Doch die Modelle betrachten Code meist isoliert und übersehen komplexe Sicherheits-Wechselwirkungen im Gesamtsystem. Schlimmer noch: Da sie mit historischem Code trainiert wurden, replizieren sie alte, bekannte Sicherheitslücken in rasantem Tempo – ganz unbemerkt vom Entwickler im „Vibe“.

Je mehr ungeprüfter, rasant generierter KI-Code in Produktion geht, desto größer wird die Angriffsfläche. Kognitive und technische Schulden verwandeln sich in offene Einfallstore. 

Für Cybersecurity-Spezialistinnen und -Spezialisten sind das gute Neuigkeiten: sie dürften auf absehbare Zeit wohl nicht arbeitslos werden.

## 📖 Weiterlesen

> Wenn erfahrene Programmiererinnen und Programmierer mit Agenten arbeiten, die Architektur und Qualität aber bewusst selbst verantworten, spricht man heute nicht mehr von Vibecoding, sondern von [[02 - Künstliche Intelligenz/2 - Work on soon/Agentic Engineering\|Agentic Engineering]]


## 📺 Aus der YouTube Academy

- Das Konzept von “Cognitive Debt” genauer erklärt: [AI Cognitive Debt: The Crisis Nobody Sees Coming](https://www.youtube.com/watch?v=Tk0hIOAwf6M)

- Die Schnelligkeit mit der auch Nicht-Programmierer oder mittelmäßige Programmierer Code produzieren können hat zu einer Krise der Open-Source-Bewegung geführt. Das zugrunde liegende Problem: Code kann von KI in sekundenschnelle generiert werden; aber er muss mühsam und zeitaufwendig von Menschen mit echtem Verständnis geprüft werden 👉 📺 [[02 - Künstliche Intelligenz/3- Veröffentlicht/Morpheus Video zu KI und OpenSource\|Morpheus Video zu KI und OpenSource]]

