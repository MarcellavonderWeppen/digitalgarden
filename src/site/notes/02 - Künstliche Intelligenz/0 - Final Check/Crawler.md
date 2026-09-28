---
{"title":"Crawler","aliases":null,"tags":null,"gen_ai_anteil":["Mistral 100%"],"created":"2026-06-03","updated":null,"status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/0-final-check/crawler/","dgPassFrontmatter":true,"dg-note-properties":{"title":"Crawler","aliases":null,"tags":null,"gen_ai_anteil":["Mistral 100%"],"created":"2026-06-03","updated":null,"status":null}}
---

# Crawler

**Crawler** (auch **Webcrawler** oder **Spider** genannt) sind **automatisierte Programme**, die das World Wide Web systematisch durchsuchen, um Webseiten zu finden und herunterzuladen.

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

Website-Betreiber können Crawler von Teilen oder ihrer gesamten Seite ausschließen. Dafür legen sie eine Textdatei namens **robots.txt** an, in der steht, welcher Crawler wohin darf und wohin nicht.

Seriöse Crawler halten sich daran; technisch erzwingen lässt sich das allerdings nicht. Es ist eher eine Bitte als ein Schloss.


