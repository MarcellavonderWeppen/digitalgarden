---
{"title":"KI-Sprachtechnologie","aliases":null,"tags":null,"gen_ai_anteil":null,"created":"2026-09-03","updated":"2026-09-06","status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/1-work-on-now/ki-sprachtechnologie/","dgPassFrontmatter":true,"dg-note-properties":{"title":"KI-Sprachtechnologie","aliases":null,"tags":null,"gen_ai_anteil":null,"created":"2026-09-03","updated":"2026-09-06","status":null}}
---


# KI-Sprachtechnologie

KI-Sprachtechnologie ist der Oberbegriff für alle Verfahren, mit denen Maschinen gesprochene Sprache verarbeiten, verstehen oder erzeugen. Sie ist die Brücke zwischen der Stimme des Menschen und den textbasierten Systemen, mit denen Computer intern arbeiten.

## *Speech* vs. *language*

Das Wort „Sprache“ ist dabei doppeldeutig. Das Englische unterscheidet zwischen _language_ (Sprache als System: Text, Grammatik, Bedeutung) und _speech_ (Sprache als Gesprochenes: Stimme und Audio). „Sprachtechnologie“ kann im Deutschen beides meinen. Dieser Artikel behandelt den engen Sinn, also Speech AI; die Verarbeitung von geschriebenem Text durch große Sprachmodelle ist ein eigenes Feld.

## Die wichtigsten Teilgebiete

**Speech-to-Text (STT)**, auch Automatic Speech Recognition (ASR) genannt, wandelt gesprochene Sprache in geschriebenen Text um. Es ist das bekannteste Teilgebiet – Diktierfunktionen und Meeting-Transkriptionen beruhen darauf. Ein verbreitetes Modell ist Whisper von OpenAI.

**Text-to-Speech (TTS)** ist der umgekehrte Weg: Text wird in natürlich klingende Sprache umgesetzt. Moderne Sprachsynthese ist kaum noch von menschlichen Sprechern zu unterscheiden.

**Voice Cloning** bildet die Stimme einer konkreten Person nach, oft schon aus wenigen Sekunden Aufnahme. Wer seine Stimme durch eine Krankheit verliert, kann so weiterhin mit der eigenen Stimme sprechen. Gleichzeitig ist dieselbe Technik aber auch Grundlage für Audio-Deepfakes.

**Sprechererkennung** beantwortet die Frage, wer spricht – zum Beispiel zur Authentifizierung per Stimme oder um in einer Aufnahme mehrere Personen auseinanderzuhalten.

**Emotions- und Tonanalyse** wertet aus, wie etwas gesagt wird: Stimmung, Betonung, Dringlichkeit.

## KI-Sprachtechnologie ist statistische KI

Alle fünf Teilgebiete gehören der **statistischen KI** an, aber in zwei verschiedenen Bereichen: Prädiktive und generative KI.

![Statistische KI Diagramm.png](/img/user/Statistische%20KI%20Diagramm.png)

| Teilgebiet               | Zuhause im Baum                         |
| ------------------------ | --------------------------------------- |
| Text-to-Speech (TTS)     | GenAI → Audio                           |
| Voice Cloning            | GenAI → Audio                           |
| Sprechererkennung        | Prädiktive KI → Klassifikation          |
| Emotions- und Tonanalyse | Prädiktive KI → Klassifikation          |
| Speech-to-Text (STT)     | teils Prädiktive KI, teils GenAI → Text |

Die Faustregel dahinter: Kommt etwas _Neues_ heraus (eine Stimme), ist es GenAI. Kommt eine _Einordnung_ heraus (wer, welche Stimmung), ist es prädiktiv.

STT ist der Mischling, weil beides zutrifft: Es ordnet ein, was gesagt wurde, aber das Ergebnis ist erzeugter Text. Modelle wie Whisper sind technisch genauso gebaut wie Übersetzer, also generativ. 

## Die wichtigsten Anwendungen

Die Teilgebiete sind Bausteine. Was man im Alltag als Produkt erlebt, kombiniert meist mehrere davon.

### Diktieren statt Tippen

Man spricht, der Computer schreibt, in jedes beliebige Textfeld, ob E-Mail, Chat oder Dokument. Moderne Tools glätten dabei gleich den Text, entfernen Füllwörter und setzen Satzzeichen. Im Kern STT; neuere Tools ergänzen ein Sprachmodell zur Nachbearbeitung.

**Beispiele:** Wispr Flow, Apples Diktierfunktion, Dragon

 👉 Mehr zu [[02 - Künstliche Intelligenz/Speech-to-Text (STT)\|Speech-to-Text (STT)]]

### Meeting-Assistenten

Ein Programm hört bei Videokonferenzen mit, schreibt alles mit, ordnet die Beiträge den Teilnehmern zu und erstellt danach eine Zusammenfassung mit den vereinbarten Aufgaben. Kombiniert STT, Sprecherzuordnung und ein Sprachmodell.

**Beispiele:** Otter, Fireflies, Microsoft Teams Copilot

👉 Mehr zu [[02 - Künstliche Intelligenz/2 - Work on soon/Meeting Intelligence\|Meeting Intelligence]]

### Sprachassistenten und Voice Agents

Man spricht mit dem System wie mit einem Menschen und bekommt eine gesprochene Antwort, sei es auf dem Handy, im Sprachmodus eines Chatbots oder bei einem Telefonbot im Kundenservice. Heute meist eine Kette aus STT, Sprachmodell und TTS.

**Beispiele:** Siri, Alexa

### Übersetzen und Synchronisieren

Gesprochene Sprache wird in Echtzeit gedolmetscht oder ein Video nachträglich in eine andere Sprache übertragen, wobei die Originalstimme erhalten bleiben kann. Kombiniert STT, Übersetzung, TTS und oft Voice Cloning.

**Beispiele:** Google Translate, ElevenLabs, HeyGen

### Barrierefreiheit

Screenreader lesen Menschen mit eingeschränktem Sehvermögen den Bildschirm vor (TTS), Live-Transkription macht Gespräche für Hörgeschädigte lesbar (STT), und wer seine Stimme durch Krankheit verliert, kann sie vorher aufnehmen und weiter nutzen (Voice Cloning).

**Beispiele:** Apple Personal Voice, Live-Untertitel in Teams und Zoom

### Stimme als Passwort

Beim Telefonbanking erkennt das System den Anrufer an der Stimme. Reine Sprechererkennung, die allerdings durch Voice Cloning zunehmend unter Druck gerät und als alleiniges Sicherheitsmerkmal nicht mehr ausreicht.

## Was bringt die Zukunft?

**Sprache ohne Umweg über Text.** Neue Modelle verarbeiten Audio direkt, ohne es erst in Text zu verwandeln. Das macht Sprachassistenten schneller und erhält, was bei einer Transkription verloren geht: Tonfall, Zögern, Ironie. Die bisherige Kette aus STT, Sprachmodell und TTS beginnt sich damit aufzulösen. Diese Zukunft hat bereits begonnen: Erste Sprachassistenten arbeiten heute schon so.

**Sprechen mit jedem, in jeder Sprache.** Ein Ohrhörer, der ein Gespräch in Echtzeit dolmetscht, und zwar mit der eigenen Stimme des Gegenübers, nicht mit einer Computerstimme. Die Bausteine dafür existieren alle schon, und erste Produkte übersetzen Telefonate bereits mit der Originalstimme. Was noch fehlt, ist die Zuverlässigkeit im Alltag.

**Stimme statt Benutzeroberfläche.** Wenn Maschinen Sprache so gut verstehen wie Menschen, braucht vieles keinen Bildschirm und keine Tastatur mehr. Ein Assistent, der Termine vereinbart, für einen anruft und Ergebnisse mündlich berichtet, ist technisch schon möglich; ob wir das wollen, ist eine andere Frage.

**Die Kehrseite wächst mit:** Je perfekter Stimmen nachgebildet werden können, desto wichtiger wird es, echte von gefälschten zu unterscheiden.