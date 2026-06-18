---
{"title":"Vibecoding","aliases":null,"tags":null,"gen_ai_anteil":["Claude 60%"],"created":"2026-06-17","updated":null,"status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/0-final-check/vibecoding/","dgPassFrontmatter":true,"dg-note-properties":{"title":"Vibecoding","aliases":null,"tags":null,"gen_ai_anteil":["Claude 60%"],"created":"2026-06-17","updated":null,"status":null}}
---

# Vibecoding

> *“Englisch ist die heißeste neue Programmiersprache.”*
> 													*- Andrej Karpathy (2023)*

Vibecoding bezeichnet einen KI-gestützten Programmieransatz, bei dem man das Modell den Code generieren lässt, indem man das gewünschte Ergebnis in Alltagssprache beschreibt. Entscheidungen fallen nach Gefühl und Geschwindigkeit, nicht nach Architektur-Prinzipien.

Der Begriff geht auf [[02 - Künstliche Intelligenz/0 - Final Check/Andrej Karpathy\|Andrej Karpathy]] zurück, der ihn im Februar 2025 in einem beiläufigen Tweet prägte. Er beschrieb eine neue Art zu programmieren, bei der man sich ganz den Vibes (dem Gefühl) hingibt: 

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

Der Code ist oft unstrukturiert und schwer zu pflegen. Was schnell entsteht, übersieht Details, die für langfristige Stabilität und Erweiterbarkeit entscheidend sind.

#
- **Verständnislücke:** Wer die eigene Codebasis nicht durchdringt, baut auf fragilen Fundamenten - mit hohen Wartungskosten als Spätfolge

## Cybersecurity - ein Job mit Zukunft

Vibe-Code genügt im allgemeinen den Ansprüchen an sicheren Code nicht: 
 - Eine Veracode-Untersuchung von 2026 fand, dass rund 45 % des KI-generierten Codes klassische OWASP-Top-10-Schwachstellen einführt - eine Quote, die sich über mehrere Testzyklen kaum verbessert hat. Die Modelle optimieren auf "Feature funktioniert", nicht auf "Feature ist sicher". 
 - Georgia Techs "Vibe Security Radar" zählte allein von Januar bis März 2026 einen Anstieg der direkt KI-zugeschriebenen CVEs (dokumentierte Sicherheitslücken) von 6 auf 35 pro Monat. Reale Folgen: durchgesickerte API-Schlüssel, offene Datenbanken, exponierte persönliche Daten.

 Genau hier entsteht ein Bumerang-Effekt. Je mehr ungeprüfter KI-Code in Produktion geht, desto mehr Arbeit kommt auf Cybersecurity-Spezialistinnen und -Spezialisten zu. Wer Lücken findet und schließt, dürfte auf absehbare Zeit nicht arbeitslos werden.

## Weiterlesen
> Wenn erfahrene Programmiererinnen und Programmierer mit Agenten arbeiten, die Architektur und Qualität aber bewusst selbst verantworten, spricht man heute nicht mehr von Vibecoding, sondern von [[Agentic Engineering\|Agentic Engineering]]


📺 [AI Cognitive Debt: The Crisis Nobody Sees Coming](https://www.youtube.com/watch?v=Tk0hIOAwf6M)

- Die Schnelligkeit mit der auch Nicht-Programmierer oder mittelmäßige Programmierer Code produzieren können hat zu einer Krise der [[02 - Künstliche Intelligenz/3- Veröffentlicht/Open Source vs Proprietär\|Open Source]]-Bewegung geführt. Das zugrunde liegende Problem: Code kann von KI in sekundenschnelle generiert werden; aber er muss mühsam und zeitaufwendig von Menschen mit echtem Verständnis geprüft werden.[[02 - Künstliche Intelligenz/3- Veröffentlicht/Morpheus Video zu KI und OpenSource\|Morpheus Video zu KI und OpenSource]]

