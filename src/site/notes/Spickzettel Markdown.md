---
{"title":"Spickzettel Markdown","aliases":null,"tags":null,"gen-ai-anteil":["Euria 100%"],"created":"22.05.2026","updated":null,"status":null,"dg-publish":true,"permalink":"/spickzettel-markdown/","dgPassFrontmatter":true,"dg-note-properties":{"title":"Spickzettel Markdown","aliases":null,"tags":null,"gen-ai-anteil":["Euria 100%"],"created":"22.05.2026","updated":null,"status":null}}
---

# Kompletter Markdown-Schnellkurs für Einsteiger

## 1. Überschriften

Überschriften beginnen mit Hashtags (#), die Anzahl bestimmt die Größe.
```Markdown
# Überschrift 1 (Haupttitel)
## Überschrift 2 (Hauptabschnitt)
### Überschrift 3 (Unterabschnitt)
#### Überschrift 4
```

Es ist üblich, nach einer Überschrift eine Leerzeile einzufügen, bevor der Fließtext folgt.

## 2. Textformatierung

Kursiv wird mit einem oder zwei Sternchen oder Unterstrichen um den Text gesetzt:
`*Kursiv* oder _Kursiv_`

Fett wird mit zwei Sternchen oder Unterstrichen hervorgehoben:
`**Fett** oder __Fett__`

Kombiniert lässt sich beides erreichen:
` ***Fett und Kursiv***`

Durchgestrichenen Text bildet man mit zwei Tilden:
`~~Durchgestrichener Text~~`

## 3. Listen

Unsortierte Listen beginnen mit einem Sternchen, einem Bindestrich oder einem Punkt gefolgt von einem Leerzeichen:
```Markdown
- Erstes Element
- Zweites Element
- Drittes Element
```

Sortierte Listen funktionieren ähnlich, nutzen aber Zahlen gefolgt von einem Punkt:
```Markdown
1. Erster Schritt
2. Zweiter Schritt
3. Dritter Schritt
```

Verschachtelte Listen entstehen durch Einrücken (meist zwei oder vier Leerzeichen) der darunterliegenden Zeilen:
```Markdown
- Hauptpunkt
  - Unterpunkt 1
  - Unterpunkt 2
    - Noch tieferer Punkt
```

## 4. Links und Bilder

Links werden in eckigen Klammern für den sichtbaren Text und in runden Klammern für die URL geschrieben:
`[Google](https://www.google.com)`

Bilder funktionieren nach demselben Prinzip, benötigen aber ein Ausrufezeichen vor den eckigen Klammern:
`![Beschreibung des Bildes](pfad/zum/bild.jpg)`

## 5. Zitate und Trennlinien

Zitate beginnen in einer neuen Zeile mit einem Winkelstrich (>):
```Markdown
> Dies ist ein Zitat, das oft verwendet wird, um Meinungen oder Quellen hervorzuheben.
>
> Eine weitere Zeile im Zitat.
```

Horizontale Trennlinien entstehen durch drei oder mehr Bindestriche, Sterne oder Unterstriche in einer eigenen Zeile:
```Markdown
---
***
___
```

## 6. Aufgabenlisten (Task Lists)

Aufzählungen können auch als Aufgabenliste genutzt werden, oft mit einem Bindestrich und einer Klammer:
```Markdown
- [ ] Unvollständige Aufgabe
- [x] Abgeschlossene Aufgabe
- [ ] Weitere Aufgabe
```

## 7. Tabellen

Tabellen werden durch senkrechte Striche (|) und Bindestriche (-) definiert. Die erste Zeile enthält die Überschriften, die zweite Zeile definiert die Ausrichtung (optional), und die folgenden Zeilen enthalten die Daten:
```Markdown
| Spalte 1 | Spalte 2 | Spalte 3 |
| :--- | :---: | ---: |
| Linksbündig | Zentriert | Rechtsbündig |
| Inhalt A | Inhalt B | Inhalt C |
| Zeile 2 | Daten | Werte |
```

## 8. Code-Beispiele (Inline)

Für kurze Code-Ausschnitte innerhalb eines Satzes verwendet man einzelne Backticks (`):
```Markdown
Verwende den Befehl `ls -l`, um Dateien aufzulisten.
```

Für längere Code-Blöcke, wie in deinem Beispiel, nutzt man drei Backticks (` ``` `) mit optionaler Sprachangabe:
```Markdown
```
def hallo():
    print("Hallo Welt")
```
```