---
{"title":"Klassische KI","aliases":["klassische KI","symbolische KI","regelbasierte KI"],"tags":null,"gen_ai_anteil":["Gemini 20%","Claude 20%"],"created":"2026-04-07","updated":"2026-09-19","status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/erkunden/grundlagen-ki/klassische-ki/","dgPassFrontmatter":true,"dg-note-properties":{"title":"Klassische KI","aliases":["klassische KI","symbolische KI","regelbasierte KI"],"tags":null,"gen_ai_anteil":["Gemini 20%","Claude 20%"],"created":"2026-04-07","updated":"2026-09-19","status":null}}
---

# Klassische KI

> [!info] Synonyme und verwandte Begriffe:
> symbolische KI, regelbasierte KI, „Good Old-Fashioned AI“ (GOFAI), wissensbasierte Systeme

Viele Jahrzehnte bevor ChatGPT das Licht der Welt erblickte und einen ungeahnten KI-Hype auslöste, existierte KI längst als Forschungsfeld und entwickelte sich weitgehend ohne öffentliche Aufmerksamkeit. Ins Leben gerufen wurde sie 1956 auf der Dartmouth Conference, wo sich einige Größen der Computerwissenschaften trafen. Der Begriff „Artificial Intelligence“, von John McCarthy geprägt, wurde dort zum offiziellen Namen der noch jungen Disziplin. Diese frühe KI nennen wir rückblickend klassisch. Sie dominierte das Feld bis in die 80er Jahre, danach gewann der [[02 - Künstliche Intelligenz/Erkunden/Grundlagen KI/Statistische KI\|statistische Ansatz]] zunehmend an Bedeutung.

## Die Grundidee: Wissen in Regeln fassen

Die **klassische künstliche Intelligenz** basiert auf der Idee, dass Intelligenz durch **explizite Regeln und Symbole** beschrieben werden kann:

- Wissen wird formal dargestellt, z. B. als Fakten und Wenn-Dann-Regeln
- Dieses Wissen wird mit zwei zentralen, oft kombinierten Verfahren verarbeitet:
  - **Logisches Ableiten**: Aus Fakten und Regeln werden neue Schlüsse gezogen
  - **Suche**: Mögliche Lösungswege werden durchprobiert und bewertet

## Zwei Spielarten: Ableiten und Suchen

![Klassische KI Diagramm.png](/img/user/02%20-%20K%C3%BCnstliche%20Intelligenz/Erkunden/Bilder/Klassische%20KI%20Diagramm.png)

|                      | Regelbasierte Systeme                                                                                                                                                 | Such- und Planungsverfahren                                                                                                                                                             |
| -------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Prinzip**          | Logisches Ableiten                                                                                                                                                    | Suche                                                                                                                                                                                   |
| **Grundidee**        | Das System wendet vorformulierte Wenn-Dann-Regeln auf bekannte Fakten an und leitet daraus neue Schlüsse ab                                                           | Das System erkundet mögliche Lösungswege Schritt für Schritt, bewertet sie und verfolgt die aussichtsreichsten weiter                                                                   |
| **Typische Systeme** | logikbasierte Programme, Expertensysteme                                                                                                                              | klassische Schachprogramme, Routenplaner                                                                                                                                                |
| **Beispiel**         | **Logic Theorist** (1956):<br>bewies mathematische Lehrsätze <br> <br>**MYCIN** (1970er):<br>diagnostizierte bakterielle Infektionen und empfahl passende Antibiotika | **Deep Blue** (1997):<br>schlug Schachweltmeister Kasparow <br> <br>**Dijkstra-Algorithmus** (1959):<br>bis heute grundlegendes Prinzip der Routenplanung, von Google Maps bis zum Navi |

## Was heißt „formal repräsentiert“?

In Abhandlungen über klassische KI heißt es oft: Wissen wird formal oder explizit repräsentiert. Aber was bedeutet das überhaupt?

Explizit heißt: Das Wissen steht lesbar im System. Man kann hineinschauen und findet Zeile für Zeile, was das Programm „weiß“: Fakten wie „Tweety ist ein Vogel“ und Regeln wie „Vögel können fliegen“. Ein Mensch hat sie hingeschrieben, ein Mensch kann sie lesen, prüfen und korrigieren.

Formal heißt hier nicht „förmlich“, sondern „die Form betreffend“. Das Wissen ist in einer Kunstsprache notiert: einem festen Vorrat an Zeichen samt klaren Regeln, wie sich diese Zeichen verknüpfen lassen. Ähnlich wie in der Mathematik oder in einer Programmiersprache. Was sich daraus ableiten lässt, ergibt sich allein aus dem Aufbau der Sätze, nicht aus ihrer Bedeutung.

Schauen wir uns zum besseren Verständnis ein Beispiel dazu an: „Alle Flurbs sind Gnaks. Zork ist ein Flurb. Also ist Zork ein Gnak.“ Niemand weiß, was ein Flurb oder ein Gnak ist. Trotzdem erkennen logisch denkende Menschen sofort, dass der Schluss folgerichtig ist. Wir brauchen nur das Muster: „Alle A sind B, x ist A, also ist x B.“ Mit Tweety funktioniert es genauso: Aus „Alle Vögel fliegen“ und „Tweety ist ein Vogel“ folgt „Tweety fliegt“. Dass wir hier zufällig wissen, was ein Vogel ist, spielt für die Schlussfolgerung keine Rolle.

![Kunstsprache Logik.png](/img/user/02%20-%20K%C3%BCnstliche%20Intelligenz/Erkunden/Bilder/Kunstsprache%20Logik.png)

Genau das macht den Ansatz für Computer tauglich: Ein Rechner versteht nichts. Für ihn ist „Vogel“ genauso bedeutungslos wie „Flurb“. Er kann nur Zeichen vergleichen und Sätze nach festen Regeln umbauen. Ist das Wissen formal notiert, wird Schlussfolgern zu einem rein mechanischen Vorgang.

Diese Zeichen nennt man in der KI **Symbole** – daher auch symbolische KI als Synonym für klassische KI. Ein Symbol ist ein Platzhalter, der für etwas in der Welt steht: „Vogel“, „Fieber“, „Tweety“. Für den Computer sind es leere Hüllen, die er nach Regeln hin- und herschiebt. Die Bedeutung entsteht allein im Kopf des Menschen, der die Symbole festgelegt hat.

Ein medizinisches Expertensystem arbeitet genau so: „Wenn Fieber und Husten und Rasselgeräusche, dann Verdacht auf Lungenentzündung.“ Ein menschlicher Arzt würde eher antworten: „Kommt drauf an“ – mit vielen Wenn und Aber. Formalisieren heißt, dieses „Kommt drauf an“ in eindeutige Bedingungen zu übersetzen – oder wegzulassen.

Bei Schach gelingt das restlos. Bei Phänomenen wie Sprache nicht, wie wir gleich sehen werden.

## Einordnung: Stärken und Grenzen der symbolischen KI

### Stark bei klaren, eindeutigen Regeln

Die klassische KI spielt ihre Stärke immer dann aus, wenn sich das Vorgehen bei einem Problem vollständig in Regeln fassen lässt.

Schach ist ein hochkomplexes Spiel, doch die Regeln sind klar, eindeutig und lassen sich auf einer Seite zusammenfassen.

Die klassischen Schachprogramme funktionieren genau so: Menschen geben die Regeln vor, der Computer rechnet Millionen möglicher Züge durch.

### Komplexität von Sprache: klassische KI stößt an ihre Grenzen

Sprache hat Regeln – ganze Bibliotheken voll: Grammatik, Rechtschreibung, Syntax.

Die klassische KI hat jahrzehntelang versucht, Sprache über Regeln zu knacken, und ist daran gescheitert.

#### Der Grund: Sprache lässt sich durch Regeln nicht vollständig beschreiben

Ein paar Beispiele machen das anschaulich:

- „Bank“ – Geldinstitut oder Sitzgelegenheit? Keine Grammatikregel sagt es einem, nur der Kontext.
- „Ich sah den Mann mit dem Fernglas.“ – Hatte ich das Fernglas oder er? Grammatisch beides korrekt.
- „Das ist ja mal eine tolle Idee.“ – Ernst gemeint oder Ironie? Hängt ab von Tonfall, Situation, Vorgeschichte.
- „Er hat den Löffel abgegeben.“ – Wörtlich oder gestorben? Eine Redewendung, die man einfach kennen muss.

Dazu kommen Dialekte, Slang, neue Wörter, Tippfehler, unvollständige Sätze, Anspielungen.

Die Regeln, die Menschen beim Sprechen tatsächlich anwenden, sind zu viele, zu vage, zu kontextabhängig und zu ausnahmenreich, als dass sie sich vollständig aufschreiben ließen.

## Das Aufkommen eines neuen [[02 - Künstliche Intelligenz/5 - soon (veröffentlicht)/Paradigma (Denkmodell)\|Paradigmas]]

Was für Sprache gilt, trifft auch auf viele andere Felder zu, wie zum Beispiel die Bilderkennung: Wie unterscheide ich einen Hund von einer Katze? Uns Menschen gelingt das mühelos, auch wenn wir wahrscheinlich nicht erklären können, wie wir das machen. Für klassische KI: ein quasi unlösbares Problem.

Genau an dieser Stelle setzt die [[02 - Künstliche Intelligenz/Erkunden/Grundlagen KI/Statistische KI\|statistische KI]] an: Anstatt mit vorgegebenen Regeln zu arbeiten, lernt sie Muster aus unzähligen Beispielen.

Die Idee künstlicher Neuronen reicht bis 1943 zurück; mit dem Perceptron gab es 1958 ein erstes lernfähiges neuronales Netz. Neuen Schwung bekam die Forschung in den 80ern, als die Grenzen der klassischen KI immer deutlicher wurden. Der breite Durchbruch ließ allerdings noch bis 2012 auf sich warten: Mit [[02 - Künstliche Intelligenz/5 - soon (veröffentlicht)/Machine Learning (ML)#Deep Learning\|Deep Learning]] gelang er zunächst in der Bilderkennung, wenige Jahre später auch bei Sprache.

> [!tip] Selbst ausprobiert
> Warum ausgerechnet die Bilderkennung so lange ein Problem war, zeigt ein kleines Experiment, das mich zum Schmunzeln brachte: Ich habe eine KI alle Regeln aufschreiben lassen, an denen man einen Hund von einer Katze unterscheidet – und dann geprüft, ob die Regeln halten, was sie versprechen.
>
> 👉 [[02 - Künstliche Intelligenz/3 - Work on tomorrow/Hund oder Katze? Das Experiment\|Das Experiment]]
