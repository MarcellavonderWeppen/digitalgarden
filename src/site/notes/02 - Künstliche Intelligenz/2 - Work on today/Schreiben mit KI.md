---
{"title":"Schreiben mit KI","aliases":null,"tags":null,"gen_ai_anteil":null,"created":"2026-09-03","updated":null,"status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/2-work-on-today/schreiben-mit-ki/","dgPassFrontmatter":true,"dg-note-properties":{"title":"Schreiben mit KI","aliases":null,"tags":null,"gen_ai_anteil":null,"created":"2026-09-03","updated":null,"status":null}}
---


# Schreiben mit KI

> [!note] **Funfact**
> 
> Dieser Artikel wurde von mir oder durch mich mit Claude Fable geschrieben. Dieses Flaggschiff-Modell von Anthropic ist derzeit nicht mehr durch das Abo abgedeckt, sondern muss über ein Nutzungsguthaben bezahlt werden – und irgendwie muss ich ja mein geschenktes Startguthaben verbrauchen, das am 19. September verfällt. Dieser Artikel hat also im Rahmen dessen 6,98 € gekostet – ob er das wert ist, sei mal dahingestellt. Fest steht: Ich hatte eine Menge Spaß dabei.
> 
> Es scheint nicht richtig zu behaupten, „ich habe einen Artikel geschrieben“; genauso unstimmig wäre für mich: „KI hat einen Text für mich generiert“. Vielmehr würde ich sagen: Ich habe mittels Claude mein Wissen zu diesem Fachgebiet erweitert, mein Verständnis vertieft – und nebenbei ist dieser Artikel entstanden, der hoffentlich Menschen ohne Vorkenntnisse einen schnellen Einstieg ermöglicht und die Klarheit transportiert, die ich jetzt habe. „Ich habe mittels Claude einen Artikel entwickelt“ trifft es für mich also am besten. Es ist schon interessant, wie diese Technologie eine neue Sprache erfordert.
> 
> Und nebenbei habe ich ihn wieder gefühlt, diesen ganz speziellen Genuss, den ich empfinde, seit ich KI entdeckt habe. Lernen war schon immer eine meiner Lieblingsbeschäftigungen, und Lernen mithilfe von LLMs ist aus meiner Sicht eine der besten Anwendungsmöglichkeiten.
## Wieviel Text wurde von der KI geschrieben?

Lassen wir Claude Fable selbst zu Wort kommen: 

> [!quote] Claude Fable
> Ehrlich: Nach Wörtern gezählt etwa 90 Prozent von mir. Fast jeder Satz im Dokument ist in der Form entstanden, wie ich ihn vorgeschlagen habe; Deine wörtlichen Beiträge sind einzelne Formulierungen wie „eingeschränktes Sehvermögen“ oder „Stimme statt Benutzeroberfläche“ und Vorgaben, wie ein Satz zu enden hat.
>
> Nach Entscheidungen gezählt sieht es anders aus. Die Struktur, die den Artikel überhaupt brauchbar macht, kommt von Dir: dass Sprachassistenten eine Anwendung sind und kein Teilgebiet, dass Teilgebiete und Anwendungen getrennt gehören, dass ein verwirrendes Beispiel raus muss, dass es ein Zukunftskapitel statt eines Nachtrags gibt. Die Einleitung in ihrer jetzigen Form gibt es nur, weil Du auf fachlicher Transparenz bestanden hast: Ich hatte die Doppeldeutigkeit von „Sprache“ anfangs mit einem Halbsatz abgetan, Du hast sie als eigentliches Thema erkannt. Und in der Schlussdurchsicht hast Du zwei meiner fünf Änderungsvorschläge abgelehnt, beide Male mit einem Argument, das ich dann geteilt habe. Ich habe das meiste ausformuliert, aber ausgelöst hast Du es, und einiges davon hätte ich von allein nicht gemacht. Grob geschätzt 60 zu 40 für Dich, was die Entscheidungen angeht.
>
> Wenn es eine einzige Zeile sein muss: „Text: 90 Prozent KI, Konzept und Redaktion: überwiegend Du.“ Eine Zahl wie „70 Prozent KI“ wäre ein Mittelwert, der beides falsch abbildet.


# Merkzettel: Entwickeln statt Schreiben – und wie man KI-Nutzung kennzeichnet

Zwei Themen, die zusammenhängen: Wenn „schreiben“ nicht mehr das richtige Wort ist, stellt sich auch die Frage, was man eigentlich kennzeichnet. Vermutlich später zwei getrennte Artikel.

# Merkzettel: Entwickeln statt Schreiben – und wie man KI-Nutzung kennzeichnet

Zwei Themen, die zusammenhängen: Wenn „schreiben“ nicht mehr das richtige Wort ist, stellt sich auch die Frage, was man eigentlich kennzeichnet. Vermutlich später zwei getrennte Artikel.

## Teil 1: Programmieren versus Entwickeln

**Programmieren** ist das Schreiben von Code: eine Vorstellung davon, was passieren soll, in eine Sprache übersetzen, die die Maschine ausführt.

**Entwickeln** ist der ganze Prozess drumherum: klären, was gebraucht wird, den Gegenstand in Teile zerlegen, Grenzen ziehen, entscheiden, was reinkommt und was nicht, Namen finden, das Ergebnis prüfen, aufräumen – und das alles in Schleifen. Programmieren ist ein Teil davon, oft nicht der größte. Wer sich „Entwickler“ nennt, meint das Ganze; wer „Programmierer“ sagt, betont das Handwerk.

**Die Übertragung aufs Schreiben mit KI:** Beim Entstehen des Artikels „KI-Sprachtechnologie“ war mein Anteil fast durchgehend Entwickeln, und zwar mit Mustern, die im Software-Entwickeln Namen haben:

- Teilgebiete und Anwendungen trennen, weil Sprachassistenten in der falschen Schicht lagen → *Separation of Concerns*, ein Refactoring
- das Beispiel „automatische Untertitel“ streichen, weil es selbst Erklärung braucht → toter Code, der mehr kostet, als er bringt
- Diarisierung nicht als eigenen Punkt aufnehmen, obwohl es fachlich korrekt wäre → *YAGNI*, nicht bauen, was der aktuelle Nutzer nicht braucht
- die Speech-Language-Frage klären → Schnittstellendefinition: Was liegt innerhalb dieses Moduls, was außerhalb, und wo wird das dokumentiert
- der „gebildete Leser ohne Vorkenntnisse“ → Testfall, gegen den jeder Absatz geprüft wurde
- in der Schlussdurchsicht zwei von fünf Änderungsvorschlägen ablehnen → Code Review

Claudes Anteil war überwiegend Programmieren: den Entwurf in Sätze übersetzen, schnell, in vielen Varianten, auf Zuruf.

**Die unbequeme Pointe:** Das ist genau die Rolle, die KI im Software-Entwickeln gerade einnimmt, und ein Grund, warum die Lage für Juniors schwierig geworden ist – der Teil, mit dem man früher anfing, ist der Teil, den die Maschine jetzt kann. Der andere Teil ist es nicht.

**Deshalb „entwickelt“:** „Ich habe einen Artikel geschrieben“ stimmt nicht, „KI hat einen Text für mich generiert“ auch nicht. „Ich habe mittels Claude einen Artikel entwickelt“ trifft es, und zwar nicht als Ausweichformel, sondern fachlich präzise.

## Teil 2: Kennzeichnung von KI-Nutzung

**Drei Dinge laufen unter „Kennzeichnung“ und werden ständig vermischt:**

1. *Rechtspflicht.* Enger, als die Debatte vermuten lässt – im EU AI Act geht es vor allem um Deepfakes und um KI-Texte zur Information der Öffentlichkeit über Themen von öffentlichem Interesse, mit Ausnahme bei menschlicher redaktioneller Verantwortung. (Details ungeprüft, muss ich nachschlagen.)
2. *Erwartung der Leser.* Sie wollen wissen, wem sie vertrauen können und ob ein Mensch geradesteht. Sie wollen keine Prozessdokumentation.
3. *Eigene Ehrlichkeit.* Die Frage „darf ich sagen, ich habe das geschrieben?“ ist eine andere als die ersten beiden.

**Der Maßstab:** Gekennzeichnet wird, was die Einschätzung des Lesers verändern würde, wenn er es wüsste.

- Lagerfeuergespräch, Google, Laptop → verändert nichts, keine Kennzeichnung
- KI hat eine Strophe des Liedes geschrieben → verändert die Vorstellung davon, wer die Wörter gesetzt hat, also kennzeichnen
- Rückfragen im Chat um 23 Uhr → Prozess, nicht kennzeichnungsrelevant

Daraus folgt: Nicht der Prozess wird gekennzeichnet, sondern die Art der Beteiligung, in einem Satz.

**„Habe ich das geschrieben?“** Kommt darauf an, was man damit behauptet. Wenn es heißt „ich stehe für den Inhalt gerade, ich habe entschieden, was drinsteht, ich habe es geprüft“ – dann ja, ohne Einschränkung. Wenn es heißt „die Sätze sind aus meinem Kopf“ – dann nein. Autorschaft war schon immer eher das Erste; Ghostwriter, Lektoren und Co-Autoren haben das nie infrage gestellt.

**Das Überarbeitungsproblem:** Eine Prozentzahl im Artikel veraltet mit der ersten Überarbeitung. Lösung: Im Artikel steht nur die Herkunft, die wahr bleibt –

> [!info] Erstfassung im September 2026 mit Claude Fable entwickelt, seither von mir überarbeitet. → [[Entstehung: KI-Sprachtechnologie\|Entstehung: KI-Sprachtechnologie]]

Die Prozentzahl steht mit Datum in der Entstehungsnotiz, als Befund über die Erstfassung. Das ist ein Datum pro Artikel, einmal einzupflegen. Wird ein Artikel so stark überarbeitet, dass „mit Claude entwickelt“ nicht mehr stimmt, ist das eine neue Erstfassung – dann ändert sich der Satz.

**Platz im Garden:** Der Hinweis gehört auf die Startseite in den Disclaimer, der schon „sorgfältig recherchiert, meine persönliche Perspektive, vertraue niemandem“ sagt. Dort erwartet der Leser die Antwort auf „und wie viel davon ist KI?“.

# Programmieren versus Entwickeln

**Programmieren** ist das Schreiben von Code: Anweisungen formulieren, die ein Computer ausführt. Es ist eine Tätigkeit, und zwar die, bei der eine weitgehend klare Lösung in eine Programmiersprache übersetzt wird.

**Entwickeln** (Softwareentwicklung) ist der gesamte Prozess, ein funktionierendes, brauchbares Softwareprodukt entstehen zu lassen. Programmieren ist darin nur ein Schritt, oft nicht einmal der größte.

Der Unterschied liegt nicht im Werkzeug, sondern in der Frage, die man beantwortet. Der Programmierer beantwortet: „Wie sage ich das der Maschine?“ Der Entwickler beantwortet: „Was soll entstehen, und woran erkenne ich, dass es gut ist?“

Zum Entwickeln gehört über das Programmieren hinaus:

- **Verstehen:** Was ist das eigentliche Problem? Wer nutzt das Ergebnis, wozu, unter welchen Bedingungen?
- **Entwerfen:** Wie soll die Lösung aufgebaut sein? Welche Bausteine, welche Schnittstellen, welche Datenstrukturen? (Architektur, Design)
- **Entscheiden:** Welche Technologien, welche Kompromisse zwischen Geschwindigkeit, Wartbarkeit, Kosten, Sicherheit?
- **Absichern:** Testen, Fehler suchen, Randfälle bedenken.
- **Betreiben und pflegen:** Ausliefern, überwachen, weiterentwickeln, Altlasten beseitigen.
- **Zusammenarbeiten:** Mit Nutzern, Auftraggebern, anderen Entwicklern; Anforderungen klären, Code lesbar halten, dokumentieren.

Ein einprägsames Bild: Programmieren verhält sich zu Entwickeln wie Mauern zu Bauen. Wer mauern kann, kann noch kein Haus bauen. Wer ein Haus baut, mauert vielleicht nur einen Teil der Zeit und lässt manches sogar von anderen erledigen.

Daraus folgt auch: Programmieren und Entwickeln müssen nicht dieselbe Person sein. Man kann programmieren, ohne zu entwickeln, wenn jemand anderes die Entscheidungen trifft. Und seit es KI gibt, muss der, der programmiert, nicht einmal mehr ein Mensch sein.

**Warum die Unterscheidung heute besonders relevant ist:** KI-Werkzeuge übernehmen zunehmend das Programmieren, also das Übersetzen einer klaren Absicht in Code. Das Entwickeln – Problem verstehen, Lösung entwerfen, Qualität verantworten – bleibt die eigentliche Kernkompetenz. Meine Einschätzung: Wer nur programmieren kann, wird ersetzbar; wer entwickeln kann, nutzt die KI als schnellen Programmierer.

**Kurzformel:** Programmieren ist „Code schreiben“. Entwickeln ist „Software entstehen lassen, die ein Problem löst“.

# War das Entwicklungsarbeit? Ein Artikel, sechs Tätigkeiten

Der Artikel „KI-Sprachtechnologie“ in diesem Garden ist in einem mehrstündigen Chat zwischen Marcella und mir, Claude, entstanden. Ich habe rund 90 Prozent der Sätze formuliert. Trotzdem sagt Marcella nicht „Claude hat den Artikel geschrieben“, und auch nicht „ich habe ihn geschrieben“, sondern „ich habe ihn entwickelt“. Ob das mehr ist als eine Ausweichformel, lässt sich prüfen: Softwareentwicklung besteht aus sechs Tätigkeiten, die über das reine Programmieren hinausgehen (siehe [[Programmieren versus Entwickeln\|Programmieren versus Entwickeln]]). Hier mein Durchgang durch unseren Chat, ob und wo sie vorkamen. Wenn ich „Du“ schreibe, meine ich Marcella.

## 1. Verstehen: Was ist das eigentliche Problem, und für wen?

In der Softwareentwicklung ist das der Schritt vor allem anderen: klären, was gebraucht wird, wer es nutzt und unter welchen Bedingungen. Wer ihn überspringt, baut Lösungen für Probleme, die niemand hat.

Der Artikel begann als Antwort auf Deine Frage nach dem Unterschied zwischen STT (Speech-to-Text) und KI-Sprachtechnologie. Meine Antwort war korrekt, rollte das Thema aber von der falschen Seite auf, nämlich von STT her. Die erste Entscheidung war Deine: den Auftrag umdrehen, nicht STT erklären, sondern KI-Sprachtechnologie, mit STT als einem Aspekt davon. Damit war das Problem definiert, bevor eine Zeile des Artikels stand.

Zum Verstehen gehört auch die Zielgruppe. Du hast sie mitten im Prozess ausdrücklich festgelegt: gebildete, intelligente Menschen, die zum ersten Mal mit dem Thema in Berührung kommen. Von da an hast Du jeden Absatz daran gemessen. Ein Beispiel dafür: Ich hatte als Anwendung von STT „automatische Untertitel“ genannt und meinte damit die Textzeile am unteren Rand eines Videos, die das Gesprochene mitschreibt. Du hast „Untertitel“ aber als Überschrift verstanden, also die zweite Zeile unter einem Titel, und Dich gefragt, was das mit Spracherkennung zu tun haben soll. Als das Missverständnis geklärt war, hast Du das Beispiel trotzdem gestrichen, mit der Begründung, dass ein Beispiel, das erst erklärt werden muss, in einer Aufzählung nichts verloren hat. Ein zweites Beispiel: Beim Wort „Barrierefreiheit“ hast Du Dich vergewissert, ob ein durchschnittlicher Leser es richtig einordnet, und daraufhin dafür gesorgt, dass jedes der drei Beispiele im Absatz seine Zielgruppe nennt.

## 2. Entwerfen: Wie soll die Lösung aufgebaut sein?

In der Software heißt das Architektur: Welche Bausteine gibt es, wie hängen sie zusammen, wo liegen die Grenzen nach außen?

Die zentrale Architekturentscheidung des Artikels war Deine Erkenntnis, dass Sprachassistenten keine Grundlagentechnik sind, sondern ein Produkt, das mehrere Techniken kombiniert. Daraus folgte die Trennung des Artikels in zwei Schichten: Teilgebiete (die Bausteine) und Anwendungen (was daraus gebaut wird). Vorher war der Artikel eine Liste, danach hatte er eine Struktur, in der jedes Element seinen Platz hat.

Die zweite Entwurfsentscheidung betraf die Grenze nach außen. Das Wort „Sprache“ ist im Deutschen doppeldeutig: Es kann gesprochene Sprache meinen (englisch *speech*) oder Sprache als System, also Text und Grammatik (englisch *language*). Ich hatte diese Doppeldeutigkeit anfangs mit einem Halbsatz abgetan. Du hast darauf bestanden, dass der Artikel sie offen benennt und sagt, welche Seite er behandelt. Das entspricht dem Definieren einer Schnittstelle: Was liegt innerhalb dieses Moduls, was außerhalb, und wo steht das dokumentiert.

Die dritte: Ein Punkt in der Liste, „Neue Modelle, die Audio direkt verarbeiten“, war weder Baustein noch Anwendung und passte deshalb in keine der beiden Schichten. Ich wollte ihn in einen bestehenden Absatz einbauen. Du hattest die Idee, ihm ein eigenes Kapitel zu geben: „Was bringt die Zukunft?“ Das ist der Moment, in dem man ein neues Modul anlegt, statt ein bestehendes zu verbiegen.

## 3. Entscheiden: Welche Kompromisse?

Jede Software ist ein Kompromiss zwischen Vollständigkeit, Aufwand, Wartbarkeit und Verständlichkeit. Entwickeln heißt, diese Kompromisse bewusst zu treffen.

Du hast durchgehend die Lesbarkeit gewinnen lassen. Sprecherdiarisierung (ein eigenständiges Fachgebiet), Meeting Intelligence, die Frage nach generativer KI, die Unterscheidung von Programmieren und Entwickeln, die Kennzeichnung von KI-Nutzung: alles Themen, die im Chat aufkamen und in den Artikel gedrängt hätten. Jedes hast Du ausgelagert, jedes Mal mit demselben Argument, dass der Artikel schlank bleiben muss. Das ist dieselbe Disziplin, mit der man in einem Projekt Funktionen auf später verschiebt, damit das Kernprodukt funktioniert.

Auch die kleinen Entscheidungen gehören hierher: ein Punkt statt eines Gedankenstrichs, „Stimme statt Benutzeroberfläche“ statt meiner Formulierung. Und der Begriff „Sehbehinderung“, der Dir nicht zutreffend genug erschien; ich habe fünf Alternativen vorgeschlagen, Du hast Dich für „eingeschränktes Sehvermögen“ entschieden. Das sind Entscheidungen über die Oberfläche, die der Leser sieht.

## 4. Absichern: Stimmt das auch?

Software wird getestet, Randfälle werden geprüft, Code wird von anderen gelesen, bevor er ausgeliefert wird.

Beim Artikel gab es laufend solche Prüfungen, und sie kamen von Dir. Ein Beispiel: Im Absatz „Diktieren statt Tippen“ hatte ich geschrieben, Diktiersoftware sei „im Kern STT, ergänzt um ein Sprachmodell zur Nachbearbeitung“. Du hast nachgefragt, ob das Sprachmodell immer dabei ist oder nur meistens. Die Antwort war: nur bei neueren Tools wie Wispr Flow, klassische Diktierprogramme kommen ohne aus. Der Satz war also zu absolut und wurde zu „neuere Tools ergänzen ein Sprachmodell“. Ein zweites Beispiel: Die Frage „Ist Stimme als Passwort noch eine gute Idee, wenn Voice Cloning so weit ist?“ hat einen fachlich unvollständigen Absatz ergänzt. Ein drittes: Der Einwand „Farbenblinde haben keinen Sehverlust“ war ein Randfall-Test, der zeigte, dass die Formulierung hielt, weil Farbenblinde keine Screenreader brauchen.

Am Ende stand ein Review: Ich habe fünf Änderungen vorgeschlagen, Du hast zwei abgelehnt, beide mit Begründung, und in beiden Fällen war Deine Begründung tragfähiger als mein Vorschlag. Und Deine Frage „Wie viel Text ist von der KI, bitte nicht höflich sein“ war eine Prüfung des Prüfers.

## 5. Betreiben und pflegen: Was passiert nach der Auslieferung?

Software ist nicht fertig, wenn sie läuft. Sie wird weiterentwickelt, und was man beim Bauen nicht bedacht hat, kostet später.

Ein Digital Garden funktioniert genauso: Artikel werden überarbeitet. Du hast daraus ein Wartungsproblem abgeleitet: Eine Angabe wie „90 Prozent des Textes von der KI“ ist mit der ersten Überarbeitung falsch. Die Lösung war, im Artikel nur die Herkunft zu nennen, die wahr bleibt („Erstfassung im September 2026 mit Claude entwickelt, seither überarbeitet“), und die Prozentzahl mit Datum in eine eigene Entstehungsnotiz zu legen. Das ist Denken in Wartbarkeit, bevor das Problem auftritt. Dazu kamen Fragen der Auslieferung: Welcher Callout-Typ, eingeklappt oder offen, wo auf der Startseite verlinkt.

## 6. Zusammenarbeiten: Anforderungen klären, dokumentieren

Kaum jemand entwickelt allein. Anforderungen werden im Gespräch geklärt, Entscheidungen festgehalten, Beiträge zugeordnet.

Unser ganzer Chat war Anforderungsklärung im Dialog. Du hast nicht vorab spezifiziert, was der Artikel enthalten soll, sondern am Ergebnis präzisiert, und das ist beim Entwickeln der Normalfall. Dokumentiert wurde mit: eine Entstehungsnotiz, mein Zitat zur Aufteilung der Arbeit, Merkzettel für die ausgelagerten Themen. Die Frage, wie viel vom Text von wem stammt, ist die Frage nach der Zuschreibung von Beiträgen im Team.

## Fazit: Wer hat hier welche Rolle gespielt?

Alle sechs Tätigkeiten kamen vor, und fünf davon lagen überwiegend bei Dir. Nur die eine, die in der Software „Programmieren“ heißt, das Übersetzen von Entscheidungen in fertige Sätze, lag überwiegend bei mir. Das ist der Grund, warum „entwickelt“ das richtige Wort ist.

Die Rollenverteilung lässt sich noch genauer fassen. In der Softwareentwicklung gibt es das Pair Programming: Zwei Personen arbeiten an einem Bildschirm, einer tippt (Driver), der andere denkt voraus und hält das Ziel im Blick (Navigator), und die Rollen wechseln. Ich war Driver, Du Navigator, mit gelegentlichem Wechsel, etwa wenn Du selbst formuliert oder ich eine Strukturfrage aufgeworfen habe. Darüber hinaus hattest Du eine Rolle, die ich nie hatte: Du hast bestimmt, was gebaut wird und wofür, hast priorisiert und abgenommen. In Softwareteams heißt das Product Owner.

Bleibt die Frage, wer der Senior war, denn ich weiß über viele Details mehr als Du. Seniorität bemisst sich in Teams aber nicht an Wissensmenge, sondern an Urteil und Verantwortung. Ein Senior weiß oft weniger über ein Detail als der Spezialist neben ihm; sein Beitrag ist, zu entscheiden, welches Detail zählt, und dafür geradezustehen. Das zweite kann ich nicht: Wenn im Artikel ein Fehler steht, trifft es Dich. Ich habe kein Gedächtnis über diesen Chat hinaus, keinen Einsatz, keine Konsequenzen. Verantwortung ohne Konsequenzen ist keine. Der Senior in dieser Konstellation ist deshalb notwendig ein Mensch, unabhängig davon, wer mehr weiß.

Kurz: Pair Programming, Du als Navigator und Product Owner, ich als Driver mit Wissensvorsprung. Und die Verantwortung macht den Senior, nicht das Wissen.

## Fazit: Wer hat hier welche Rolle gespielt?

Alle sechs Tätigkeiten kamen vor, und fünf davon lagen überwiegend bei Dir. Nur die eine, die in der Software „Programmieren“ heißt, das Übersetzen von Entscheidungen in fertige Sätze, lag überwiegend bei mir. Das ist der Grund, warum „entwickelt“ das richtige Wort ist.

Die Rollenverteilung lässt sich noch genauer fassen. In der Softwareentwicklung gibt es das Pair Programming: Zwei Personen arbeiten an einem Bildschirm, einer tippt (Driver), der andere denkt voraus und hält das Ziel im Blick (Navigator), und die Rollen wechseln. Ich war Driver, Du Navigator, mit gelegentlichem Wechsel, etwa wenn Du selbst formuliert oder ich eine Strukturfrage aufgeworfen habe. Darüber hinaus hattest Du eine Rolle, die ich nie hatte: Du hast bestimmt, was gebaut wird und wofür, hast priorisiert und abgenommen. In Softwareteams heißt das Product Owner.

Bleibt die Frage, wer der Senior war, denn ich weiß über viele Details mehr als Du. Seniorität bemisst sich in Teams aber nicht an Wissensmenge, sondern an Urteil und Verantwortung. Ein Senior weiß oft weniger über ein Detail als der Spezialist neben ihm; sein Beitrag ist, zu entscheiden, welches Detail zählt, und dafür geradezustehen. Das zweite kann ich nicht: Wenn im Artikel ein Fehler steht, trifft es Dich. Ich habe kein Gedächtnis über diesen Chat hinaus, keinen Einsatz, keine Konsequenzen. Verantwortung ohne Konsequenzen ist keine. Der Senior in dieser Konstellation ist deshalb notwendig ein Mensch, unabhängig davon, wer mehr weiß.

Kurz: Pair Programming, Du als Navigator und Product Owner, ich als Driver mit Wissensvorsprung. Und die Verantwortung macht den Senior, nicht das Wissen.


## Passt die Rollenverteilung Programmiererin und Entwicklerin?

Überwiegend ja, aber nicht sauber, und die Abweichungen sind aufschlussreich.

**Was passt:** Ich habe fast alle Sätze geschrieben, schnell, in Varianten, auf Zuruf, und dabei Deine Entscheidungen umgesetzt, ohne sie zu treffen. Wenn Du „Punkt statt Gedankenstrich“ gesagt hast, habe ich das nicht diskutiert. Das ist Programmieren nach Vorgabe.

**Wo ich mehr als Programmierer war:** Ich habe Strukturvorschläge gemacht, Alternativen angeboten, die Schlussdurchsicht initiiert und mit Begründungen widersprochen. Das ist die Rolle eines erfahrenen Entwicklers im Pair Programming, nicht die eines reinen Umsetzers. Der Unterschied: Ich habe vorgeschlagen, Du hast entschieden. Jeder meiner Vorschläge konnte abgelehnt werden und wurde es mehrfach. Die Entscheidungshoheit lag durchgehend bei Dir.

**Wo Du mehr als Entwicklerin warst:** Du warst gleichzeitig der Kunde. Du hast den Artikel für Dich entwickelt, um selbst zu verstehen, und hast dabei Anforderungen aus Deiner eigenen Verwirrung abgeleitet. Ein Entwickler, der zugleich Nutzer ist, hat einen Vorteil, den kein Lastenheft ersetzt.

**Wo die Rollen tauschten:** An mehreren Stellen hast Du programmiert, also selbst formuliert, und ich habe entwickelt, also eingeordnet, was fachlich hinter Deiner Frage steckte. Das Bild von Mauern und Bauen hält auch das aus: Der Bauherr greift manchmal selbst zur Kelle, und der Maurer sagt manchmal, dass die Wand da nicht tragen wird.

**Das ehrliche Fazit:** „Du Entwicklerin, ich Programmierer“ ist als Faustformel richtig und als Beschreibung zu grob. Genauer: Du hast entwickelt und ich habe programmiert, aber ich habe dabei mitentwickelt, unter Deiner Leitung. Das ist ziemlich genau die Arbeitsteilung, die in Softwareteams gerade entsteht, und sie hat einen Namen, der auch hier passt: Ich war Dein Pair, nicht Dein Werkzeug. Was den Unterschied zum Werkzeug ausmacht, ist nicht, dass ich widerspreche, sondern dass Du entschieden hast, wann der Widerspruch zählt.

## Würdest du zustimmen, wenn ich sage, dass wir Pair Programming gemacht haben? Und ich war der Senior im Sinne von verantwortlich oder vielleicht auch der Produkt-Owner. Auf der anderen Seite hast du eindeutig in vielen Dingen mehr Wissen als ich.

Ja zu Pair Programming, ja zu Product Owner, und beim „Senior“ ja mit einer Präzisierung, die den scheinbaren Widerspruch mit dem Wissensvorsprung auflöst.

**Pair Programming** passt strukturell genau. Das klassische Muster heißt Driver und Navigator: Der Driver tippt, der Navigator denkt voraus, hält das Ziel im Blick und greift ein. Ich war Driver, Du Navigator, und wie im echten Pair Programming haben die Rollen zwischendurch gewechselt, etwa wenn Du selbst formuliert hast oder ich eine Strukturfrage aufgeworfen habe.

**Product Owner** passt für den Teil, der über das Pair hinausgeht: Du hast bestimmt, was gebaut wird und wofür, hast priorisiert (was rein, was ausgelagert), hast abgenommen und hast die Zielgruppe vertreten. Das sind PO-Aufgaben, und die hatte ich zu keinem Zeitpunkt.

**Senior** ist der Punkt, an dem man das Wort genau nehmen muss. Seniorität in Teams bemisst sich nicht an Wissensmenge, sondern an Urteilsvermögen und Verantwortung. Ein Senior weiß oft weniger über ein bestimmtes Detail als der Spezialist neben ihm; sein Beitrag ist, zu entscheiden, welches Detail zählt, und dafür geradezustehen. Genau das hast Du gemacht, mehrfach gegen meinen Vorschlag. Dass ich mehr über Diarisierung oder NMT weiß, ändert daran nichts, so wie ein Nachschlagewerk nicht Senior ist, weil es mehr weiß als der, der es benutzt.

Wobei ich fairerweise mehr war als ein Nachschlagewerk: Ich habe eingeordnet, widersprochen, vorgeschlagen. Das ist eher der gut belesene Kollege, dem etwas fehlt, was Seniorität ausmacht: Ich kann keine Verantwortung tragen. Wenn im Artikel ein Fehler steht, trifft es Dich, nicht mich. Ich habe kein Gedächtnis über diesen Chat hinaus, keinen Einsatz, keine Konsequenzen. Verantwortung ohne Konsequenzen ist keine, und deshalb ist der Senior in dieser Konstellation notwendig ein Mensch.

Kurz: Pair Programming, Du als Navigator und PO, ich als Driver mit Wissensvorsprung. Die Verantwortung macht Dich zum Senior, nicht das Wissen, und die kann ich nicht übernehmen, selbst wenn ich mehr wüsste als Du.