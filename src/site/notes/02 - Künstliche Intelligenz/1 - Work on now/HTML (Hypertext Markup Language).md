---
{"title":"HTML (Hypertext Markup Language)","aliases":["HTML"],"tags":null,"gen_ai_anteil":["Euria 20%","Claude 20%"],"created":"2026-05-23","updated":"2026-05-23","status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/1-work-on-now/html-hypertext-markup-language/","dgPassFrontmatter":true,"dg-note-properties":{"title":"HTML (Hypertext Markup Language)","aliases":["HTML"],"tags":null,"gen_ai_anteil":["Euria 20%","Claude 20%"],"created":"2026-05-23","updated":"2026-05-23","status":null}}
---


# HTML (Hypertext Markup Language)

HTML ist die grundlegende Auszeichnungssprache (engl. „Markup Language“) für das World Wide Web. Das bedeutet: Text wird durch Tags (Markierungen) wie zum Beispiel `<h1>` „ausgezeichnet“.

Hier ein Beispiel für HTML-Code:

```HTML
<h1> Ich bin die Hauptüberschrift</h1>
<p> Ich bin ein Fließtext und enthalte einen <a href="https://google.com">Link zu Google</a></p>
```

So teilen wir dem Browser mit, wie die Seite aufgebaut ist: Was sind Überschriften, was sind Links, was ist Fließtext?

Für das Design ist HTML nicht zuständig, dafür brauchen wir zusätzlich [[02 - Künstliche Intelligenz/5 - soon (veröffentlicht)/CSS (Cascading Style Sheets)\|CSS]].

Ohne CSS würden alle Seiten immer noch so aussehen wie Anfang der 90er, in den frühen Tagen des Webs:

![Website ohne CSS.png](/img/user/02%20-%20K%C3%BCnstliche%20Intelligenz/Garten%20erkunden/Bilder/Website%20ohne%20CSS.png)

## Hypertext

Das „HT“ in HTML steht für **Hypertext**. Das ist Text, der Verlinkungen zu anderen Texten (oder Ressourcen) enthält.

Die Idee ist älter als das Internet – schon in den 1960ern wurden Konzepte entwickelt, um Dokumente durch Links miteinander zu verbinden. Das World Wide Web ist heute der bekannteste Anwendungsfall davon.

### Hypertext, das Internet und das WWW

Umgangssprachlich verschwimmen die Grenzen zwischen diesen Begriffen oft, aber lass uns einen Augenblick innehalten und die genauen Definitionen betrachten:

**Hypertext** = Konzept für Text, der Verlinkungen zu anderen Texten enthält

**World Wide Web** = über das Internet abrufbares System von Hypertext-Dokumenten (also Webseiten), die in HTML geschrieben und über eine Adresse (URL) erreichbar sind

**Internet** = Das weltweite Netzwerk aus miteinander verbundenen Computern. Die physische und technische Infrastruktur, auf der verschiedene Dienste laufen, wie das World Wide Web, E-Mail, Streaming und Cloud-Gaming

> [!info] Was genau ist mit Internet gemeint?
>
> Streng genommen ist damit nur die Infrastruktur gemeint, aber im allgemeinen Sprachgebrauch meinen Menschen damit natürlich das Gesamtpaket: Infrastruktur inklusive aller Dienste, die darauf laufen.

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
`<a>` wird verwendet, um Links zu markieren (von engl. „anchor“, Anker). Der Zusatz `href="…"` bestimmt, wohin der Link führt.

## HTML betrifft wirklich nur die Struktur, nicht das Design

Die Größe unserer `<h1>`-Überschrift ist übrigens schon Design, und zwar die Standardgestaltung des Browsers: Jeder Browser stellt Überschriften von sich aus groß und fett dar, Links blau und unterstrichen. Das können wir mit CSS nach Belieben ändern. Für HTML zählt allein, dass es sich um die oberste Ebene der Gliederung handelt.

Mit anderen Worten: `<h1>` sagt nicht „größte Überschrift“, sondern „*wichtigste* Überschrift“. Klar – wahrscheinlich werden wir sie mittels CSS als größte Überschrift gestalten; notwendig ist das aber nicht. 

Wichtig ist diese Gliederung zum Beispiel für Menschen, die sich Webseiten mit einem Screenreader vorlesen lassen: Sie können so von Überschrift zu Überschrift springen und bekommen schnell einen Überblick, und bekommen schnell einen Überblick, so wie Sehende einen Text überfliegen.

## 📖 Weiterlesen

- Mehr über [[02 - Künstliche Intelligenz/5 - soon (veröffentlicht)/CSS (Cascading Style Sheets)\|CSS (Cascading Style Sheets)]], die „Design-Sprache“ des Webs
- Ein Artikel über HTML, der Tim Berners-Lee nicht erwähnt, ist eigentlich unvollständig. Für alle, die mehr wissen wollen, hier eine [[02 - Künstliche Intelligenz/2 - Work on today/Eine sehr kurze Geschichte des Internets\|sehr kurze Geschichte des Internets]].
