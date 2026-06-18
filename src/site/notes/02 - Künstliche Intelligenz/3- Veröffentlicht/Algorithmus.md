---
{"title":"Algorithmus","aliases":["Algorithmen"],"tags":null,"gen_ai_anteil":["Claude 40%"],"created":"2026-06-16","updated":null,"status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/3-veroeffentlicht/algorithmus/","dgPassFrontmatter":true,"dg-note-properties":{"title":"Algorithmus","aliases":["Algorithmen"],"tags":null,"gen_ai_anteil":["Claude 40%"],"created":"2026-06-16","updated":null,"status":null}}
---

# Algorithmus

>**Definition:** Ein Algorithmus ist eine endliche, eindeutige Schritt-für-Schritt-Anleitung zur Lösung eines Problems.

> [!info]  **Drei Merkmale** machen eine Anleitung zum Algorithmus:
> - **Eindeutig** - jeder Schritt ist klar formuliert, kein Interpretationsspielraum
> - **Endlich** - er hat einen definierten Anfang und ein definiertes Ende
> - **Allgemein** - er löst nicht nur einen Einzelfall, sondern eine ganze Klasse von Problemen

## Beispiel: Apfelkuchen-Rezept

Problem: Du hast Appetit auf Kuchen, aber alle Bäckereien haben geschlossen. 
Lösung: Omas Apfelkuchen Rezept

Ein Backrezept ist ein Algorithmus - es beschreibt exakt, in welcher Reihenfolge welche Schritte ausgeführt werden, damit am Ende (hoffentlich) ein Kuchen herauskommt.

![Omas Apfelkuchen.png](/img/user/02%20-%20K%C3%BCnstliche%20Intelligenz/0%20-%20Final%20Check/Bilder/Omas%20Apfelkuchen.png)
## Algorithmus vs. Computerprogramm

Ein Algorithmus ist die **Idee** - abstrakt, sprachunabhängig. Ein Computerprogramm ist die **Umsetzung** dieser Idee in einer konkreten Programmiersprache, die ein Computer ausführen kann.

- Dasselbe Rezept lässt sich auf Deutsch, Englisch oder Französisch aufschreiben. 
- Derselbe Algorithmus lässt sich in Python, Java oder C++ implementieren.
 
![Algorithmus Spamfilter.png](/img/user/02%20-%20K%C3%BCnstliche%20Intelligenz/0%20-%20Final%20Check/Bilder/Algorithmus%20Spamfilter.png)

## Im Zeitalter der KI sind wir alle Programmierer

Bisher brauchte man eine Programmiersprache, um einem Computer eine Abfolge von Schritten vorzugeben. Bei modernen KI-Tools reicht Alltagssprache. Ein mehrschrittiger Prompt ähnelt einem Algorithmus:

```
Problem: Ich habe Hunger und wenig Zeit, will aber nicht einkaufen gehen und nichts wegwerfen. Aus den Resten im Kühlschrank soll etwas Warmes entstehen.

Ziel: Ein schnelles, leckeres Gericht, das ich ohne zusätzliche Einkäufe in unter 30 Minuten kochen kann.

1. Ich habe noch ein paar Zutaten im Kühlschrank: ...
2. Schlage mir 3 Gerichte vor, die ich daraus kochen kann
3. Wähle das schnellste aus
4. Schreibe mir das Rezept Schritt für Schritt

Ergebnis: ein fertiges Rezept zum Loslegen.
```

Das ist eine klare, endliche Schritt-für-Schritt-Anweisung - dieselbe Grundstruktur wie ganz oben in der Definition.

Natürlich kann man mit KI nicht nur für Rezepte, sondern auch für das Programmieren ganzer Apps und Webseiten verwenden - das sogenannte [[02 - Künstliche Intelligenz/0 - Final Check/Vibecoding\|Vibecoding]].

### Praxiswissen für gute Prompts

- Ein guter Prompt führt - so wie ein guter Algorithmus - vom Problem zur Lösung. 
- Formuliere das Problem so genau wie möglich - denn im Formulieren des Problems ist die Lösung oft schon vorhanden
- Beschreibe die gewünschte Lösung / das Ergebnis möglichst klar und eindeutig
- Ein guter Algorithmus ist allgemein. Einmal geschrieben, funktioniert er für zahllose gleichartige Anwendungsfälle. Auch ein guter Prompt skaliert - er kann ein ähnliches Problem wieder und wieder lösen.

![Prompt Algorithmus 1.png](/img/user/02%20-%20K%C3%BCnstliche%20Intelligenz/0%20-%20Final%20Check/Bilder/Prompt%20Algorithmus%201.png)
### Prompts sind Algorithmen … fast

Ein klassischer Algorithmus liefert bei gleicher Eingabe immer dasselbe Ergebnis. Ein Prompt nicht - dieselbe Anweisung kann zwei verschiedene Antworten erzeugen.

Ein Prompt ist also kein Algorithmus im strengen Sinn, aber er teilt mit ihm den Kern: das Denken in klaren, nachvollziehbaren Schritten. 