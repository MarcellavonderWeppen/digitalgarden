---
{"title":"Möglichkeiten, sich gegen Crawler zu wehren","aliases":null,"tags":null,"gen_ai_anteil":["Claude 100%"],"created":"2026-10-01","updated":null,"status":null,"dg-publish":true,"permalink":"/moeglichkeiten-sich-gegen-crawler-zu-wehren/","dgPassFrontmatter":true,"dg-note-properties":{"title":"Möglichkeiten, sich gegen Crawler zu wehren","aliases":null,"tags":null,"gen_ai_anteil":["Claude 100%"],"created":"2026-10-01","updated":null,"status":null}}
---


# Möglichkeiten, sich gegen Crawler zu wehren

Wer eine Website betreibt, kann [[02 - Künstliche Intelligenz/0 - Final Check/Crawler\|Crawlern]] den Zugang verwehren oder zumindest erschweren. Dieser Artikel gibt einen Überblick über die wichtigsten Möglichkeiten. Für die konkrete Umsetzung lohnt sich ein Blick in die Hilfe des eigenen Hosters oder Website-Baukastens.

Die Gründe, Crawler aussperren zu wollen, sind unterschiedlich:

- **Urheberrecht und Einwilligung:** Viele möchten nicht, dass ihre Texte, Bilder oder Fotos ungefragt zum Training von KI-Modellen genutzt werden.
- **Serverlast und Kosten:** Manche Crawler rufen in kurzer Zeit sehr viele Seiten ab. Das kann eine Website ausbremsen und gerade kleinen Betreibern spürbare Kosten verursachen.
- **Wenig Gegenleistung:** Suchmaschinen schicken Besucher zurück, wenn sie eine Seite in ihren Ergebnissen zeigen. Bei KI-Anwendungen steht die Antwort oft schon im Chat, und nur wenige Nutzer klicken sich noch zur Quelle durch.
- **Kontrolle:** Man möchte grundsätzlich selbst bestimmen, was mit den eigenen Inhalten geschieht.

> [!info] Drei Stufen
> Die Möglichkeiten lassen sich grob in drei Stufen einteilen: **bitten**, **aussperren** und **zurückschlagen**.

## Auf den guten Willen setzen

Auf dieser Stufe hinterlässt man einen Hinweis, was man möchte und was nicht. Ob sich ein Crawler daran hält, entscheidet er selbst.

### robots.txt

Das bekannteste Mittel ist die robots.txt, eine Textdatei im Hauptverzeichnis der Website. Wie sie funktioniert, steht im Artikel [[02 - Künstliche Intelligenz/0 - Final Check/Crawler#Muss denn das sein?\|Crawler]].

### Weitere maschinenlesbare Hinweise

Daneben gibt es weitere Wege, Wünsche so zu hinterlegen, dass Maschinen sie lesen können:

- **Meta-Tags:** kurze Anweisungen im Quellcode einer einzelnen Seite, die Besucher nicht sehen. Etabliert ist zum Beispiel „noindex“: Die Seite soll nicht in Suchergebnissen auftauchen. Für KI gibt es Vorschläge wie „noai“, die aber kein offizieller Standard sind und nur von wenigen Anbietern beachtet werden.
- **Nutzungsvorbehalte:** spezielle Formate, mit denen man ausdrücklich erklärt, dass Inhalte nicht automatisiert ausgewertet werden dürfen (Fachbegriff: Text- und Data-Mining). Ein Beispiel ist das „TDM Reservation Protocol“, entwickelt in einer Arbeitsgruppe des W3C (World Wide Web Consortium), das Standards für das Web erarbeitet.
- **Neue Standards in Arbeit:** Die IETF (Internet Engineering Task Force), die viele grundlegende Internetstandards entwickelt, arbeitet an einem einheitlichen Vokabular für KI-Nutzungswünsche, etwa „nicht für KI-Training“. Es soll sich in die robots.txt schreiben oder beim Abruf einer Seite mitschicken lassen. Fertig ist es noch nicht (Stand: Oktober 2026).

Auch wenn all das freiwillig ist: In der EU hat ein maschinenlesbarer Widerspruch rechtliches Gewicht, mehr dazu unter [[02 - Künstliche Intelligenz/0 - Final Check/Crawler#Mehr als ein freundlicher Hinweis\|Mehr als ein freundlicher Hinweis]].

## Technisch aussperren

Auf dieser Stufe kommt es nicht mehr auf den guten Willen des Crawlers an: Er bekommt die Inhalte schlicht nicht.

### Blockieren

Jeder Besucher, ob Mensch oder Bot, schickt eine Anfrage an den Server, auf dem die Website liegt. Der Server kann Anfragen abweisen, zum Beispiel:

- **nach Name:** Crawler nennen bei jeder Anfrage einen Namen (Fachbegriff: User-Agent). Der Server kann bestimmte Namen ablehnen. Anders als bei der robots.txt entscheidet hier der Server, nicht der Crawler.
- **nach Herkunft:** Anfragen von bestimmten IP-Adressen (den „Hausnummern“ von Geräten im Internet) werden gesperrt, etwa bekannte Adressbereiche von KI-Firmen.
- **nach Verhalten:** Wer in kurzer Zeit auffällig viele Seiten abruft, wird gebremst oder ausgesperrt (Fachbegriff: Rate Limiting).
- **per Rechenaufgabe:** Werkzeuge wie Anubis lassen jeden Browser vor dem Zugang eine kleine Rechenaufgabe lösen. Für einen einzelnen Besucher ist das kaum spürbar, für einen Crawler, der Millionen Seiten abruft, wird es teuer.

Die Grenze: Namen lassen sich fälschen, IP-Adressen wechseln. Je besser sich ein Crawler tarnt, desto schwerer ist er zu erkennen.

Viele Betreiber überlassen diese Arbeit daher **Dienstleistern** wie Cloudflare, die zwischen Website und Besuchern geschaltet werden und Bots mit großem Aufwand erkennen. Cloudflare sperrt KI-Crawler für neue Websites inzwischen teilweise schon standardmäßig und bietet an, von KI-Firmen Geld für den Zugriff zu verlangen (Stand: Oktober 2026). Der Preis: Man macht sich von einem großen Anbieter abhängig, über den ohnehin schon ein erheblicher Teil des Webverkehrs läuft.

### Verstecken

Was nicht öffentlich erreichbar ist, kann auch kein Crawler einsammeln.

- **Login:** Inhalte sind nur für angemeldete Nutzer sichtbar.
- **Paywall:** Inhalte gibt es nur gegen Bezahlung. Achtung: Manche Paywalls verdecken Texte nur optisch. Im Quellcode stehen sie trotzdem und sind für Crawler lesbar.
- **CAPTCHAs:** kleine Tests, die Menschen von Maschinen unterscheiden sollen („Klicke alle Bilder mit Ampeln an“). Moderne KI löst viele davon inzwischen allerdings selbst.

Der Preis: Die Hürden treffen auch Menschen. Versteckte Inhalte tauchen zudem nicht mehr in Suchmaschinen auf. Und CAPTCHAs, aber auch Rechenaufgaben, die JavaScript oder ein schnelles Gerät voraussetzen, können für Menschen mit Behinderung oder ältere Technik zur echten Barriere werden.

## Zurückschlagen

Auf dieser Stufe bekommt der Crawler nicht nichts, sondern etwas Falsches. Das Ziel ist weniger, die eigenen Inhalte zu schützen, als dem Crawler Kosten zu verursachen. Gemeint sind vor allem Crawler, die Hinweise wie die robots.txt ignorieren.

- **Labyrinthe:** Der Crawler wird über unsichtbare Links in ein endloses Geflecht automatisch erzeugter Seiten gelockt, die immer weiter aufeinander verweisen. Dort verschwendet er Zeit und Rechenleistung und sammelt wertlosen Text ein (Fachbegriff: Tarpit, Teergrube). Bekannt ist das frei verfügbare Werkzeug Nepenthes, benannt nach einer fleischfressenden Kannenpflanze. Cloudflare bietet mit „AI Labyrinth“ eine Variante an, die nur verdächtigen Bots gezeigt wird und gleichzeitig dabei hilft, sie zu erkennen.
- **Vergiftete Inhalte:** Werkzeuge wie Nightshade verändern Bilder für Menschen unsichtbar so, dass KI-Modelle beim Training falsche Zusammenhänge lernen, etwa einen Hund für eine Katze halten.

**Was es bringt:** Gegen große, professionelle Crawler vermutlich wenig. Sie begrenzen, wie tief sie sich durch eine Website klicken, und filtern ihre Trainingsdaten. Forscher haben zudem ein Verfahren vorgestellt, das mit Nightshade veränderte Bilder fast immer erkennt und bereinigt. Eine spürbare Wirkung entsteht wohl erst, wenn sehr viele Websites mitmachen.

**Was es kostet:**
- **Serverlast:** Wer ein Labyrinth selbst betreibt, belastet damit auch den eigenen Server.
- **Kollateralschäden:** Ist die Falle schlecht eingestellt, verfangen sich auch Suchmaschinen oder Archiv-Crawler darin. Die Website kann dann in der Suche leiden.
- **Barrierefreiheit:** Werden Menschen fälschlich als Bot eingestuft oder lesen Screenreader die versteckten Links vor, landen auch sie im Labyrinth.

**Perspektiven:** Befürworter sehen darin legitime Gegenwehr gegen Crawler, die sich über die Wünsche von Betreibern hinwegsetzen. Wenn rücksichtsloses Crawlen teurer wird, so das Argument, lohnt es sich weniger. Kritiker halten dagegen, dass dabei auf beiden Seiten Energie und Rechenleistung verschwendet werden, Unbeteiligte getroffen werden können und am Ende ein Wettrüsten steht, das vor allem große Anbieter gewinnen.

## Fazit: Keinen hundertprozentigen Schutz

In der Praxis kombinieren Betreiber oft mehrere Maßnahmen. Dabei gilt: Je stärker der Schutz, desto größer der Aufwand und die Nebenwirkungen. Und was ein Crawler bereits eingesammelt hat, holt keine Maßnahme zurück.

Hinzu kommt ein **Zielkonflikt:** Wer KI-Crawler aussperrt, taucht womöglich auch in KI-gestützten Suchen nicht mehr auf, etwa in ChatGPT, Claude oder Perplexity. Einige Anbieter betreiben deshalb getrennte Crawler fürs Training und für die Suche, sodass man das eine erlauben und das andere verbieten kann. Bei Google ist das nur teilweise möglich: Fürs Gemini-Training lässt sich ein eigener Widerspruch einlegen. Die KI-Übersichten in der Google-Suche speisen sich aber aus demselben Crawler wie die normale Suche. Wer dort nicht auftauchen möchte, muss Einschränkungen in der klassischen Suche in Kauf nehmen.
