---
{"title":"Transformer","aliases":["Transformermodelle"],"tags":null,"gen_ai_anteil":null,"created":"2026-06-04","updated":null,"status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/0-final-check/transformer/","dgPassFrontmatter":true,"dg-note-properties":{"title":"Transformer","aliases":["Transformermodelle"],"tags":null,"gen_ai_anteil":null,"created":"2026-06-04","updated":null,"status":null}}
---

# Was sind Transformer?

Diese KI-Architektur ist die Grundlage für alle modernen Sprachmodelle - ChatGPT, Claude, Gemini und Co. Mit dem großen Erfolg von ChatGPT begann der eigentliche Boom im Bereich der [LLMs](https://claude.ai/chat/LLMs "Large Language Models"). Transformer sind die Technik dahinter.

## Der Durchbruch: Alles auf einmal statt Wort für Wort

Frühere Modelle - sogenannte RNNs (Recurrent Neural Networks) - lasen Texte wie ein schlechter Dolmetscher: Wort für Wort, in strenger Reihenfolge. Dieses Vorgehen brachte keine befriedigenden Ergebnisse.

Transformer hingegen betrachten den gesamten Satz auf einmal und analysieren, wie jedes Wort mit jedem anderen zusammenhängt.

## Attention: Wer schaut auf wen?

Dafür berechnet der Transformer für jedes Wortpaar im Satz einen Wert: wie stark das eine Wort dem anderen "Aufmerksamkeit schenken" soll. Dieser Mechanismus heißt Attention (Aufmerksamkeit) - weil er nachahmt, wie wir Menschen beim Lesen selektiv aufmerksam sind. Manche Wörter bekommen viel Aufmerksamkeit, andere wenig.

Beispiel: Im Satz "Die Katze saß auf der Matte, weil sie müde war" schenkt "sie" viel Aufmerksamkeit der "Katze" - und wenig der "Matte". Das Modell hat gelernt, dass Katzen müde werden können, Matten aber nicht.

Und hier wird es spannend: Woher weiß das Modell das? Nicht, weil irgendwo gespeichert wäre "Katze gehört zu müde". Das käme bei den unendlich vielen möglichen Wortkombinationen nie hin. Stattdessen trägt jedes Wort eine Art Steckbrief mit Eigenschaften mit sich: "Katze" ist ein Lebewesen, das Zustände haben kann; "müde" ist so ein Zustand; "Matte" ist ein unbelebter Gegenstand. Attention vergleicht diese Steckbriefe - und wo sie zusammenpassen, fließt viel Aufmerksamkeit.

Diese Steckbriefe sind das, was beim Training gelernt wurde. Während des Trainings stellt sich das Netz über seine Gewichte - Millionen von Stellschrauben - nach und nach so ein, dass jedes Wort am Ende sinnvolle Eigenschaften bekommt. Die Gewichte stehen nach dem Training fest. Der Vergleich über Attention dagegen läuft bei jedem neuen Satz frisch ab. Deshalb funktioniert er auch bei Sätzen, die so nie in den Trainingsdaten standen.

## Warum "Transformer"?

Man kann es sich so merken: Der Mechanismus transformiert die Beziehungen zwischen Wörtern in etwas, das wie Verständnis aussieht. Aus statistischen Mustern wird brauchbare Bedeutung.

> [!info] Analogie: Dolmetscher
> 👉 Ein schlechter Dolmetscher übersetzt Wort für Wort, ohne auf den Sinn zu achten.
   👉 Ein guter Dolmetscher versteht den ganzen Satz und „transformiert“ ihn in eine natürliche Übersetzung.