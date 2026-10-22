---
{"title":"Cognitive Debt","aliases":["Cognitive Debt (kognitive Schulden)","kognitive Schulden"],"tags":null,"gen_ai_anteil":["Claude 80%"],"created":"2026-10-15","updated":null,"status":null,"dg-publish":true,"permalink":"/zum-karnickelstall/1-final-check/cognitive-debt/","dgPassFrontmatter":true,"dg-note-properties":{"title":"Cognitive Debt","aliases":["Cognitive Debt (kognitive Schulden)","kognitive Schulden"],"tags":null,"gen_ai_anteil":["Claude 80%"],"created":"2026-10-15","updated":null,"status":null}}
---

# Cognitive Debt

**Cognitive Debt** („kognitive Schulden“) beschreibt die versteckten Kosten, die entstehen, wenn man sich das Denken abnehmen lässt: Kurzfristig spart man Mühe, langfristig zahlt man drauf, mit Zinsen. 

Die Metapher lehnt sich an die **Technical Debt** (technische Schulden) aus der Softwareentwicklung an, ein Begriff, den Ward Cunningham 1992 prägte: Wer heute schnell und unsauber programmiert, muss morgen teuer aufräumen.

## Ein Begriff, drei Bedeutungen

Der Begriff wird heute meist mit KI verbunden, ist aber älter. Je nach Fachgebiet meint er Unterschiedliches.

### Medizin (2015)

Natalie Marchant und Robert Howard führten den Begriff in der Alzheimer-Forschung ein.[^marchant] Gemeint sind Denk- und Verhaltensmuster, die das Risiko für Alzheimer erhöhen, allen voran wiederholtes negatives Grübeln, wie es bei Depression, Angststörungen oder chronischem Stress vorkommt.

Cognitive Debt ist hier das Gegenstück zur **kognitiven Reserve**, also dem Puffer, den Bildung, geistige Aktivität und soziale Kontakte im Gehirn aufbauen. Ist die kognitive Reserve das Sparkonto, ist Cognitive Debt die Kreditkartenrechnung.
### Schreiben mit KI (2025)

Bekannt wurde der Begriff durch eine [[Zum Karnickelstall/1 - Final Check/MIT-Studie zum Schreiben mit ChatGPT\|MIT-Studie zum Schreiben mit ChatGPT]].[^mit] Dort meint er die langfristigen Kosten, wenn ein Mensch Denkarbeit dauerhaft an KI abgibt: weniger kritisches Denken, schwächere Erinnerung, weniger eigene Ideen. Untersucht wurde nur eine einzige Aufgabe, nämlich das Schreiben von Essays. Die Medien machten daraus vielfach pauschal „ChatGPT macht dumm“.

Vielerorts liest man außerdem, das MIT habe den Begriff „geprägt“. Das stimmt nicht, und die Studie selbst erhebt diesen Anspruch auch nicht.
### Softwareteams (2025/26)

Die Informatik-Professorin Margaret-Anne Storey (University of Victoria) übertrug den Begriff aufs Programmieren.[^storey] Hier geht es um das **gemeinsame Verständnis eines Teams**: Niemand weiß mehr so recht, wie und warum die eigene Software funktioniert. Für Storey ist Cognitive Debt deshalb eine Eigenschaft des Projekts, nicht einer Person. Besonders schnell häufen sich diese Schulden beim [[Garten erkunden/Grundlagen/Vibecoding\|Vibecoding]] an, wenn KI den Code schreibt und niemand mehr genau hinschaut.

## Drei Arten von Schulden

Für die Softwareentwicklung unterscheidet Storey drei Schichten:[^storey]

| Schuldenart | Wo sie sitzt | Was sie begrenzt |
|---|---|---|
| **Technical Debt** | im Code | wie leicht sich das System ändern lässt |
| **Cognitive Debt** | in den Köpfen | wie gut das Team über Änderungen nachdenken kann |
| **Intent Debt** | in der Dokumentation | ob das System noch tut, was es ursprünglich sollte |

**Intent Debt** („Absichtsschulden“) entsteht, wenn Ziele, Gründe und Rahmenbedingungen nie aufgeschrieben wurden, sondern nur in einzelnen Köpfen existieren.

Die unbequeme Pointe: KI kann technische Schulden sogar senken, weil sie oft sauberen Code schreibt. Gleichzeitig beschleunigt sie kognitive und Absichtsschulden. Der Code sieht gut aus, aber keiner versteht ihn mehr.

Storey stützt sich dabei auf eine Idee des dänischen Informatikers Peter Naur aus dem Jahr 1985: Ein Programm ist mehr als sein Code. Es ist eine **Theorie** in den Köpfen der Entwickler, darüber, was das System tun soll und warum es so gebaut ist. Geht diese Theorie verloren, bleibt nur Code übrig, den niemand mehr sicher verändern kann.

## Woran man sie erkennt

Cognitive Debt meldet sich nicht laut. Es gibt keine Fehlermeldung, keinen abgestürzten Build. Storey beschreibt ein Studententeam, das in Woche sieben oder acht an eine Wand lief: Selbst kleine Änderungen machten plötzlich an unerwarteter Stelle etwas kaputt. Zunächst schob das Team es auf unsauberen Code. Das eigentliche Problem war ein anderes: Niemand konnte mehr erklären, warum bestimmte Entscheidungen getroffen worden waren.

Typische Warnsignale:

- **Im Team:** Niemand kann erklären, warum etwas so gebaut ist. Fehleranalysen enden im Rätselraten.
- **Beim Einzelnen:** Man kann eigene Texte oder Lösungen nicht wiedergeben oder erklären. Ohne KI fällt der Einstieg schwer.

## Nicht jedes Auslagern ist ein Problem

Gedächtnis und Denken an Hilfsmittel abzugeben ist nichts Neues. Die Kognitionspsychologie nennt das **Cognitive Offloading** (kognitive Entlastung).[^offloading] Wir tun es ständig: mit Kalendern, Einkaufszetteln, Taschenrechnern, Navis.

Der Unterschied liegt darin, *was* man auslagert:

- **Unproblematisch:** Dinge, die man nicht selbst können muss. Einen Termin muss ich mir nicht merken, wenn er im Kalender steht.
- **Problematisch:** Fähigkeiten, die man eigentlich aufbauen oder behalten will. Wer jedes Urteil, jede Analyse und jeden Gedankengang der KI überlässt, verlernt genau das.

## Gegenmittel

> [!quote] Denken kann man auslagern, Verständnis nicht.
> _- Andrej Karpathy (2026)_

Daraus folgt Karpathys wichtigste Regel,[^karpathy] für Einzelne wie für Teams: **Die KI nichts bauen lassen, was man selbst nicht versteht.**

**Für Einzelne:**
- Erst selbst denken, dann KI. Die MIT-Studie deutet darauf hin, dass die Reihenfolge eine Rolle spielt.
- KI Fragen stellen lassen, statt sich Antworten liefern zu lassen. Mehr dazu unter [[Garten erkunden/Digitale Gärten, PKM & Lernen/Aktives Lernen\|Aktives Lernen]].
- Ab und zu bewusst ohne KI arbeiten und prüfen, ob man es noch kann.

**Für Teams:**
- Bewusst langsamer werden, wenn das Verständnis nicht mehr hinterherkommt.
- Entscheidungen und deren Gründe aufschreiben. Das bekämpft gleichzeitig Intent Debt.
- KI-generierten Code gemeinsam besprechen, statt ihn ungelesen zu übernehmen.

## Kritik am Begriff

- **Schwer messbar:** „Schulden“ ist eine Metapher. Wie viel Cognitive Debt ein Mensch oder Team angehäuft hat, lässt sich bislang nicht beziffern.
- **Alter Wein in neuen Schläuchen?** Manche halten den Begriff für überflüssig, weil es mit Cognitive Offloading oder **Deskilling** (Verlust von Fähigkeiten durch Automatisierung) längst etablierte Begriffe gibt.
- **Verwässerung:** Drei Fachgebiete, drei Bedeutungen. Wer „Cognitive Debt“ liest, sollte genau hinschauen, welche gemeint ist.

## 📖 Weiterlesen

- [[Zum Karnickelstall/1 - Final Check/MIT-Studie zum Schreiben mit ChatGPT\|MIT-Studie zum Schreiben mit ChatGPT]]: die Studie, die den Begriff im KI-Kontext bekannt machte, samt ihrer Schwachstellen.
- [[Garten erkunden/Grundlagen/Vibecoding\|Vibecoding]]: Wo Cognitive Debt in der Softwareentwicklung besonders schnell entsteht.
- [[Garten erkunden/Grundlagen/Agentic Engineering\|Agentic Engineering]]: Programmieren mit KI-Agenten, bei dem Menschen Architektur und Verständnis bewusst selbst verantworten.

## 📺 Aus der YouTube Academy

- Ein sehr empfehlenswertes Video zu kognitive Schulden in der Softwareentwicklung: [AI Cognitive Debt: The Crisis Nobody Sees Coming](https://www.youtube.com/watch?v=Tk0hIOAwf6M)
- Karpathy spricht noch eine vierte Form der kognitiven Schulden an. Sie entsteht, wenn ein Großteil der Menschheit das Verständnis und die Kontrolle über die noch junge Technologie verliert: [Karpathy: The AI Understanding Gap Is Getting Worse, Fast](https://www.youtube.com/watch?v=BjO_JC6ujXs) Aus meiner Sicht ist es tragisch, wenn eine kleine Elite von nur etwa 5000 Menschen diese Erfindung wirklich versteht und vorantreibt, die für das Schicksal der Menschheit so entscheidend sein könnte. Wer lieber lesen als gucken möchte: 📖 [[Zum Karnickelstall/Must-Have/KI – alles nur Hype? Wenn nur wenige verstehen, was gerade entsteht\|KI – alles nur Hype? Wenn nur wenige verstehen, was gerade entsteht]]


[^marchant]: Marchant, N. L. & Howard, R. J. (2015): „Cognitive Debt and Alzheimer's Disease“, Journal of Alzheimer's Disease 44(3), S. 755–770. [doi.org/10.3233/JAD-141515](https://doi.org/10.3233/JAD-141515)

[^mit]: Kosmyna et al. (2025): „Your Brain on ChatGPT: Accumulation of Cognitive Debt when Using an AI Assistant for Essay Writing Task“, arXiv:2506.08872

[^storey]: Margaret-Anne Storey (2026): „How Generative and Agentic AI Shift Concern from Technical Debt to Cognitive Debt“, [margaretstorey.com/blog/2026/02/09/cognitive-debt](https://margaretstorey.com/blog/2026/02/09/cognitive-debt/). Erstmals verwendet hat sie den Begriff laut eigener Aussage im Oktober 2025 in einem Startup-Kurs.

[^offloading]: Geprägt u. a. von Evan Risko und Sam Gilbert (2016): „Cognitive Offloading“, Trends in Cognitive Sciences.

