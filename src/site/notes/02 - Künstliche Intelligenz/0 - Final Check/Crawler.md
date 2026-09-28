---
{"title":"Crawler","aliases":null,"tags":null,"gen_ai_anteil":["Mistral 100%"],"created":"2026-06-03","updated":null,"status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/0-final-check/crawler/","dgPassFrontmatter":true,"dg-note-properties":{"title":"Crawler","aliases":null,"tags":null,"gen_ai_anteil":["Mistral 100%"],"created":"2026-06-03","updated":null,"status":null}}
---

# Crawler

**Crawler** (auch unter dem Namen **Webcrawler**, **Spider** oder **Bot** bekannt) sind **automatisierte Programme**, die das World Wide Web systematisch durchsuchen, um Webseiten zu finden und herunterzuladen.

Sie bilden die Grundlage für Suchmaschinen wie Google oder Bing, aber auch für Datensammlungen wie Common Crawl, die als Trainingsdaten für große Sprachmodelle dienen.

## Was Crawler tun

- **Entdecken:** Sie folgen Links von Seite zu Seite und erkunden so das Web.
- **Speichern:** Sie legen die Inhalte (Texte, Metadaten, manchmal auch Bilder oder andere Medien) ab, damit sie weiterverarbeitet werden können, etwa von einer Suchmaschine, die sie indiziert und durchsuchbar macht.
- **Aktualisieren:** Sie kehren regelmäßig zu bereits besuchten Seiten zurück, um Änderungen oder neue Inhalte zu erfassen.

Crawler sind also das **Werkzeug**, um große Mengen an Webinhalten für Suchmaschinen oder Trainingsdaten zu sammeln.

## So arbeitet ein Crawler

Ein Crawler startet auf einer Webseite, liest deren Inhalt, extrahiert alle Links und fügt diese zu einer Warteschlange hinzu. Dann besucht er die nächsten Seiten in dieser Warteschlange – und wiederholt den Prozess.

So entsteht eine automatisierte, breite Erfassung des [[02 - Künstliche Intelligenz/Garten erkunden/Grundlagen/Das Internet - Surface Web, Deep Web und Dark Web#Surface Web – Die Spitze des Eisbergs\|Surface Web]].

## Muss denn das sein?

Website-Betreiber können Crawler von Teilen oder ihrer gesamten Seite ausschließen. Dafür legen sie im Hauptverzeichnis ihrer Website eine Textdatei namens robots.txt an (also unter `meine-website.de/robots.txt`), in der steht, welcher Crawler wohin darf und wohin nicht.

### Beispiel für ein robots.txt

```
User-agent: *
Disallow: /

User-agent: Googlebot
Allow: /
```

Hier werden alle Crawler von der gesamten Seite ausgeschlossen (`*` steht für „alle“, `/` für „die ganze Seite“).

Damit wäre allerdings auch der Googlebot ausgesperrt, und die Seite würde nicht mehr in der Google-Suche auftauchen. Deshalb bekommt er im zweiten Block eine Ausnahme: Er darf wieder rein.

Seriöse Crawler halten sich daran; technisch erzwingen lässt sich das allerdings nicht. 

Der Server kontrolliert nämlich nichts; der Crawler muss die robots.txt selbst lesen und sich freiwillig daran halten. Und wer da anklopft, lässt sich nicht einmal sicher sagen: Jeder Crawler gibt sich seinen Namen selbst und kann sich genauso gut als ganz normaler Browser ausgeben.

Rechtlich ist die robots.txt trotzdem mehr als ein freundlicher Hinweis. In der EU dürfen öffentlich zugängliche Inhalte grundsätzlich automatisiert ausgewertet werden (Fachbegriff: Text- und Data-Mining), auch fürs KI-Training. Es sei denn, wer die Rechte daran hat, widerspricht, und zwar so, dass eine Maschine den Widerspruch lesen kann. Ob dafür ein Satz in normaler Sprache genügt, zum Beispiel in den Nutzungsbedingungen, ist umstritten; die robots.txt gilt als der sicherste Weg.[^laion]


[^laion]: Ein Fotograf klagte gegen den gemeinnützigen Verein LAION, der Datensätze für KI-Training zusammenstellt. LAION hatte 2021 eines seiner Fotos heruntergeladen, um zu prüfen, ob Bild und Beschreibung zusammenpassen. Die Website, auf der das Foto stand, hatte der automatisierten Nutzung nur in ihren Nutzungsbedingungen widersprochen. Das OLG Hamburg urteilte im Dezember 2025 (Az. 5 U 104/24): Beim Download 2021 konnten Maschinen so einen Satz in normaler Sprache noch nicht zuverlässig lesen, der Widerspruch zählte also nicht. Es ist unklar, wie die Lage heute aussieht; inzwischen können Maschinen auch normale Sprache verstehen.