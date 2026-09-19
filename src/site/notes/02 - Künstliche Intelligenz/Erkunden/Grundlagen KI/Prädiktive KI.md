---
{"title":"Prädiktive KI","aliases":["prädiktive KI"],"tags":null,"gen_ai_anteil":["Claude 60%"],"created":"2026-09-11","updated":"2026-09-18","status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/erkunden/grundlagen-ki/praediktive-ki/","dgPassFrontmatter":true,"dg-note-properties":{"title":"Prädiktive KI","aliases":["prädiktive KI"],"tags":null,"gen_ai_anteil":["Claude 60%"],"created":"2026-09-11","updated":"2026-09-18","status":null}}
---

# Prädiktive KI

Es handelt sich um [[02 - Künstliche Intelligenz/Erkunden/Grundlagen KI/Statistische KI\|statistische KI-Systeme]], die aus vorhandenen Daten Muster lernen, um Aussagen über Zukünftiges oder Unbekanntes zu treffen. Das Ergebnis ist eine Einschätzung, etwa eine Kategorie, ein Wert oder ein Risiko, aber kein neuer Inhalt.

## Begriffsklärung

**Der Begriff ist ein Retronym:** Er entstand erst, nachdem [[02 - Künstliche Intelligenz/Erkunden/Grundlagen KI/Generative KI\|generative KI]] populär wurde und man ein Wort für diese „andere KI“ brauchte. „Prädiktive KI“ war vor 2022 kaum gebräuchlich; man sagte einfach [[02 - Künstliche Intelligenz/5 - soon (veröffentlicht)/Machine Learning (ML)\|Machine Learning]], Klassifikation, Regression. Etabliert war allenfalls „Predictive Analytics“ als Sammelbegriff für datengestützte Prognosen in Unternehmen.

> [!info] Wortherkunft
>
> lat. _praedicere_ = „vorhersagen“ (_prae_ = „vor“, _dicere_ = „sagen“)
>
> Ich halte den Begriff für schlecht gewählt, denn „Prediction“ meint im maschinellen Lernen nicht zwingend die Zukunft, sondern das Schätzen eines unbekannten Werts. Das Modell kennt die richtige Antwort nicht, es leitet sie aus Mustern ab, die es gelernt hat. Manchmal liegt dieser Wert in der Zukunft (Absatzprognose), oft aber nicht (Bilderkennung).

## Abgrenzung zu generativer KI

- **Prädiktive KI** schätzt, bewertet und ordnet ein: „Zeigt das Bild einen Hund oder eine Katze?“
- **Generative KI** erzeugt neue Inhalte wie Texte, Bilder oder Code: „Erstelle ein Bild von einer Katze.“

> [!info] Definition über den Zweck
> Auch [[02 - Künstliche Intelligenz/5 - soon (veröffentlicht)/LLMs (Large Language Models)\|LLMs (Large Language Models)]] sind technisch gesehen Vorhersagemaschinen: Sie berechnen, welches [[Token\|Token]] am wahrscheinlichsten als Nächstes folgt. Die Grenze verläuft also weniger über die Technik als über den Zweck.

Anwendungen wie [[02 - Künstliche Intelligenz/Erkunden/Grundlagen KI/KI-Sprachtechnologie#STT gibt es in zwei Varianten\|STTs]] (eine KI-Sprachtechnologie) können je nach Umsetzung in den prädiktiven oder in den generativen Bereich fallen.

👉 Siehe dazu auch [[02 - Künstliche Intelligenz/Erkunden/Grundlagen KI/Generative KI#Begriffliche Klärung\|GenAI – Begriffliche Klärung]]

## Typische Anwendungen

- **Spamfilter:** schätzt, wie wahrscheinlich eine Mail Spam ist
- **Betrugserkennung:** sperrt die Bankkarte, wenn eine Zahlung nicht zum üblichen Muster passt
- **Streaming-Empfehlungen:** „Das könnte dir auch gefallen“
- **[[02 - Künstliche Intelligenz/Erkunden/Grundlagen KI/KI-Sprachtechnologie\|KI-Sprachtechnologie]]**: teils prädiktiv, teils generativ
- **Wortvorschläge** auf der Handytastatur: technisch ein winziges Sprachmodell, jedoch ohne generativen Zweck
