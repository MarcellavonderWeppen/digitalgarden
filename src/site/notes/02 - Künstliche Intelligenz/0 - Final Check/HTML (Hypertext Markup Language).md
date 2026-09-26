---
{"title":"HTML (Hypertext Markup Language)","aliases":["HTML"],"tags":null,"gen_ai_anteil":["Euria 20%","Claude 20%"],"created":"2026-05-23","updated":"2026-05-23","status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/0-final-check/html-hypertext-markup-language/","dgPassFrontmatter":true,"dg-note-properties":{"title":"HTML (Hypertext Markup Language)","aliases":["HTML"],"tags":null,"gen_ai_anteil":["Euria 20%","Claude 20%"],"created":"2026-05-23","updated":"2026-05-23","status":null}}
---


# HTML (Hypertext Markup Language)

HTML ist die grundlegende Auszeichnungssprache (engl. „Markup Language“) für das World Wide Web. Das bedeutet: Text wird durch Tags (Markierungen) wie zum Beispiel `<h1>` „ausgezeichnet“.

Hier ein Beispiel für HTML-Code:

```HTML
<h1>Ich bin die Hauptüberschrift</h1>
<p>Ich bin ein Fließtext und enthalte einen <a href="https://google.com">Link zu Google</a></p>
```

So teilen wir dem Browser mit, wie die Seite aufgebaut ist: Was sind Überschriften, was sind Links, was ist Fließtext?

Für das Design ist HTML nicht zuständig, dafür brauchen wir zusätzlich [[02 - Künstliche Intelligenz/0 - Final Check/CSS (Cascading Style Sheets)\|CSS]].

Ohne CSS würden alle Seiten immer noch so aussehen wie Anfang der 90er, in den frühen Tagen des Webs:

![Website ohne CSS.png](/img/user/02%20-%20K%C3%BCnstliche%20Intelligenz/Garten%20erkunden/Bilder/Website%20ohne%20CSS.png)

## Hypertext

Das „HT“ in HTML steht für **Hypertext**. Das ist Text, der Verlinkungen zu anderen Texten (oder Ressourcen) enthält.

Die Idee ist älter als das Internet – schon in den 1960ern wurden Konzepte entwickelt, um Dokumente durch Links miteinander zu verbinden. Das World Wide Web ist heute der bekannteste Anwendungsfall davon.

![Hypertext vs Buch.png](/img/user/02%20-%20K%C3%BCnstliche%20Intelligenz/Garten%20erkunden/Bilder/Hypertext%20vs%20Buch.png)

### Hypertext, das Internet und das WWW

Umgangssprachlich verschwimmen die Grenzen zwischen diesen Begriffen oft, aber lass uns einen Augenblick innehalten und die genauen Definitionen betrachten:

**Hypertext** = ein Konzept für Text, der Verlinkungen zu anderen Texten enthält.

**World Wide Web** = ein über das Internet abrufbares System von Webseiten. Webseiten sind Hypertext-Dokumente, die in HTML geschrieben und über eine Adresse (URL) erreichbar sind.

**Internet** = das weltweite Netzwerk aus miteinander verbundenen Computern. Die physische und technische Infrastruktur, auf der verschiedene Dienste laufen, wie das World Wide Web, E-Mail, Streaming und Cloud-Gaming.

> [!info] Was genau ist mit Internet gemeint?
>
> Streng genommen ist damit nur die Infrastruktur gemeint, aber im allgemeinen Sprachgebrauch meinen Menschen damit natürlich das Gesamtpaket: Infrastruktur inklusive aller Dienste, die darauf laufen.

![Internet vs Web.png](/img/user/02%20-%20K%C3%BCnstliche%20Intelligenz/Garten%20erkunden/Bilder/Internet%20vs%20Web.png)

## Markup Language

Eine **Markup Language** (**Auszeichnungssprache**) ist eine Sprache für den Computer, die Texten eine **Bedeutung** oder eine **Struktur** verleiht.

Man kann sie sich wie einen Korrekturstift vorstellen, mit dem ein Lektor auf einem Manuskript Notizen macht: „Das hier ist eine Überschrift“ oder „Hier beginnt ein neues Kapitel“. In der digitalen Welt passiert das durch **Tags** (Markierungen).

Noch mal zu unserem Beispiel von oben:

```HTML
<h1> Ich bin die Hauptüberschrift</h1>
<p> Ich bin ein Fließtext und enthalte einen <a href="https://google.com">Link zu Google</a></p>
```

`<h1>`, `<p>` und `<a>` sind die Tags, und sie markieren den Text, welchen sie umschließen. Dafür treten sie meist paarweise auf: Das Start-Tag (`<h1>`) öffnet, das End-Tag mit Schrägstrich (`</h1>`) schließt wieder.

`<h1>` kennzeichnet die Hauptüberschrift (die oberste Gliederungsebene),
`<p>` bedeutet „Absatz“ (von engl. „paragraph“), und
`<a>` markiert einen Link. Der Zusatz `href="…"` bestimmt, wohin der Link führt.

## HTML betrifft wirklich nur die Struktur, nicht das Design

HTML legt ausschließlich die Struktur fest. `<h1>` bedeutet also nur: Das ist die oberste Ebene der Gliederung. Mit anderen Worten: `<h1>` sagt nicht „größte Überschrift“, sondern „*wichtigste* Überschrift“.

Diese Gliederung hilft zum Beispiel blinden und sehbehinderten Menschen, die sich Webseiten von einem Screenreader vorlesen lassen: Sie können so von Überschrift zu Überschrift springen und bekommen schnell einen Überblick, ähnlich wie beim Überfliegen eines Textes.

Wenn es nicht ums Aussehen geht - wie kommt es dann, dass in unserem Beispiel von oben die Überschrift groß und fett dargestellt wird? Das liegt nicht an HTML, sondern an den Standardeinstellungen des Browsers: Er gibt jedem Element eine Grundgestaltung mit, solange nichts anderes festgelegt ist. Deshalb sieht eine Website ohne CSS auch heute noch so aus wie in den frühen 90ern. Mit CSS können wir das nach Belieben ändern.

In der Praxis gestalten wir die `<h1>` meist trotzdem als größte Überschrift, weil das der Orientierung hilft. Notwendig ist das aber nicht.

So könnte unser Beispiel von oben aussehen, wenn wir es mit CSS eigenwillig gestalten:

![Website mit eigenwilligem CSS.png](/img/user/02%20-%20K%C3%BCnstliche%20Intelligenz/Garten%20erkunden/Bilder/Website%20mit%20eigenwilligem%20CSS.png)

Damit würden wir Sehende wahrscheinlich verwirren. Menschen, die einen Screenreader verwenden, bemerken davon dagegen nichts: Der Screenreader kündigt „Ich bin die Hauptüberschrift“ weiterhin als Überschrift der obersten Ebene an und den Link als Link. Genau das meint die Trennung von Struktur und Design: HTML sagt, _was_ etwas ist, CSS sagt, _wie_ es aussieht.

👉 Wer neugierig geworden ist, kann sich hier angucken, wie das [[02 - Künstliche Intelligenz/0 - Final Check/CSS (Cascading Style Sheets)#Ein eigenwilliges Beispiel\|CSS hinter unserem Beispiel]] aussieht.
## 📖 Weiterlesen

- Ein Artikel über HTML, der Tim Berners-Lee nicht erwähnt, ist eigentlich unvollständig: Er hat HTML und das World Wide Web erfunden. Wie es dazu kam, steht in der [[02 - Künstliche Intelligenz/3 - Work on tomorrow/Eine kurze Geschichte des Internets\|kurzen Geschichte des Internets]].
- Ein Hypertext-System muss nicht digital sein. Der [[02 - Künstliche Intelligenz/2 - Work on today/Zettelkasten und Hypertext\|Zettelkasten]] ist ein analoges Beispiel.
- Mehr über [[02 - Künstliche Intelligenz/0 - Final Check/CSS (Cascading Style Sheets)\|CSS]], die „Design-Sprache“ des Webs