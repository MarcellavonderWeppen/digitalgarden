---
{"title":"Klassische KI","aliases":["klassische KI","symbolische KI","regelbasierte KI"],"tags":null,"gen_ai_anteil":["Gemini 20%","Claude 20%"],"created":"2026-04-07","updated":"2026-06-06","status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/3-work-on-tomorrow/klassische-ki/","dgPassFrontmatter":true,"dg-note-properties":{"title":"Klassische KI","aliases":["klassische KI","symbolische KI","regelbasierte KI"],"tags":null,"gen_ai_anteil":["Gemini 20%","Claude 20%"],"created":"2026-04-07","updated":"2026-06-06","status":null}}
---

# Klassische KI

> [!info] **Synonyme und verwandte Begriffe**: 
> symbolische KI, regelbasierte KI, „Good Old-Fashioned AI“ (GOFAI), wissensbasierte Systeme

Viele Jahrzehnte bevor ChatGPT das Licht der Welt erblickte und einen ungeahnten KI-Hype auslöste, gab es KI schon als Forschungsfeld und entwickelte sich ohne große öffentliche Aufmerksamkeit. Ins Leben gerufen wurde sie 1956 auf der Dartmouth Conference, als sich einige Größen der Computerwissenschaften trafen und John McCarthy ihr mit dem Begriff „Artificial Intelligence“ offiziell ihren Namen gab.

Die **klassische künstliche Intelligenz** basiert auf der Idee, dass Intelligenz durch **explizite Regeln und Symbole** beschrieben werden kann:

- Wissen wird formal dargestellt, z. B. als Fakten und Wenn-Dann-Regeln
- Dieses Wissen wird mit zwei zentralen, oft kombinierten Verfahren verarbeitet:
    - **Logisches Ableiten**: Aus Fakten und Regeln werden neue Schlüsse gezogen
    - **Suche**: Mögliche Lösungswege werden durchprobiert und bewertet

## Typische Beispiele

- Expertensysteme, z. B. MYCIN (1970er Jahre), das bakterielle Infektionen diagnostizierte und passende Antibiotika empfahl
- Logikbasierte Programme, z. B. der „Logic Theorist“ (1956), der mathematische Lehrsätze selbstständig bewies
- Klassische Schachprogramme, z. B. Deep Blue, das 1997 den Schachweltmeister Kasparow schlug

| Verfahren          | Grundidee                                              | Typisches Beispiel                        |
| ------------------ | ------------------------------------------------------ | ----------------------------------------- |
| Logisches Ableiten | Wenn-Dann-Regeln werden auf bekannte Fakten angewendet | logikbasiertes Programme, Expertensysteme |
| Suche              | Mögliche Lösungswege werden schrittweise erkundet      | klassische Schachprogramme, Routenplaner  |

## Formal repräsentiert

In Abhandlungen über klassische KI heißt es oft, Wissen wird formal oder explizit repräsentiert. Aber was bedeutet das überhaupt?

Explizit heißt: Das Wissen steht lesbar im System. Man kann hineinschauen und findet Zeile für Zeile, was das Programm „weiß“: Fakten wie „Tweety ist ein Vogel“ und Regeln wie „Vögel können fliegen“. Ein Mensch hat sie hingeschrieben, ein Mensch kann sie lesen, prüfen und korrigieren.

Formal heißt hier nicht „förmlich“, sondern „die Form betreffend“. Das Wissen ist in einer eindeutigen Kunstsprache notiert, und was sich daraus ableiten lässt, ergibt sich allein aus dem Aufbau der Sätze, nicht aus ihrer Bedeutung.

Was das heißt, zeigt ein kleiner Test: „Alle Flurbs sind Gnaks. Zork ist ein Flurb. Also ist Zork ein Gnak.“ Niemand weiß, was ein Flurb oder ein Gnak ist. Trotzdem erkennen logisch denkende Menschen sofort, dass der Schluss stimmt. Wir brauchen nur das Muster: „Alle A sind B, x ist A, also ist x B.“ Mit Tweety funktioniert es genauso: Aus „Alle Vögel fliegen“ und „Tweety ist ein Vogel“ folgt „Tweety fliegt“. Dass wir hier zufällig wissen, was ein Vogel ist, spielt für die Schlussfolgerung keine Rolle.

Genau das macht den Ansatz für Computer tauglich: Ein Rechner versteht nichts. Für ihn ist „Vogel“ genauso bedeutungslos wie „Flurb“. Er kann nur Zeichen vergleichen und nach Regeln umbauen. Ist das Wissen formal notiert, wird Schlussfolgern zu einem rein mechanischen Vorgang.

Ein medizinisches Expertensystem arbeitet genau so: „Wenn Fieber und Husten und Rasselgeräusche, dann Verdacht auf Lungenentzündung.“ Ein Arzt würde eher ein „kommt drauf an“ mit vielen Wenn und Aber formulieren. Formalisieren heißt, dieses „kommt drauf an“ in eindeutige Bedingungen zu übersetzen – oder wegzulassen.

Bei Schach gelingt das restlos. Bei Sprache, wie wir gleich sehen werden, nicht.

## Einordnung: Stärken und Grenzen der regelbasierten KI 

### Stark bei klaren, eindeutigen Regeln

Die klassische KI spielt ihre Stärke immer dann aus, wenn sich das Vorgehen bei einem Problem vollständig in Regeln fassen lässt.

Schach ist ein hochkomplexes Spiel, doch seine Regeln sind klar, eindeutig und lassen sich auf einer Seite zusammenfassen. 

Die klassischen Schachprogramme  funktionieren genau so: Menschen geben die Regeln vor, der Computer rechnet Millionen möglicher Züge durch.

### Komplexität von Sprachen: klassische KI stößt an ihre Grenzen

Sprache hat Regeln – ganze Bibliotheken voll: Grammatik, Rechtschreibung, Syntax. 

Die klassische KI hat jahrzehntelang versucht, Sprache über Regeln zu knacken, und ist daran  gescheitert. 

#### Der Grund: Sprache lässt sich durch Regeln nicht vollständig beschreiben.

Ein paar Beispiele machen das anschaulich:

- „Bank“ – Geldinstitut oder Sitzgelegenheit? Keine Grammatikregel sagt es einem, nur der Kontext.
- „Ich sah den Mann mit dem Fernglas.“ – Hatte ich das Fernglas oder er? Grammatisch beides korrekt.
- „Das ist ja mal eine tolle Idee.“ – Ernst gemeint oder Ironie? Hängt ab von Tonfall, Situation, Vorgeschichte.
- „Er hat den Löffel abgegeben.“ – Wörtlich oder gestorben? Eine Redewendung, die man einfach kennen muss.

Dazu kommen Dialekte, Slang, neue Wörter, Tippfehler, unvollständige Sätze, Anspielungen. 

Die Regeln, die Menschen beim Sprechen tatsächlich anwenden, sind zu viele, zu vage, zu kontextabhängig und zu ausnahmenreich, als dass sie sich vollständig aufschreiben ließen. 

#### Das Aufkommen eines neuen [[02 - Künstliche Intelligenz/5 - soon (veröffentlicht)/Paradigma (Denkmodell)\|Paradigmas]] 

Genau an dieser Stelle setzt die [[02 - Künstliche Intelligenz/0 - Final Check/Statistische KI\|statistische KI]] an: Sie lernt Sprache nicht über Regeln, sondern aus Milliarden von Beispielen.  

Die Idee künstlicher Neuronen reicht bis 1943 zurück, mit dem Perceptron gab es 1958 ein erstes lernfähiges neuronales Netz. Neuen Schwung bekam die Forschung daran in den 80ern, als die Grenzen der klassischen KI immer deutlicher wurden. Der breite Durchbruch ließ allerdings bis 2012 auf sich warten: Mit [[02 - Künstliche Intelligenz/5 - soon (veröffentlicht)/Machine Learning (ML)#Deep Learning\|Deep Learning]]gelang er zunächst in der Bilderkennung, wenige Jahre später auch bei Sprache.



