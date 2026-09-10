---
{"title":"Klassische KI","aliases":["klassische KI","symbolische KI","regelbasierte KI"],"tags":null,"gen_ai_anteil":["Gemini 20%","Claude 20%"],"created":"2026-04-07","updated":"2026-06-06","status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/3-work-on-tomorrow/klassische-ki/","dgPassFrontmatter":true,"dg-note-properties":{"title":"Klassische KI","aliases":["klassische KI","symbolische KI","regelbasierte KI"],"tags":null,"gen_ai_anteil":["Gemini 20%","Claude 20%"],"created":"2026-04-07","updated":"2026-06-06","status":null}}
---

# Klassische KI

> [!info] **Synonyme und verwandte Begriffe**: 
> symbolische KI, regelbasierte KI, „Good Old-Fashioned AI“ (GOFAI), wissensbasierte Systeme

Viele Jahrzehnte bevor ChatGPT das Licht der Welt erblickte und einen ungeahnten KI-Hype auslöste, gab es KI schon als Forschungsfeld und entwickelte sich ohne große öffentliche Aufmerksamkeit. Ins Leben gerufen wurde sie 1956 auf der Dartmouth Conference, als sich einige Größen der Computerwissenschaften trafen und John McCarthy ihr mit dem Begriff „Artificial Intelligence“ offiziell ihren Namen gab.

Die **klassische künstliche Intelligenz** basiert auf der Idee, dass Intelligenz durch **explizite Regeln und Symbole** beschrieben werden kann.

- Wissen wird **formal repräsentiert** (z. B. als Regeln, Fakten, Logik)
- Schlussfolgerungen erfolgen durch logisches Ableiten
- **Wenn-Dann-Regeln** (oder systematisches Durchsuchen vieler Möglichkeiten)

Typische Beispiele sind

- Expertensysteme (z. B. medizinische Diagnosesysteme)
- Logikbasierte Programme 
- Schach (klassische Schachprogramme wie Deep Blue, das 1997 Kasparow schlug)

## Formal repräsentiert

In Abhandlungen über klassische KI heißt es oft, Wissen wird formal oder explizit repräsentiert. Aber was bedeutet das überhaupt?

Explizit heißt: Das Wissen steht lesbar im System. Man kann hineinschauen und findet Zeile für Zeile, was das Programm „weiß“: Fakten wie „Tweety ist ein Vogel“ und Regeln wie „Vögel können fliegen“. Ein Mensch hat sie hingeschrieben, ein Mensch kann sie lesen, prüfen und korrigieren.

Formal heißt hier nicht „förmlich“, sondern „auf die Form bezogen“. Das Wissen ist in einer präzisen Kunstsprache notiert, in der allein die Gestalt der Zeichen festlegt, was daraus folgt. Aus „Alle Vögel fliegen“ und „Tweety ist ein Vogel“ ergibt sich „Tweety fliegt“ – nach dem Muster „Alle A sind B, x ist A, also x ist B“. Das Muster funktioniert für beliebige A, B und x. Was ein Vogel ist, muss dafür niemand wissen.

Genau das macht den Ansatz für Computer tauglich: Ein Rechner versteht nichts, er kann nur Zeichen vergleichen und nach Regeln umbauen. Ist das Wissen formal notiert, wird Schlussfolgern zu einem rein mechanischen Vorgang.

Ein medizinisches Expertensystem arbeitet so: „Wenn Fieber und Husten und Rasselgeräusche, dann Verdacht auf Lungenentzündung.“ Ein Arzt würde dasselbe eher als „kommt drauf an“ mit vielen Wenn und Aber formulieren. Formalisieren heißt, dieses „kommt drauf an“ in eindeutige Bedingungen zu übersetzen – oder wegzulassen.

Bei Schach gelingt das restlos. Bei Sprache, wie wir gleich sehen werden, nicht.

## Einordnung: Stärken und Grenzen der regelbasierten KI 

### Stark bei klaren, eindeutigen Regeln

Die klassische KI spielt ihre Stärke immer dann aus, wenn sich das Vorgehen bei einem Problem vollständig in Regeln fassen lässt.

Schach ist ein hochkomplexes Spiel, doch seine Regeln sind klar, eindeutig und lassen sich auf einer Seite zusammenfassen. 

Die klassischen Schachprogramme – bis hin zu Deep Blue, das 1997 Weltmeister Kasparow schlug – funktionierten genau so: Menschen gaben die Regeln vor, der Computer rechnete Millionen möglicher Züge durch.

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

Selbst wenn man all das in Regeln fassen wollte – niemand hat es je geschafft. 

Die Regeln, die Menschen beim Sprechen tatsächlich anwenden, sind zu viele, zu vage, zu kontextabhängig und zu ausnahmenreich, als dass sie sich vollständig aufschreiben ließen. 

#### Das Aufkommen eines neuen [[02 - Künstliche Intelligenz/5 - soon (veröffentlicht)/Paradigma (Denkmodell)\|Paradigmas]] 

Genau an dieser Stelle setzt die [statistische KI](Statistische KI) an: Sie lernt Sprache nicht über Regeln, sondern aus Milliarden von Beispielen.  

Die Idee künstlicher Neuronen reicht bis 1943 zurück, mit dem Perceptron gab es 1958 ein erstes lernfähiges neuronales Netz. Neuen Schwung bekam die Forschung daran in den 80ern, als die Grenzen der klassischen KI immer deutlicher wurden. Der breite Durchbruch ließ allerdings bis 2012 auf sich warten: Mit [Deep Learning](Machine Learning (ML)#Deep Learning) gelang er zunächst in der Bilderkennung, wenige Jahre später auch bei Sprache.



