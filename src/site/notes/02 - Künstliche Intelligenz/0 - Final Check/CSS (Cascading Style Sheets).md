---
{"title":"CSS (Cascading Style Sheets)","aliases":["CSS"],"tags":null,"gen_ai_anteil":["Euria 20%","Claude 20%"],"created":"2026-05-23","updated":"2026-05-24","status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/0-final-check/css-cascading-style-sheets/","dgPassFrontmatter":true,"dg-note-properties":{"title":"CSS (Cascading Style Sheets)","aliases":["CSS"],"tags":null,"gen_ai_anteil":["Euria 20%","Claude 20%"],"created":"2026-05-23","updated":"2026-05-24","status":null}}
---


# CSS (Cascading Style Sheets)

CSS ist das schicke Geschwisterchen von [[02 - Künstliche Intelligenz/0 - Final Check/HTML (Hypertext Markup Language)\|HTML]]. Es ist für das Design von Webseiten zuständig.

Ohne CSS würde das gesamte Internet noch immer wie Anfang der 90er aussehen:

![Website without HTML 2.png](/img/user/02%20-%20K%C3%BCnstliche%20Intelligenz/Garten%20erkunden/Bilder/Website%20without%20HTML%202.png)

Gut, dass wir CSS erfunden haben!

Übrigens: Dieses Beispiel ist nicht ausgedacht. Es ist die allererste Website der Welt, und man kann sie bis heute besuchen: [info.cern.ch](https://info.cern.ch/hypertext/WWW/TheProject.html). Sir [[02 - Künstliche Intelligenz/1 - Work on now/Eine kurze Geschichte des Internets#Das World Wide Web Ein Geschenk an die Welt\|Tim Berners-Lee]] hat sie Anfang der 90er am CERN online gestellt und damit der Welt das World Wide Web geschenkt. 
## Ein einfaches Beispiel für CSS

So könnte eine CSS-Regel aussehen:

```css
h1 {
  color: blue;
  font-size: 20px;
}
```

Das bedeutet: „Mache alle Hauptüberschriften (`h1`) blau und gib ihnen eine Größe von 20 Pixeln.“
## Warum zwei Sprachen?

An diesem Punkt stellt sich dem aufmerksamen Leser vielleicht die Frage: Wozu zwei Sprachen - HTML _und_ CSS? Hätte man nicht auch eine Sprache erfinden können, die alles kann?

Gute Frage!

Tatsächlich war es anfangs genau so: Bevor es CSS gab, wurde das Aussehen direkt ins HTML geschrieben. Eine blaue Überschrift sah dann zum Beispiel so aus: `<h1><font color="blue">Überschrift</font></h1>`.

Das funktioniert, hat aber einen gewaltigen Haken.

Man stelle sich eine Webseite mit hunderten Unterseiten vor. Jede Unterseite hat eine große blaue Überschrift wie in unserem Beispiel. Nun entscheidet der Besitzer der Website: Die Überschriften sollen rot sein!

Steckt das Aussehen direkt im HTML, müssten wir nun auf hunderten Seiten von Hand die Überschrift von blau auf rot umstellen.

Aber zum Glück gibt es CSS!

Eine einzige CSS-Datei kann mit beliebig vielen Unterseiten verknüpft sein.

Wir ändern nur diese eine CSS-Regel:

```css
h1 {
  color: red;
  font-size: 20px;
}
```

Fertig! Genau deshalb ist die Trennung von Struktur und Aussehen ein genialer Schachzug.
## Ein eigenwilliges Beispiel

Farbe und Größe sind natürlich erst der Anfang. Mit CSS lässt sich noch viel mehr anstellen. Im Artikel über [[02 - Künstliche Intelligenz/0 - Final Check/HTML (Hypertext Markup Language)\|HTML]] haben wir unserem Beispiel ein ziemlich eigenwilliges Aussehen verpasst:

![Website mit eigenwilligem CSS.png](/img/user/02%20-%20K%C3%BCnstliche%20Intelligenz/Garten%20erkunden/Bilder/Website%20mit%20eigenwilligem%20CSS.png)

Hier noch einmal das HTML zu unserem Beispiel: 

```html
<h1>Ich bin die Hauptüberschrift</h1>
<p>Ich bin ein Fließtext und enthalte einen <a href="https://google.com">Link zu Google</a></p>
```

Und so sieht das CSS dahinter aus:

```css
h1 {
  font-size: 14px;              /* winzig statt riesig */
  text-transform: uppercase;    /* in Großbuchstaben */
  letter-spacing: 4px;          /* mit viel Luft zwischen den Buchstaben */
  color: crimson;               /* in kräftigem Rot */
}

p {
  font-size: 24px;              /* größer als die Überschrift! */
  font-family: Georgia, serif;  /* in einer Schrift mit Serifen */
  line-height: 1.5;             /* mit etwas mehr Zeilenabstand */
}

a {
  color: black;                 /* schwarz statt blau */
  text-decoration: none;        /* ohne Unterstreichung */
  background-color: yellow;     /* dafür wie mit Textmarker hervorgehoben */
  padding: 0 2px;               /* mit etwas Luft links und rechts */
}
```

Alles zwischen `/*` und `*/` sind Kommentare: Notizen für Menschen, die der Browser einfach ignoriert.
## Aber es gibt doch auch noch JavaScript…?

Psst! 🤫

Ganz richtig. HTML gibt der Seite Struktur, CSS ein schickes Aussehen und JavaScript ist für die Interaktivität zuständig.

Aber das sprengt jetzt den Umfang dieses Digitalen Gartens.

Wenn Du bis hierher gelesen hast, solltest Du vielleicht Dein eigenes Abenteuer starten und Dich mit Programmierung befassen.

Hier habe ich vor vielen Jahren mein Programmier-Abenteuer gestartet 👇

https://www.codecademy.com/ 🕳️ 🐇