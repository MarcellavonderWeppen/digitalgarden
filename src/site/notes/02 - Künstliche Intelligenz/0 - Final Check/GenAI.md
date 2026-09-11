---
{"title":"GenAI","aliases":["Generative KI"],"tags":null,"gen_ai_anteil":["Mistral 80%"],"created":"2026-06-03","updated":"2026-06-04","status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/0-final-check/gen-ai/","dgPassFrontmatter":true,"dg-note-properties":{"title":"GenAI","aliases":["Generative KI"],"tags":null,"gen_ai_anteil":["Mistral 80%"],"created":"2026-06-03","updated":"2026-06-04","status":null}}
---

# Was ist Generative KI?

Generative KI (GenAI) ist eine Form der [[02 - Künstliche Intelligenz/0 - Final Check/Statistische KI\|statistischen KI]]. Sie basiert auf komplexen Algorithmen, die große Datenmengen analysieren, um Muster zu erkennen und daraus neue Inhalte zu erzeugen – sei es Text, Bilder, Musik oder sogar Videos. 

Im Gegensatz zu [[02 - Künstliche Intelligenz/3 - Work on tomorrow/Klassische KI\|klassischen KI-Systemen]], die auf festen Regeln basieren, kann GenAI kreativ sein: Sie erzeugt neue, gelegentlich sogar originelle Inhalte – basierend auf den Mustern, die sie aus den Trainingsdaten gelernt hat.

Die Technologie hinter GenAI sind meist neuronale Netze, insbesondere [Transformermodelle](Transformer), die durch [[02 - Künstliche Intelligenz/5 - soon (veröffentlicht)/Machine Learning (ML)\|maschinelles Lernen]] trainiert werden. Die bekannteste Ausprägung sind [[02 - Künstliche Intelligenz/5 - soon (veröffentlicht)/LLMs (Large Language Models)\|große Sprachmodelle (LLMs)]], welche hinter Chatbots wie [[02 - Künstliche Intelligenz/5 - soon (veröffentlicht)/ChatGPT\|ChatGPT]] stehen. Diese Transformer werden mit riesigen Textmengen trainiert und erzeugen Sprache Wort für Wort.  

Bei Bild, Video und Ton kommt ein zusätzliches Verfahren dazu: [[02 - Künstliche Intelligenz/4 - very soon/Diffusion-Modelle\|Diffusion]].

## Begriffliche Klärung

„Generativ“ hat zwei Lesarten, die sich nicht ganz decken.

Im Alltagsverständnis ist generativ, was einen neuen Inhalt hervorbringt: ChatGPT schreibt einen Text, den es vorher nicht gab, Midjourney malt ein Bild, das niemand vorgegeben hat.

Im technischen Sinn ist generativ, was neue Daten erzeugt, statt vorhandene nur zu erkennen oder einzuordnen. Ob der Inhalt dabei neu ist, spielt keine Rolle. Danach ist auch Voice Cloning generativ: Gesagt wird nur, was man vorgibt, aber die Stimme dazu wird künstlich erzeugt. 
## Bekannte Beispiele

- Chatbots wie ChatGPT 
- Bildgeneratoren wie Midjourney
- Videogeneratoren wie Google Veo
- Musiktools wie Suno

![genai.png](/img/user/02%20-%20K%C3%BCnstliche%20Intelligenz/1%20-%20Work%20on%20now/Bilder/genai.png)

## Potenzial und Problematik

Diese Systeme haben das Potenzial, Arbeitsprozesse zu beschleunigen, kreative Arbeit zu unterstützen und Dinge zu ermöglichen, die bislang an fehlenden finanziellen Mitteln gescheitert sind: beispielsweise individualisiertes Lernmaterial, wie es sonst nur Privatunterricht bietet, oder Übersetzungen in Sprachen, für die sich das nie gelohnt hat.

Allerdings hat GenAI einen hohen Preis, der oft übersehen wird: Weltweit werden  Rechenzentren aus dem Boden gestampft, welche enorme Mengen an Strom, Wasser und Landflächen verschlingen, oft [[02 - Künstliche Intelligenz/4 - very soon/über die Köpfe der Menschen vor Ort hinweg\|über die Köpfe der Menschen vor Ort hinweg]]. Dazu kommen ungelöste ethische Fragen wie Urheberrecht, Datenschutz und Deepfakes.

 📖 Weiterlesen: [[02 - Künstliche Intelligenz/5 - soon (veröffentlicht)/Kritik an GenAI\|Kritik an GenAI]]
## Es geht auch anders

Aus meiner Sicht ist das Problem nicht die Technologie an sich, sondern die Logik  profitmaximierender Konzerne, welche unkontrolliertes Wachstum über Menschen und die Erhaltung unserer Lebensgrundlagen stellt. 

Bereits heute gibt es Unternehmen, die andere Prioritäten setzten und Alternativen aufzeigen:

- Cloudanbieter wie [Hetzner](https://www.hetzner.com/de/unternehmen/nachhaltigkeit/) setzen auf erneuerbare Energien, der Schweizer Anbieter [[02 - Künstliche Intelligenz/5 - soon (veröffentlicht)/Infomaniak\|Infomaniak]] beheizt mit der Abwärme seines Genfer Rechenzentrums sogar tausende Haushalte
- [[02 - Künstliche Intelligenz/4 - very soon/DeepSeek\|DeepSeek]] hat sein [offenes](Open Source vs Proprietär) Modell V3 mit einem Bruchteil der Rechenleistung trainiert, die üblicherweise für das Training eines LLMs verwendet wird
- Intelligentere Architekturen und Verfahren wie Mixture of Experts (siehe [[Mistral\|Mistral]] oder DeepSeek) arbeiten wesentlich effizienter
- [[SLMs (kleine Sprachmodelle)\|SLMs (kleine Sprachmodelle)]] wie Phi oder Gemma stellen das Narrativ „größer ist besser“ in Frage
- Dienste wie Lumo von [[02 - Künstliche Intelligenz/4 - very soon/Proton\|Proton]] betreiben offene Modelle auf eigenen Servern in Europa und setzen auf Datenschutz statt Datensammeln


