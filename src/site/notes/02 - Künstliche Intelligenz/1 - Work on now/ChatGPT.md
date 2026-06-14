---
{"title":"ChatGPT","aliases":null,"tags":null,"gen_ai_anteil":null,"created":"2026-06-06","updated":"2026-06-13","status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/1-work-on-now/chat-gpt/","dgPassFrontmatter":true,"dg-note-properties":{"title":"ChatGPT","aliases":null,"tags":null,"gen_ai_anteil":null,"created":"2026-06-06","updated":"2026-06-13","status":null}}
---

# ChatGPT

## Erfolgreichste Software-Anwendung aller Zeiten

Am 30. November 2022 betrat ChatGPT die Bühne der Welt und nahm sie auch gleich im Sturm. 

Bereits nach 5 Tagen hatte es eine Million Nutzer und war somit zu diesem Zeitpunkt mit Abstand die am schnellsten wachsende Anwendung aller Zeiten - weit vor Facebook, Instagram oder Spotify. 

Ich war nicht unter der ersten Million, stieg aber als “ [[02 - Künstliche Intelligenz/3- Veröffentlicht/Diffusion of Innovations#Early Adopters (~13,5 %)\|Early Adopter]]” kurz darauf ein. Keine 2 Monate später waren wir schon 100 Millionen Anwender. 

Der Erfolg kam völlig unerwartet, auch für die Firma hinter dem noch jungen [[02 - Künstliche Intelligenz/3- Veröffentlicht/LLMs (Large Language Models)\|LLM]]: [[02 - Künstliche Intelligenz/2 - Work on soon/OpenAI\|OpenAI]].

![ChatGPT 1 Mio Nutzer Statista.png](/img/user/02%20-%20K%C3%BCnstliche%20Intelligenz/1%20-%20Work%20on%20now/Bilder/ChatGPT%201%20Mio%20Nutzer%20Statista.png)

## Immer noch: Marktführer

Heute nutzen täglich Millionen Menschen den freundlichen (ja, [[02 - Künstliche Intelligenz/3- Veröffentlicht/Sykophantie\|allzufreundlichen]]) Chatbot. 

Obwohl in Rankings inzwischen viele andere [[02 - Künstliche Intelligenz/3- Veröffentlicht/LLMs (Large Language Models)\|LLMs]] ChatGPT den Platz an der Spitze als bestes Sprachmodell streitig machen, liegt der Marktanteil nach wie vor bei über 50% (je nach Messmethode und Zeitpunkt - die Zahlen sind gerade im Sinkflug, Gemini holt stark auf).

![Pasted image 20260614091311.png](/img/user/02%20-%20K%C3%BCnstliche%20Intelligenz/1%20-%20Work%20on%20now/Bilder/Pasted%20image%2020260614091311.png)

Auf Seiten wie [https://llm-stats.com/](https://llm-stats.com/) kann man nachschauen, welches LLM in aktuellen Benchmarks vorne liegt; aktuell liefern sich mal wieder Claude und ChatGPT ein hartes Kopf-an-Kopf-Rennen, aber auch Grok und Gemini hatten immer mal wieder den ersten Platz inne. 
## GPT = Generative Pre-trained Transformer

“Chat” kommt aus dem Englischen und bedeutet “Gespräch, Plauderei”, aber was hat es eigentlich mit dem “GPT” in ChatGPT auf sich? 

G - Generative
P - Pre-trained
T - Transformer

Wir haben es hier mit einem “generativem vortrainiertem Transformer” zu tun. 

Schauen wir es uns Schritt für Schritt an:
### Generative

- Das Modell erzeugt etwas (und zwar Texte)
- Es gehört damit der übergeordneten Kategorie [[02 - Künstliche Intelligenz/3- Veröffentlicht/GenAI\|Generative KI]] an, welche u.a. Texte, Bilder, Videos und Musik generieren kann 
### Pre-trained

- Es wurde **vorab** mit riesigen Mengen Text trainiert: prinzipiell stand das gesamte [[02 - Künstliche Intelligenz/3- Veröffentlicht/Das Internet - Surface Web, Deep Web und Dark Web\|Internet]] zur Verfügung, allerdings wurde hier eine gewisse [[02 - Künstliche Intelligenz/3- Veröffentlicht/LLMs (Large Language Models)#Vorauswahl\|Vorauswahl]] getroffen und [[02 - Künstliche Intelligenz/3- Veröffentlicht/LLMs (Large Language Models)#Filter\|Filter]] kamen zum Einsatz. So wird sichergestellt, dass die Textausgaben einen gewissen Sprachstandard einhalten — und offensichtlich diskriminierende Inhalte werden bereits hier herausgefiltert.
- Die Vorauswahl und Filter allein reichen jedoch nicht aus, um Diskriminierung vollständig auszuschließen - subtile Vorurteile stecken oft in der Sprache selbst, auch in harmlosen Texten. Deshalb wird im Post-Training gezielt nachgesteuert. 
- Wir als Nutzer können die “fertig trainierte” KI nicht mehr prinzipiell ändern
- Ein Beispiel: Versuche ChatGPT im normalen Gebrauch dazu zu bringen, frauenfeindliche oder islamophobe Äußerungen von sich zu geben. Du wirst scheitern - die Schutzmechanismen verhindern das zuverlässig (von [[Jailbreaks\|Jailbreaks]] einmal abgesehen).
### Transformer

- Eine spezielle KI-Technologie, welche den Durchbruch der KI-Forschung und den enormen Erfolg von ChatGPT mit sich brachte
- Merkhilfe: [[02 - Künstliche Intelligenz/2 - Work on soon/Transformer\|Transformer]]-Modelle nehmen die Texteingabe des Nutzers - und _transformieren_ sie in eine (hoffentlich) hilfreiche Antwort: Eingabe (Input) → Antwort (Output)

👉 Hier liegt das [[02 - Künstliche Intelligenz/2 - Work on soon/Input-Output-Prinzip\|Input-Output-Prinzip]] zugrunde, dem nicht nur [[02 - Künstliche Intelligenz/3- Veröffentlicht/LLMs (Large Language Models)\|LLMs]], sondern auch Computer allgemein folgen. 

## ChatGPT, Sykophanthie und KI-Psychosen

LLMs wurden darauf trainiert, dem Nutzer Antworten zu geben, welche er oder sie als nützlich empfindet.

In Tests haben User generell Antworten von LLMs als besser bewertet, wenn sie eine Antwort erhalten haben anstatt ein “ehrlich gesagt, ich weiß es nicht.” - selbst wenn die Antwort falsch war. Das ist einer der Faktoren, die das Auftreten von falschen Antworten, sogenannten [[Halluzinationen\|Halluzinationen]] stark verstärkt haben.

Die Neigung, nützlich erscheinen zu wollen und sich beim User einzuschmeicheln, nennt sich [[02 - Künstliche Intelligenz/3- Veröffentlicht/Sykophantie\|Sykophantie]] - und ChatGPT hat diese Kunst gemeistert. Das hatte weitreichende Konsequenzen, angefangen bei der Anthropomorphisierung (Vermenschlichung) dieser Modelle, über emotionale Abhängigkeit bis hin zu [[02 - Künstliche Intelligenz/2 - Work on soon/KI-Psychosen\|KI-Psychosen]]. 

## 📖 Weiterlesen

[[02 - Künstliche Intelligenz/2 - Work on soon/OpenAI\|OpenAI]] - die Firma hinter ChatGPT
[[02 - Künstliche Intelligenz/2 - Work on soon/Sam Altman\|Sam Altman]] - der charismatische CEO von OpenAI
[[Empire of AI\|Empire of AI]] - ein kritisches Werk von [[Karen Hao\|Karen Hao]]
[[Welches LLM ist das beste?\|Welches LLM ist das beste?]]

  
