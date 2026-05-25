---
{"title":"HTML (Hypertext Markup Language)","aliases":["HTML"],"tags":null,"gen-ai-anteil":["Euria 20%","Claude 20%"],"created":"23.05.2026","updated":"2026-05-23","status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/2-veroeffentlicht/html-hypertext-markup-language/","dgPassFrontmatter":true,"dg-note-properties":{"title":"HTML (Hypertext Markup Language)","aliases":["HTML"],"tags":null,"gen-ai-anteil":["Euria 20%","Claude 20%"],"created":"23.05.2026","updated":"2026-05-23","status":null}}
---

# HTML (Hypertext Markup Language) 

HTML ist die grundlegende Auszeichnungssprache (engl. “Markup Language”) für das World Wide Web. Das bedeutet: Text wird durch Tags (Markierungen) wie zum Beispiel `<h1>` “ausgezeichnet”.

Hier ein Beispiel für den Code:

```HTML
<h1> Ich bin eine große h1-Überschrift</h1>
<p> Ich bin ein Fließtext und enthalte einen <a href="https://google.com">Link zu Google</a></p>
``` 

Der Browser wird über die Struktur der Seite informiert: Was sind Überschriften, was sind Links, was ist Fließtext? 

Über das Design kann HTML keine Auskunft geben, dafür brauchen wir zusätzlich [[02 - Künstliche Intelligenz/2- Veröffentlicht/CSS (Cascading Style Sheets)\|CSS]].

Ohne CSS würden alle Seiten immer noch wie beim Aufkommen des Internets in den 90ern aussehen: 

![Website ohne HTML 1.png](/img/user/02%20-%20K%C3%BCnstliche%20Intelligenz/1%20-%20Work%20on%20next/Bilder/Website%20ohne%20HTML%201.png)

## Hypertext 

Das „HT“ in HTML steht für **Hypertext**. Das ist Text, der Verlinkungen zu anderen Texten (oder Ressourcen) enthält.

Das Konzept ist älter als das Internet – schon in den 1960ern wurde die Idee entwickelt, Dokumente durch Links miteinander zu verbinden. Das World Wide Web ist heute der bekannteste Anwendungsfall davon.

### Hypertext, das Internet und das WWW

Umgangssprachlich verschwimmen die Grenzen zwischen diesen Begriffen oft, aber lass uns einen Augenblick innehalten und die genauen Definitionen betrachten: 

**Hypertext** = Konzept für Text, der Verlinkungen zu anderen Texten enthält

---
**World Wide Web** = über das Internet abrufbares System von elektronischen Hypertext-Dokumenten (also Websites), welche in HTML geschrieben sind.

---

**Internet** = Das weltweite Netzwerk aus miteinander verbundenen Computern.  Die physische und technische Infrastruktur, auf der verschiedene Dienste laufen, wie das World Wide Web, E-Mail, Streaming und Cloud-Gaming.

> [!info] Was genau ist mit Internet gemeint?
> 
> Streng genommen ist damit tatsächlich nur die physische Infrastruktur gemeint, aber im allgemeinen Sprachgebrauch meinen Menschen damit natürlich das Gesamtpaket - Infrastrukur inklusive aller Dienste, die darauf laufen.

## Markup Language

Eine **Markup Language** (**Auszeichnungssprache**) ist eine Sprache für den Computer, die Texten eine **Bedeutung** oder eine **Struktur** verleiht.

Man kann sie sich wie einen Korrekturstift vorstellen, mit dem ein Lektor auf einem Manuskript Notizen macht:  „Das hier ist eine Überschrift“ oder „Hier beginnt ein neues Kapitel“. In der digitalen Welt passiert das durch **Tags** (Markierungen).

Noch mal zu unserem Beispiel von oben: 

```HTML
<h1> Ich bin eine große h1-Überschrift</h1>
<p> Ich bin ein Fließtext und enthalte einen <a href="https://google.com">Link zu Google</a></p>
``` 

`<h1>`, `<p>`und `<a>`sind die Tags, und sie markieren den Text, welchen sie umschließen.

`<h1>` kennzeichnet die größte Überschrift, 
`<p>` bedeutet “Absatz” (von engl. “paragraph”), und 
`<a>` wird verwendet um Links zu markieren.

📖 Weiterlesen: [[02 - Künstliche Intelligenz/2- Veröffentlicht/CSS (Cascading Style Sheets)\|CSS (Cascading Style Sheets)]]