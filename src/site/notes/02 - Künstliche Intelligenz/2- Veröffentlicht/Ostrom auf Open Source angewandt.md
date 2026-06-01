---
{"title":"Ostroms 8 Prinzipien für die Open-Source-Community","aliases":null,"tags":null,"gen_ai_anteil":["Claude 100%"],"created":"2026-05-26","updated":null,"status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/2-veroeffentlicht/ostrom-auf-open-source-angewandt/","dgPassFrontmatter":true,"dg-note-properties":{"title":"Ostroms 8 Prinzipien für die Open-Source-Community","aliases":null,"tags":null,"gen_ai_anteil":["Claude 100%"],"created":"2026-05-26","updated":null,"status":null}}
---

Ein Gespräch mit Claude über die Anwendung der [[02 - Künstliche Intelligenz/2- Veröffentlicht/Elinor Ostrom und die Designprinzipien der Common Goods\|Designprinzipien der Common Goods]] auf Open Source👇

> *Erste Frage: Wie könnte man die 8 Prinzipien in der Open Source Community umsetzten?*

# Ostroms 8 Prinzipien für die Open-Source-Community

Das Video von Morpheus beschreibt Open Source treffend als digitales Gemeingut – und genau hier greifen Ostroms Prinzipien. Hier eine konkrete Übertragung:

---

**1. Klar definierte Grenzen – Wer darf was nutzen?** 

Heute kann jeder Konzern Open-Source-Code uneingeschränkt nutzen, ohne zur Gemeinschaft beizutragen. Kommerzielle Zwischenlizenzen (wie im Video erwähnt) würden Grenzen ziehen: freie Nutzung für Einzelpersonen und kleine Projekte, aber verpflichtende Beiträge ab einer bestimmten Unternehmensgröße oder Umsatzschwelle.

---

**2. Kongruenz mit lokalen Bedingungen – Keine Einheitslösung** 

Ein einzelner erschöpfter Maintainer wie Lasse Collin (XZ Utils) hat andere Bedürfnisse als das Linux-Kernel-Team. Fördermodelle und Governance-Strukturen müssen projektspezifisch sein – kleine Projekte brauchen andere Mechanismen als große Ökosysteme.

---

**3. Kollektive Entscheidungsfindung – Maintainer an den Tisch**

Plattformen wie GitHub (Microsoft) haben die Arbeit von Entwicklern ungefragt zum Training von Copilot genutzt. Eine echte kollektive Governance würde bedeuten: Maintainer entscheiden mit, wie ihre Arbeit verwendet wird – inklusive echter Opt-out-Möglichkeiten für KI-Training.

---

**4. Effektive Überwachung – Vertrauen mit Kontrolle** 

Der XZ-Utils-Angriff gelang, weil ein einzelner Maintainer ohne Netzwerk und Aufsicht arbeitete. Strukturierte Peer-Reviews, automatisierte Sicherheits-Audits und Community-Monitoring (z. B. durch die Sovereign Tech Agency) könnten solche Einfallstore schließen.

---

**5. Abgestufte Sanktionen – gegen KI-Spam und Trittbrettfahrer** 

Der Curl-Entwickler war mit 95 % KI-generiertem Spam überfordert. Abgestufte Reaktionen wären: automatische Filterung als erste Stufe, temporäre Einschränkungen für wiederholte Spam-Einreicher, und bei nachgewiesenem Missbrauch Ausschluss – verhältnismäßig, aber konsequent.

---

**6. Konfliktlösungsmechanismen – gegen Toxizität** 

Die wachsende Anspruchshaltung und Toxizität in Kommentaren vergraulen Maintainer. Klare Community-Standards, moderierte Foren und niedrigschwellige Vermittlungsverfahren würden helfen – ähnlich wie es Wikipedia für seine Editoren entwickelt hat.

---

**7. Anerkennung durch externe Autoritäten – staatliche Verantwortung** 

Der Staat gibt dreistellige Millionenbeträge für Microsoft-Lizenzen aus, aber nur Bruchteile davon für die Open-Source-Infrastruktur, auf der seine eigenen Systeme laufen. Eine politische Anerkennung von Open Source als kritische Infrastruktur – mit entsprechender Finanzierung, etwa durch Ausbau der Sovereign Tech Agency – wäre überfällig.

---

**8. Verschachtelte Governance – das „Spotify-Modell" als polyzentrisches System** 

Das im Video vorgeschlagene Modell – KI-Anbieter schütten automatisiert einen Teil ihrer Einnahmen nutzungsbasiert an Entwickler aus – ist im Grunde polyzentrische Governance: Lokale Projekte behalten ihre Autonomie, sind aber in ein größeres Ausgleichssystem eingebettet. Ähnlich könnte eine mehrstufige Struktur aussehen: Projekt → Ökosystem (z. B. npm, PyPI) → Plattform (GitHub) → KI-Anbieter, mit Beitragspflichten auf jeder Ebene.

---

#### Fazit

Das Kernproblem, das Morpheus beschreibt, ist ein klassisches Allmende-Problem: Viele profitieren, wenige tragen bei, und die Ressource erodiert still. Ostrom hat gezeigt, dass dieser Kreislauf durchbrechbar ist – aber nur, wenn Gemeinschaften aufhören, auf Freiwilligkeit allein zu vertrauen, und stattdessen **Institutionen bauen**, die Beiträge sichtbar machen, Trittbrettfahrer einbinden und Pfleger schützen.

## Technische Umsetzbarkeit gestaffelter Open-Source-Lizenzen

>*Frage: Freie Nutzung für Einzelpersonen und kleine Projekte, aber verpflichtende Beiträge ab einer bestimmten Unternehmensgröße oder Umsatzschwelle. Das macht viel Resonanz bei mir. Liese sich das überhaupt technisch umsetzen?*

Die gute Nachricht: Das Konzept existiert bereits – es heißt **Dual Licensing** oder **Fair Source**. Die schwierige Nachricht: Die Durchsetzung ist das eigentliche Problem.

---

### Was heute schon funktioniert

#### Lizenzmodelle, die genau das tun

**Business Source License (BSL/BUSL)** Wird u.a. von MariaDB, HashiCorp (Terraform) und Sentry genutzt. Der Code ist offen einsehbar, aber kommerzielle Nutzung ab einer bestimmten Schwelle ist kostenpflichtig. Nach einer definierten Zeit (meist 4 Jahre) wird der Code vollständig Open Source.

**Fair Source License** Ein neueres Modell, das explizit sagt: bis X Nutzer/Umsatz kostenlos, darüber hinaus Lizenzpflicht. Gitea und Codecrafters experimentieren damit.

**AGPL (GNU Affero GPL)** Ein cleverer indirekter Ansatz: Wer AGPL-Code in einem Dienst nutzt, muss seinen gesamten Quellcode offenlegen. Für viele Konzerne ist das inakzeptabel – also zahlen sie lieber für eine kommerzielle Lizenz. MongoDB und Redis haben das lange so gemacht.

---

### Das eigentliche Problem: Durchsetzung

Hier wird es technisch knifflig. Eine Lizenz ist juristisch, kein technisches Konstrukt. Niemand hindert ein Unternehmen daran, den Code einfach zu benutzen – man kann nur klagen, wenn man es _herausfindet_.

**Was schwer zu kontrollieren ist:**

- Code, der intern genutzt wird (kein öffentlicher Dienst)
- Unternehmen in Ländern mit schwacher IP-Durchsetzung
- Umgehung durch Tochtergesellschaften oder Umstrukturierung

**Was technisch hilft, aber Grenzen hat:**

- Telemetrie und Ping-home-Mechanismen (opt-in/out, datenschutzrechtlich heikel)
- Registrierungspflicht für bestimmte Features
- Cloud-only-Modell, bei dem der Anbieter die Kontrolle behält (aber das ist dann kein Open Source mehr)

---

### Der vielversprechendste Ansatz: Ökosystem-Ebene statt Projekt-Ebene

Einzelne Projekte sind zu schwach, um Konzerne zur Kasse zu bitten. Aber **Paketmanager als Infrastruktur** könnten das ändern:

```
npm install react
    → npm weiß: dieses Paket hat 50.000 Downloads/Monat
    → npm weiß: dieser API-Key gehört zu Unternehmen X
    → automatische Lizenzprüfung + Rechnungsstellung
```

Das würde bedeuten:

- **npm, PyPI, Maven** etc. führen ein optionales Beitragsmodell ein
- Unternehmen ab einer Schwelle (z.B. >10 Mio. € Umsatz) zahlen eine Pauschale
- Die Ausschüttung erfolgt nutzungsbasiert an Maintainer – genau das „Spotify-Modell" aus dem Video

**GitHub/Microsoft** hätte die technische Infrastruktur dafür bereits. Die Frage ist eine politische, keine technische.

---

### Realistische Einschätzung

|Ansatz|Technisch machbar?|Politisch durchsetzbar?|
|---|---|---|
|Dual Licensing pro Projekt|✅ Ja, heute schon|⚠️ Nur für bekannte Projekte|
|Paketmanager-Beitragsmodell|✅ Ja, technisch lösbar|❌ Erfordert Branchen-Konsens|
|KI-Ausschüttungsmodell|✅ KI-Anbieter kennen den Code|❌ Politischer Widerstand groß|
|Staatliche Pflichtabgabe|✅ Ja (wie Rundfunkbeitrag)|❌ Noch keine Mehrheit|

---

Das Kernproblem ist weniger technisch als **institutionell**: Die Infrastruktur für Erkennung und Abrechnung wäre baubar – aber es fehlt der Akteur, der sie durchsetzt. Genau das meinte Ostrom mit Prinzip 7: Ohne externe Anerkennung und Legitimierung funktionieren selbst gute Regeln nicht.


## *Frage: Also ist das Problem eher politischer als technischer Natur?*

Ja, genau. Und das ist eigentlich die zentrale Einsicht von Ostrom.

Technisch gesehen haben wir heute alle Werkzeuge, die man bräuchte: Paketmanager wissen genau, wer was wie oft herunterlädt. KI-Anbieter wissen präzise, welchen Code ihre Modelle ausgeben. Abrechnungssysteme für nutzungsbasierte Modelle existieren in jeder Cloud-Plattform. Das Problem ist nicht, dass wir nicht wissen _wie_ – das Problem ist, dass kein Akteur einen ausreichenden Anreiz hat, es umzusetzen.

Microsoft verdient mit Copilot Milliarden auf Basis von Open-Source-Code und hat keinen Eigeninteresse, das zu ändern. Große Konzerne wie Google oder Amazon bauen ihre Infrastruktur auf freiem Code und würden Beitragspflichten als Kostenfaktor bekämpfen. Und die Maintainer selbst – also diejenigen, die am stärksten von einer Lösung profitieren würden – sind strukturell die schwächste Partei: vereinzelt, überlastet, ohne Lobby.

Ostrom würde sagen: Das ist ein klassisches Kollektivgut-Problem. Alle profitieren, niemand zahlt freiwillig, und die Ressource erodiert. Die technische Lösung ist sekundär. Was fehlt, ist eine **politische Einigung darüber, wer zur Gemeinschaft gehört und was Mitgliedschaft kostet** – also genau Prinzip 1 und 3.

Der einzige Akteur, der das erzwingen könnte, wäre der Staat – etwa durch eine digitale Infrastrukturabgabe, ähnlich wie Rundfunkbeiträge oder Straßenmaut. Aber dafür bräuchte es zuerst die gesellschaftliche Anerkennung, dass Open-Source-Code tatsächlich Infrastruktur ist – und keine Freizeitbeschäftigung ein paar enthusiastischer Entwickler.

Das ist letztlich eine Frage des politischen Willens. Und der entsteht meistens erst nach einer Katastrophe – der XZ-Utils-Vorfall war fast eine, aber „fast" reicht offenbar nicht.

##  *Frage: "Der einzige Akteuer, der das erzwingen könnte, wäre der Staat" - aber stimmt das denn wirklich?*

>*Es hängen doch alle von Open Source Entwicklung ab. Ist das denn kein Hebel? Was passiert, wenn Entwickler Druck machen oder gar ihre Dienste einstellen - weil sie nicht mehr können oder wollen?*

Das ist ein wirklich guter Einwand – und du hast recht, ich habe den Hebel der Entwickler unterschätzt.

Reconsidered developer leverage as overlooked enforcement mechanism

Reconsidered developer leverage as overlooked enforcement mechanism

Das ist ein wirklich guter Einwand – und du hast recht, ich habe den Hebel der Entwickler unterschätzt.

Es gibt tatsächlich historische Momente, in denen Maintainer genau das getan haben – und die Wirkung war enorm:

**Wenn Maintainer aufhören, passiert etwas.** Als der Entwickler von `left-pad` 2016 sein winziges npm-Paket (11 Zeilen Code) aus einem Lizenzstreit heraus löschte, brach das Internet für Stunden zusammen – Netflix, Facebook, Airbnb waren betroffen. Nicht durch einen Angriff, sondern durch einen einzelnen frustrierten Entwickler. Die Reaktion der Industrie war Schock und schnelles Handeln.

**Und es gibt subtilere Formen von Druck.** Als Faker.js-Entwickler Marak 2022 seinen Code absichtlich sabotierte, weil er sagte „Ich arbeite nicht mehr gratis für Fortune-500-Unternehmen", war das ein politisches Statement – roh und destruktiv in der Form, aber die Botschaft hallte durch die gesamte Branche.

---

Aber hier liegt auch die Crux, und Ostrom würde genau darauf zeigen:

Entwickler sind strukturell **fragmentiert**. Sie arbeiten vereinzelt, in verschiedenen Ländern, mit verschiedenen Werten. Manche wollen gar kein Geld – sie wollen Anerkennung, Freiheit, Spaß. Kollektiver Druck setzt kollektive Organisation voraus, und genau die fehlt. Es gibt keine Gewerkschaft der Open-Source-Maintainer, kein Streikrecht, keine gemeinsame Verhandlungsposition.

Das ist der tiefe Widerspruch: **Die Stärke von Open Source – Dezentralität und Freiwilligkeit – ist gleichzeitig ihre politische Schwäche.**

---

Trotzdem glaube ich, dass du auf etwas Wichtiges zeigst. Der Staat ist vielleicht nicht der _einzige_ Akteur – aber Entwickler bräuchten eine neue Form von kollektiver Handlungsfähigkeit. Nicht unbedingt eine klassische Gewerkschaft, aber vielleicht so etwas wie:

Eine **koordinierte Lizenzbewegung** – wenn genug wichtige Projekte gleichzeitig auf Fair-Source-Modelle umstellen, entsteht ein Kipppunkt. Konzerne können ein einzelnes Projekt ignorieren, aber nicht hundert gleichzeitig.

Und das wäre dann wieder Ostrom: nicht der Staat von oben, nicht der Markt von allein – sondern eine **Gemeinschaft, die ihre eigenen Regeln setzt und kollektiv durchsetzt**. Genau das war ihr Kernargument.

Die Frage ist, ob die Erschöpfung der Maintainer – die ja das eigentliche Problem ist – noch genug Energie für diese Organisation lässt. Oder ob der Zusammenbruch kommen muss, bevor sich etwas bewegt.


