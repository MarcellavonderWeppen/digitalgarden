---
{"title":"Statistische KI – So funktioniert das Training","aliases":null,"tags":null,"gen_ai_anteil":null,"created":"2026-09-28","updated":null,"status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/3-work-on-tomorrow/statistische-ki-so-funktioniert-das-training/","dgPassFrontmatter":true,"dg-note-properties":{"title":"Statistische KI – So funktioniert das Training","aliases":null,"tags":null,"gen_ai_anteil":null,"created":"2026-09-28","updated":null,"status":null}}
---

# Statistische KI – So funktioniert das Training

Klassische Software wird programmiert: Ein Mensch schreibt Regeln, der Computer führt sie aus. [[02 - Künstliche Intelligenz/Garten erkunden/Grundlagen/Statistische KI\|Moderne KI]]wird dagegen **trainiert**: Man gibt ihr Daten, und sie leitet die Regeln selbst daraus ab.

## Die Grundidee

Ein KI-Modell hat eine riesige Zahl an Stellschrauben, die sogenannten **Parameter**. Beim Training macht das Modell eine Vorhersage und bekommt eine Rückmeldung, wie gut sie war. Dann werden die Stellschrauben so nachjustiert, dass es beim nächsten Mal etwas besser liegt.

Bei neuronalen Netzen, der Grundlage heutiger KI, geschieht das in winzigen Schritten, unzählige Male wiederholt. Am Ende steckt das „Wissen“ des Modells in den Werten seiner Parameter.

## Drei Arten zu lernen

Je nachdem, woher die Rückmeldung kommt, unterscheidet man drei grundlegende Lernarten:

**Überwachtes Lernen** (Supervised Learning): Das Modell lernt aus Beispielen mit richtiger Lösung. Ein Spamfilter sieht Tausende E-Mails, die Menschen als „Spam“ oder „kein Spam“ markiert haben, und lernt, die beiden zu unterscheiden.

**Unüberwachtes Lernen** (Unsupervised Learning): Es gibt keine vorgegebenen Lösungen. Das Modell sucht selbst nach Mustern, etwa um Kunden mit ähnlichem Kaufverhalten in Gruppen einzuteilen.

Ein wichtiger Sonderfall ist das **selbstüberwachte Lernen** (Self-Supervised Learning): Das Modell erzeugt sich die Lösungen aus den Daten selbst. Man verdeckt zum Beispiel das nächste Wort eines Satzes und lässt es raten. Der Vorteil: Niemand muss die Daten vorher beschriften. Deshalb lassen sich damit riesige Textmengen nutzen.

**Bestärkendes Lernen** (Reinforcement Learning): Das Modell probiert etwas aus und bekommt dafür Belohnung oder Abzug, ohne dass es eine Musterlösung gibt. So lernte AlphaGo Zero, Go auf Weltklasseniveau zu spielen – allein durch Partien gegen sich selbst.

## Große Modelle: die Lernarten hintereinander

Klassische KI-Modelle nutzen meist nur eine dieser Lernarten und werden für genau eine Aufgabe trainiert. Große Sprachmodelle, wie sie hinter ChatGPT, Claude oder Gemini stecken, durchlaufen dagegen mehrere Phasen. Jede entspricht einer Lernart:

1. **Pretraining** (selbstüberwacht): Das Modell lernt an gewaltigen Textmengen, das nächste Wort (genauer: [[Token\|Token]]) vorherzusagen. Dabei eignet es sich Sprache, Faktenwissen und Zusammenhänge an. Heraus kommt ein Basismodell, das Texte fortsetzen kann, aber noch kein hilfreicher Gesprächspartner ist.
2. **Fine-Tuning** (überwacht): Anhand ausgewählter Beispiele aus Frage und guter Antwort lernt das Modell, sich wie ein Assistent zu verhalten.
3. **Belohnungsphase** (bestärkend): Das Modell erzeugt Antworten, die bewertet werden – von Menschen (RLHF, Reinforcement Learning from Human Feedback) oder automatisch, etwa danach, ob Code läuft oder eine Rechnung stimmt. Gut bewertetes Verhalten wird verstärkt.

Die Phasen 2 und 3 fasst man oft als **Post-Training** zusammen. In der Praxis ist die Abfolge komplexer: Anbieter kombinieren und wiederholen Phasen. Das Grundmuster bleibt aber dasselbe.

Pretraining und Fine-Tuning gibt es übrigens nicht nur bei Sprachmodellen, sondern auch bei großen Bild- oder Audiomodellen; nur die Vortrainingsaufgabe ist eine andere. Die Belohnungsphase spielt vor allem bei Chatbots und Coding-Modellen eine große Rolle.

## Was daraus folgt

Ein Modell wird auf das optimiert, was im Training gemessen wird. Zählt in der Belohnungsphase, ob Code läuft, lernt es, lauffähigen Code zu schreiben. Ob dieser Code auch sicher ist, steht auf einem anderen Blatt.
