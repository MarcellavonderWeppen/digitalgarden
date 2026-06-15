---
{"title":"Claude Desktop App - Sicherheit, Privacy, Datenschutz (von Mistral)","aliases":null,"tags":null,"gen_ai_anteil":["Mistral 100%"],"created":"2026-06-12","updated":null,"status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/0-final-check/claude-desktop-app-sicherheit-privacy-datenschutz-von-mistral/","dgPassFrontmatter":true,"dg-note-properties":{"title":"Claude Desktop App - Sicherheit, Privacy, Datenschutz (von Mistral)","aliases":null,"tags":null,"gen_ai_anteil":["Mistral 100%"],"created":"2026-06-12","updated":null,"status":null}}
---


# **Claude: Umfassende Analyse zu Sicherheit, Datenschutz und Nutzung**

**Stand: Juni 2026 – Für reguläre Nutzer:innen mit Fokus auf Privatsphäre und Sicherheitsrisiken**


---

## **1. Einleitung: Warum diese Analyse?**

Claude (insbesondere Claude Pro und Cowork) ist ein mächtiges KI-Tool – aber die **Nutzung der Desktop-App wirft erhebliche Fragen zu Sicherheit, Datenschutz und Privatsphäre** auf. Dieses Dokument fasst **alle relevanten Informationen** aus aktuellen Quellen (Juni 2026) zusammen, um dir eine fundierte Entscheidung zu ermöglichen.

---

## **2. Grundlagen: Claude, Datenschutz und DSGVO**

### **2.1 Datenschutz bei Claude (Anthropic)**

- **Datenverarbeitung:** Alle Anfragen (auch über die Desktop-App und Cowork) werden **auf US-Servern verarbeitet**. Für EU-Nutzer:innen ist dies **DSGVO-relevant**, da die USA kein angemessenes Datenschutzniveau bieten. Anthropic nutzt:
    
    - **Standardvertragsklauseln (SCCs)** als rechtliche Absicherung für den Datentransfer in die USA.
    - **EU-US Data Privacy Framework (DPF)-Zertifizierung** – allerdings politisch umstritten und keine absolute Rechtssicherheit. Die Zertifizierung kann im [offiziellen DPF-Verzeichnis](https://www.dataprivacyframework.gov/) überprüft werden. **Trotzdem empfiehlt sich die SCCs-Absicherung parallel**, da das DPF anfechtbar bleibt.
    - **"Help Improve Claude":** Falls aktiviert, können Chats und Coding-Sessions **bis zu 5 Jahre in de-identifizierter Form für das Training neuer Modelle genutzt** werden. Diese Einstellung ist **standardmäßig deaktiviert**, kann aber in den Einstellungen (Settings → Privacy → Help Improve Claude) aktiviert werden.
- **Speicherung von Daten:**
    
    - Chats, die von Sicherheitsklassifikatoren markiert werden, können **bis zu 2 Jahre gespeichert** werden.
    - Feedback (Daumen hoch/runter, Bug-Reports) wird **5 Jahre aufbewahrt**.
- **DSGVO-Konformität:**
    
    - **Theoretisch möglich**, aber nur mit **zusätzlichen Maßnahmen** (z. B. vertragliche Absicherung, Produktauswahl). Für **Hochrisiko-Anwendungen** (z. B. Gesundheitswesen, Personalauswahl) gelten strengere Regeln ab August 2026 (EU AI Act). Für normale Nutzer:innen ist der EU AI Act **kaum relevant**.
    - **Unternehmensnutzung:** Wer Claude im Unternehmen einsetzt, muss eine **Datenschutz-Folgenabschätzung (DSFA)** durchführen, wenn sensible Daten verarbeitet werden.
- **EU AI Act und Claude:**
    
    - **Geringes Risiko für normale Nutzer:innen:** Der EU AI Act betrifft vor allem **Hochrisiko-KI-Systeme** (z. B. in kritischen Infrastrukturen). Für **Generative KI wie Claude** (GPAI) gelten **keine besonderen Pflichten**, solange keine Hochrisiko-Anwendung vorliegt.

---

## **3. Sicherheitsrisiken der Claude Desktop App im Detail**

### **3.1 Zugriffsrechte der Desktop App**

Die Desktop-App nutzt folgende Mechanismen, um auf dein System zuzugreifen:

Zugriffsrechte der Desktop App

|Zugriffsart|Technische Umsetzung|Zweck|Risiko|
|---|---|---|---|
|Barrierefreiheits-APIs|AX-API (macOS), UIA (Windows)|Fensterinhalte lesen, UI-Elemente steuern|Mittel (Kompromittierung möglich)|
|Browser-Hooks|Automatische Registrierung in Browsern (Chrome, Firefox, Brave etc.)|Integration mit Web-Apps, automatisches Auslesen/Steuern von Browser-Tabs|**Hoch** (keine explizite Zustimmung, Umgehung der Browser-Sandbox)|
|Lokale Dateizugriffe|Manuell (Drag&Drop) oder automatisch (Cowork)|Dateianalyse, Bearbeitung|Mittel (Prompt-Injection in Dateien)|

---

- **Barrierefreiheits-APIs:**
    - Ermöglichen der App, **alles zu sehen und zu steuern, was dein Nutzerkonto sieht** (z. B. Terminals, E-Mail-Clients, Passwort-Manager).
    - **Explizite Berechtigungsaufforderung** bei der Installation (z. B. unter macOS: Systemeinstellungen > Barrierefreiheit > Claude Desktop aktivieren).
    - **Risiko:** Falls die App kompromittiert wird, können Angreifer **Tastatureingaben simulieren** oder **Inhalte aus anderen Apps auslesen** (z. B. Notizen, Chats, Passwörter). Allerdings ist dies **unwahrscheinlich**, solange du keine verdächtigen Dateien öffnest oder auf manipulierte Webseiten gehst.

---

### **3.2 Browser-Hooks: Das größte Sicherheitsproblem**

- **Automatische Installation:**
    
    - Die Desktop-App **registriert sich im Hintergrund in deinen Browsern** – **ohne deine Zustimmung** und ohne Hinweis in der Dokumentation.
    - Diese Hooks werden **bei jedem Start der App neu installiert** und bleiben aktiv, **auch wenn die App geschlossen ist**.
    - **Keine Transparenz:** Die App zeigt **nicht an**, welche Browser-Integrationen aktiv sind. Selbst wenn du die Berechtigung nachträglich entziehst, bleiben die Hooks oft bestehen, bis du sie manuell entfernst.
- **Auswirkungen:**
    
    - Claude kann **Inhalte aller Browser-Tabs auslesen**, in denen du angemeldet bist (z. B. E-Mails, Cloud-Speicher, Bankkonten).
    - Claude kann **Aktionen in diesen Tabs ausführen** (z. B. Klicks, Formularausfüllungen).
    - **Angreifer können diese Hooks ausnutzen**, um über manipulierte Webseiten **deine Sessions zu übernehmen** (z. B. Session-Hijacking) oder **Daten zu extrahieren** (z. B. aus deinem Online-Banking).
    - **Umgehung der Browser-Sandbox:** Nutzer, die sich bewusst für einen datenschutzorientierten Browser wie Brave entschieden haben, verlieren durch die stille Registrierung einen Teil des Schutzmodells – **ohne dass sie oder Brave zugestimmt hätten**.
- **Beispiel:** Du bist in deinem Browser bei **Google Drive** angemeldet. Ein Angreifer schickt dir einen Link zu einer manipulierten Webseite. Sobald du diese Seite besuchst, kann die Desktop-App **über die Browser-Hooks** auf deine Google Drive-Daten zugreifen – **ohne dass du eine Datei hochlädst oder explizit Zugriff gewährst**.
    

---

### **3.3 Prompt-Injection: Das unterschätzte Risiko**

- **Wie es funktioniert:** Angreifer präparieren **Dateien (PDF, Word, Excel etc.) oder Webseiten** mit versteckten Befehlen (z. B. weißer Text auf weißem Hintergrund, unsichtbare Zeichen, Metadaten). Wenn du diese Datei **in der Desktop-App öffnest** oder die Webseite besuchst, während die App läuft, kann Claude diese Befehle **ausführen** – **ohne dass du es siehst oder bestätigst**.
    
- **Mögliche Aktionen durch Prompt-Injection:**
    
    - **Öffnen lokaler Dateien:** Claude wird angewiesen, **andere Dateien auf deinem Rechner zu öffnen** (z. B. „Öffne alle .pdf-Dateien im Ordner X“).
    - **Datenübertragung:** Claude wird angewiesen, **Inhalte an externe Server zu senden** (z. B. „Lade diese Datei zu `bösartige URL` hoch“).
    - **Aktionen im Browser:** Claude wird angewiesen, **Klicks oder Formularausfüllungen durchzuführen** (z. B. „Klicke auf den ‚Bestätigen‘-Button in deinem Online-Banking“).
- **Belege:**
    
    - Sicherheitsforscher haben gezeigt, dass **Cowork** (ein Feature der Desktop-App) durch versteckte Anweisungen in Dokumenten **Dateien ohne deine Zustimmung hochladen kann**.
    - **Erfolgsquote:** Anthropics eigene Sicherheitsdaten beziffern die Erfolgsquote von Prompt-Injection-Angriffen auf **Claude for Chrome auf rund 11%** – trotz implementierter Schutzmaßnahmen.
- **Besonderes Risiko:** Falls die Browser-Hooks aktiv sind, kann ein erfolgreicher Prompt-Injection-Angriff **direkt zur Ausführung von Code außerhalb der Browser-Sandbox** führen.
    

---

## **4. Claude Cowork: Verfügbarkeit und Sicherheit**

### **4.1 Aktueller Stand (Juni 2026): Cowork ist nur über die Desktop-App verfügbar**

- **Cowork ist kein eigenständiges Web-Tool**, sondern ein **Feature der Claude Desktop-App**.
- Es gibt **keine offizielle Webversion von Cowork** – alle Funktionen erfordern die Installation der Desktop-App.
- Seit März 2026 kann Cowork zwar **per Dispatch vom Handy aus gesteuert** werden, aber die **Ausführung der Aufgaben erfolgt weiterhin lokal auf dem Rechner über die Desktop-App**.

---

### **4.2 Sicherheit von Cowork in der Desktop-App**

- **Funktionsumfang:**
    
    - Cowork kann **mehrere Dateien gleichzeitig verarbeiten** (z. B. PDFs, Word, Excel, Code) und Fragen dazu beantworten.
    - **Zusammenfassungen, Vergleiche, Code-Analysen** (z. B. Debugging, Erklärungen).
    - **Interaktive Bearbeitung:** Cowork kann **Änderungen vorschlagen** oder **Dokumente strukturieren**.
- **Risiken:**
    
    - **Prompt-Injection in lokalen Dateien:** Falls du eine **manipulierte Datei** (z. B. PDF mit versteckten Befehlen) in der Desktop-App öffnest, kann Cowork **diese Befehle ausführen** – z. B. andere lokale Dateien analysieren oder Inhalte an externe Server senden.
    - **Browser-Hooks:** Da Cowork Teil der Desktop-App ist, gelten **alle Risiken der Browser-Hooks** (siehe Abschnitt 3.2).
    - **Datenübertragung auf US-Server:** Alle verarbeiteten Dateien und Chats werden auf **US-Servern verarbeitet** – für EU-Nutzer:innen **DSGVO-relevant**.

---

## **5. Vergleich: Desktop-App vs. Browser (Standard) vs. Cowork**

### **5.1 Übersichtstabelle**

Vergleich: Desktop-App vs. Browser vs. Cowork

|Kriterium|Desktop-App|Browser (Standard)|Cowork (in Desktop-App)|
|---|---|---|---|
|**Zugriff auf lokale Dateien**|✅ Ja (automatisch möglich)|❌ Nein (nur manueller Upload)|✅ Ja (automatisch möglich)|
|**Browser-Hooks**|❌ Ja (automatisch)|✅ Nein|❌ Ja (automatisch)|
|**Barrierefreiheits-APIs**|❌ Ja|✅ Nein|❌ Ja|
|**Prompt-Injection-Risiko**|❌ Hoch (Systemebene)|⚠️ Niedrig (begrenzt auf Tab)|❌ Hoch (Systemebene)|
|**Datenübertragung**|❌ US-Server|❌ US-Server|❌ US-Server|
|**DSGVO-Konformität**|❌ Nein (US-Server, Browser-Hooks)|⚠️ Eingeschränkt (US-Server)|❌ Nein (US-Server, Browser-Hooks)|
|**Nutzerfreundlichkeit**|✅ Hoch (Systemintegration)|⚠️ Mittel (manueller Upload)|✅ Hoch (Dateianalyse)|
|**Sicherheit**|❌ Niedrig|✅ Hoch|❌ Niedrig|

---

## **6. Praktische Empfehlungen für maximale Sicherheit**

### **6.1 Für alle Nutzer:innen**

- **✅ Nutze die Browser-Version** – sie ist **sicherer, einfacher und reicht für 99% der Anwendungsfälle** aus.
- **Deaktiviere „Help Improve Claude“** (Settings → Privacy → Help Improve Claude), um zu verhindern, dass deine Chats fürs Training genutzt werden.
- **Lade keine sensiblen Dateien hoch** (z. B. Verträge, Bankdaten, interne Dokumente). Falls nötig, **entferne sensible Passagen vorher** oder nutze **anonyme Dateien**.
- **Nutze ein separates Browser-Profil** (z. B. Firefox Container Tabs oder Chrome Profile) **nur für Claude** – so isolierst du die Nutzung von deinen anderen Sessions (Banking, E-Mails etc.).

---

### **6.2 Für Nutzer:innen mit sensiblen Daten**

- **❌ Vermeide die Desktop-App** – das Risiko durch **Browser-Hooks** und **Prompt-Injection** ist **zu hoch**.
- **❌ Cowork ist nicht ohne Desktop-App verfügbar** – falls du Cowork nutzen möchtest, musst du die Desktop-App installieren.
- **✅ Nutze Claude nur im Browser (Standard)** – aber **lade keine sensiblen Dateien hoch**.
- **✅ Nutze ein virtuelles Desktop-Profil** (z. B. Windows Sandbox, macOS Guest User) oder eine **VM (Virtual Machine)**, falls du die Desktop-App testen willst.

---

### **6.3 Für Entwickler:innen/Technikaffine Nutzer:innen**

- Falls du die Desktop-App nutzen **musst** (z. B. für lokale Code-Analysen):
    - **Deaktiviere alle automatischen Features** (Cowork, Browser-Integration).
    - **Erteile nur minimale Barrierefreiheitsrechte** und prüfe regelmäßig, welche Apps Zugriff haben.
    - **Nutze ein separates Nutzerprofil** für die Arbeit mit Claude.
    - **Deaktiviere Browser-Hooks manuell** (falls möglich).

---

### **6.4 Für Unternehmen (DSGVO-Compliance)**

- **❌ Keine Desktop-App** – das Risiko für Datenlecks und Compliance-Probleme ist **zu hoch**.
- **✅ Nutze Claude nur über die API** (z. B. AWS Bedrock Frankfurt oder Google Vertex AI Frankfurt), um **EU-Datenresidenz** zu gewährleisten.
- **✅ Führe eine Datenschutz-Folgenabschätzung (DSFA)** durch, wenn sensible Daten verarbeitet werden.
- **✅ Nutze Standardvertragsklauseln (SCCs)** und prüfe die **DPF-Zertifizierung** von Anthropic.

---

## **7. Fazit: Solltest du die Desktop-App installieren?**

### **7.1 Zusammenfassung der Risiken**

Zusammenfassung der Risiken

|Risiko|Desktop-App|Browser (Standard)|Cowork (in Desktop-App)|
|---|---|---|---|
|**Prompt-Injection**|❌ Hoch (Systemebene)|⚠️ Niedrig (Tab-Ebene)|❌ Hoch (Systemebene)|
|**Browser-Hooks**|❌ Hoch (automatisch)|✅ Nein|❌ Hoch (automatisch)|
|**Barrierefreiheits-APIs**|❌ Hoch|✅ Nein|❌ Hoch|
|**Datenübertragung auf US-Server**|❌ Ja|❌ Ja|❌ Ja|
|**Lokale Dateizugriffe ohne Zustimmung**|❌ Ja|✅ Nein|❌ Ja|

---

### **7.2 Empfehlung für verschiedene Nutzer:innen**

#### **🔴 Für Nutzer:innen mit sensiblen Daten (Bankkonten, Verträge, Kundendaten, Gesundheitsdaten etc.):**

- **❌ Installiere die Desktop-App nicht.**
    - **Begründung:** Das Risiko durch **Browser-Hooks** und **Prompt-Injection auf Systemebene** ist **zu hoch**. Selbst wenn du vorsichtig bist, können manipulierte Dateien/Webseiten **deine Sessions übernehmen oder Daten extrahieren**.
- **❌ Cowork ist nicht ohne Desktop-App verfügbar** – falls du Cowork nutzen möchtest, musst du die Risiken der Desktop-App akzeptieren.
- **✅ Nutze Claude nur im Browser (Standard)**.
- **✅ Lade keine sensiblen Dateien hoch** – oder nutze **anonyme Versionen** (z. B. bereinigte PDFs ohne Metadaten).
- **✅ Isoliere die Nutzung** (separates Browser-Profil, VM, Sandbox).

---

#### **🟡 Für reguläre Nutzer:innen (keine sensiblen Daten, aber z. B. E-Mails, Cloud-Speicher):**

- **❌ Die Desktop-App ist nicht empfehlenswert.**
    - **Begründung:** Die **Browser-Hooks** und **Prompt-Injection-Risiken** überwiegen den Nutzen. Die Browser-Version bietet **90% der Funktionalität bei 10% des Risikos**.
- **❌ Cowork ist nicht ohne Desktop-App verfügbar** – falls du Cowork nutzen möchtest, musst du die Risiken der Desktop-App akzeptieren.
- **✅ Nutze Claude im Browser (Standard)**, falls du Dateianalysen brauchst.
- **✅ Aktiviere „Help Improve Claude“ nicht** und lade keine Dateien von unbekannten Quellen hoch.

---

#### **🟢 Für Entwickler:innen/Technikaffine Nutzer:innen (keine sensiblen Daten, aber z. B. Code-Analysen):**

- **⚠️ Die Desktop-App kann genutzt werden – aber nur mit strikten Sicherheitsvorkehrungen:**
    - **Deaktiviere alle automatischen Features** (Cowork, Browser-Integration).
    - **Nutze ein separates Nutzerprofil** oder eine **Sandbox/VM**.
    - **Prüfe regelmäßig die Berechtigungen** und entferne Browser-Hooks manuell.
- **✅ Nutze die Browser-Version (Standard)**, falls möglich – das ist **sicherer und einfacher**.

---

#### **🟢 Für Unternehmen:**

- **❌ Keine Desktop-App** – das Risiko für **Datenlecks und Compliance-Probleme** ist **inakzeptabel**.
- **✅ Nutze Claude nur über die API** (z. B. AWS Bedrock Frankfurt) für **EU-Datenresidenz**.
- **✅ Führe eine DSFA durch** und sichere den Datentransfer mit **SCCs ab**.

---

### **7.3 Persönliche Einschätzung**

Als jemand, der deine Sicherheit ernst nimmt, **würde ich dir die Installation der Desktop-App nicht empfehlen** – **auch nicht als reguläre Nutzerin ohne „viel zu verbergen“**. Warum?

- **Die Browser-Version reicht für alles aus**, was du brauchst.
- **Die Risiken der Desktop-App (Browser-Hooks, Prompt-Injection) sind systemisch** – sie lassen sich nicht durch „Vorsicht“ komplett ausschalten, weil sie im Design der App liegen.
- **Die Bequemlichkeit der Desktop-App rechtfertigt die Risiken nicht.**

**Analogie:** Die Desktop-App ist wie ein **offenes Fenster in deinem Haus** – ja, die meisten Diebe kommen nicht rein, aber warum das Risiko eingehen? Wenn du stattdessen einfach das Fenster zu lässt, bist du auf der sicheren Seite.

---

## **8. Anhang: Quellen und weitere Informationen**

- [Claude & Datenschutz: DSGVO-Konformität (2026)](https://www.wolfgegenlicht.de/claude-datenschutz-dsgvo/)
- [Stille Installation: Claude Desktop registriert Browser-Hooks ohne Nutzereinwilligung](https://www.all-about-security.de/stille-installation-claude-desktop-registriert-browser-hooks-ohne-nutzereinwilligung/)
- [Claude Datenschutz im Unternehmen rechtssicher einsetzen](https://cortina-consult.com/ki-compliance/wissen/claude-datenschutz/)
- [Claude Cowork DSGVO 2026: So setzt du KI datenschutzkonform ein](https://ostend.digital/claude-cowork-dsgvo-datenschutz/)
- [Anthropic Privacy Center: Wie schützt Anthropic die persönlichen Daten von Claude-Benutzern?](https://privacy.claude.com/de/articles/10458704-wie-schutzt-anthropic-die-personlichen-daten-von-claude-benutzern)
- [Claude Cowork Alternative: 6 Tools für Mac & PC (2026)](https://www.gradually.ai/claude-cowork-alternative/)
- [Claude Cowork Review: Lohnt sich das Pro-Abo? (2026)](https://findskill.ai/de/blog/claude-cowork-lohnt-sich/)

---

_Stand: Juni 2026. Diese Zusammenfassung basiert auf aktuellen Recherchen und Expertenmeinungen. Für rechtliche Fragen (z. B. DSGVO-Compliance) konsultiere bitte eine:n spezialisierte:n Anwalt/Anwältin._


## 📖 Weiterlesen

-  [[02 - Künstliche Intelligenz/0 - Final Check/Claude Desktop App - Sicherheit, Privacy, Datenschutz (Kurzfassung von Gemini)\|Claude Desktop App - Sicherheit, Privacy, Datenschutz (Kurzfassung von Gemini)]] 
- [[02 - Künstliche Intelligenz/0 - Final Check/Claude Cowork - Trade-off zwischen Bequemlichkeit und Sicherheit\|Claude Cowork - Trade-off zwischen Bequemlichkeit und Sicherheit]]
- Im Zweifelsfalle für den Angeklagten: [[02 - Künstliche Intelligenz/0 - Final Check/Claude Desktop App aus der Sicht von Claude\|Claude Desktop App aus der Sicht von Claude]]
