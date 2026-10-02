---
{"title":"Crawler","aliases":["Webcrawler","Spider","Bot"],"tags":null,"gen_ai_anteil":["Mistral 20%","Claude 20%"],"created":"2026-06-03","updated":"2026-10-01","status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/garten-erkunden/grundlagen/crawler/","dgPassFrontmatter":true,"dg-note-properties":{"title":"Crawler","aliases":["Webcrawler","Spider","Bot"],"tags":null,"gen_ai_anteil":["Mistral 20%","Claude 20%"],"created":"2026-06-03","updated":"2026-10-01","status":null}}
---

# Crawler

> [!info] Synonyme: Webcrawler, Spider oder Bot 

**Crawler** sind **automatisierte Programme**, die das World Wide Web systematisch durchsuchen, um Webseiten zu finden und herunterzuladen.

Sie bilden die Grundlage für Suchmaschinen wie Google oder Bing, aber auch für Datensammlungen wie Common Crawl, die als Trainingsdaten für große Sprachmodelle dienen.

## Was Crawler tun

- **Entdecken:** Sie folgen Links von Seite zu Seite und erkunden so das Web.
- **Speichern:** Sie legen die Inhalte (Texte, Metadaten, manchmal auch Bilder oder andere Medien) ab, damit sie weiterverarbeitet werden können, etwa von einer Suchmaschine, die sie indiziert und durchsuchbar macht.
- **Aktualisieren:** Sie kehren regelmäßig zu bereits besuchten Seiten zurück, um Änderungen oder neue Inhalte zu erfassen.

Crawler sind also ein Werkzeug, das große Mengen an Webinhalten für Suchmaschinen oder als Trainingsdaten sammelt.

### So arbeitet ein Crawler

Ein Crawler startet auf einer Webseite, liest deren Inhalt, extrahiert alle Links und fügt diese zu einer Warteschlange hinzu. Dann besucht er die nächsten Seiten in dieser Warteschlange – und wiederholt den Prozess.

So entsteht eine automatisierte, breite Erfassung des [[02 - Künstliche Intelligenz/Garten erkunden/Grundlagen/Das Internet - Surface Web, Deep Web und Dark Web#Surface Web – Die Spitze des Eisbergs\|Surface Web]].

## Muss denn das sein?

Website-Betreiber können Crawler von Teilen oder ihrer gesamten Seite ausschließen. Dafür legen sie im Hauptverzeichnis ihrer Website eine Textdatei namens robots.txt an (also unter `meine-website.de/robots.txt`), in der steht, welcher Crawler wohin darf und wohin nicht.

Seriöse Crawler halten sich daran; technisch erzwingen lässt sich das allerdings nicht. Der Server kontrolliert nämlich nichts; der Crawler muss die robots.txt selbst lesen und sich freiwillig daran halten. Es lässt sich nicht einmal sicher sagen, wer da anklopft: Betreiber benennen ihre Crawler selbst und können sie genauso gut als ganz normalen Browser ausgeben.

Es gibt weitere [[02 - Künstliche Intelligenz/3 - Work on tomorrow/Möglichkeiten, sich gegen Crawler zu wehren\|Möglichkeiten, sich gegen Crawler zu wehren]], einen hundertprozentigen Schutz gibt es jedoch nicht.

### Beispiele für eine robots.txt

Um einen bestimmten Crawler auszusperren, muss man ihn beim Namen nennen:

```
User-agent: ClaudeBot
Disallow: /privat/
Disallow: /entwuerfe/
```

Hier darf `ClaudeBot`, der Crawler von Anthropic, nichts besuchen, was unter `/privat/` und `/entwuerfe/` erreichbar ist. Der Rest der Seite bleibt für ihn offen, und alle anderen Crawler sind davon gar nicht betroffen.

Es gibt aber Hunderte Bots, und es wäre viel Arbeit, sie alle aufzulisten; ohnehin sind nicht alle beim Namen bekannt. Daher kann man mit einem Stern auch alle auf einmal aussperren:

```
User-agent: *
Disallow: /

User-agent: Googlebot
Allow: /
```

Der erste Block sperrt alle Crawler aus dem Hauptverzeichnis (`/`) aus und damit von allem, was darin liegt, also von der ganzen Seite. Damit wäre allerdings auch der Googlebot ausgesperrt, und die Seite würde nicht mehr in der Google-Suche auftauchen. Deshalb bekommt er im zweiten Block ausdrücklich wieder Zutritt.

### Mehr als ein freundlicher Hinweis

Technisch kann jeder Crawler die robots.txt ignorieren. Rechtlich hat sie aber dennoch Gewicht: In der EU dürfen öffentlich zugängliche Inhalte grundsätzlich automatisiert ausgewertet werden (Fachbegriff: Text- und Data-Mining), auch fürs KI-Training. Das gilt allerdings nur, solange die Rechteinhaber nicht widersprechen, und zwar so, dass eine Maschine den Widerspruch lesen kann. Ob dafür ein Satz in normaler Sprache genügt, zum Beispiel in den Nutzungsbedingungen, ist umstritten; die robots.txt gilt als der sicherste Weg.[^laion]

[^laion]: Im Dezember 2025 entschied das OLG Hamburg (Az. 5 U 104/24) über die Klage des Fotografen Robert Kneschke gegen den gemeinnützigen Verein LAION, der Datensätze für KI-Training zusammenstellt. LAION hatte 2021 eines seiner Fotos heruntergeladen, um zu prüfen, ob Bild und Beschreibung zusammenpassen. Die Fotoagentur, über die das Foto angeboten wurde, hatte der automatisierten Nutzung nur in ihren Nutzungsbedingungen widersprochen, also in normaler Sprache. Das Gericht wies die Klage aus zwei Gründen ab. Erstens konnte der Fotograf nicht belegen, dass Maschinen 2021 so einen Satz schon zuverlässig lesen konnten; der Widerspruch zählte also nicht. Zweitens durfte LAION das Foto als gemeinnützige Forschungseinrichtung ohnehin nutzen, denn für nicht-kommerzielle Forschung spielt ein Widerspruch keine Rolle. Nach Ansicht des Gerichts hätte dem Fotografen also selbst eine robots.txt nicht geholfen. Rechtskräftig ist das Urteil noch nicht: Der Fotograf ist in Revision gegangen, der Bundesgerichtshof hat im September 2026 verhandelt (Az. I ZR 281/25) und erwägt, die Sache dem Europäischen Gerichtshof vorzulegen. (Stand: September 2026; da KI inzwischen normale Sprache versteht, bleibt unklar, ob ein Hinweis in den Nutzungsbedingungen inzwischen reichen könnte).