---
{"title":"Eine kurze Geschichte des Internets","aliases":null,"tags":null,"gen_ai_anteil":["Claude 80%"],"created":"2026-09-21","updated":null,"status":null,"dg-publish":true,"permalink":"/02-kuenstliche-intelligenz/3-work-on-tomorrow/eine-kurze-geschichte-des-internets/","dgPassFrontmatter":true,"dg-note-properties":{"title":"Eine kurze Geschichte des Internets","aliases":null,"tags":null,"gen_ai_anteil":["Claude 80%"],"created":"2026-09-21","updated":null,"status":null}}
---


# Eine kurze Geschichte des Internets

## Am Anfang war der Hypertext

1945, der Zweite Weltkrieg geht gerade zu Ende. Die wenigen Computer, die es gibt, füllen ganze Räume und können kaum mehr als rechnen. Und dennoch träumen schon damals Menschen davon, Texte miteinander zu verknüpfen.

- **1945 – Vannevar Bush skizziert den „Memex“:** Der US-Wissenschaftler beschreibt in seinem Essay *As We May Think* eine Schreibtisch-Maschine, in der man Bücher, Notizen und Fotos speichert und über selbst angelegte „Pfade“ miteinander verbindet. Die Maschine existierte nur auf dem Papier, aber sie hat Generationen von Informatikern inspiriert.
- **1965 – Ted Nelson erfindet ein Wort:** Er prägt den Begriff „Hypertext“ und entwirft mit seinem Projekt Xanadu ein weltweites System aus verknüpften Dokumenten. Fertig wurde es nie – aber der Name ist geblieben.
- **1968 – Douglas Engelbart bringt Hypertext zum Laufen:** In San Francisco führt er vor rund tausend Zuschauern sein System NLS vor. Zum ersten Mal sieht das Publikum Hypertext in Aktion: Texte, die per Mausklick auf andere Texte verweisen. Nebenbei präsentiert er Dinge, die damals kaum jemand für möglich hielt: die Maus, Fenster auf dem Bildschirm, gemeinsames Bearbeiten von Texten und sogar eine Videokonferenz. Später bekommt der Auftritt den Spitznamen „Mother of All Demos“, die Mutter aller Vorführungen.

Was noch fehlte: ein Netz, über das Computer an verschiedenen Orten miteinander kommunizieren konnten.

> [!info] Was ist Hypertext?
>
> Text, der über Links mit anderen Texten verbunden ist. Ein Buch hat eine feste Reihenfolge: Seite folgt auf Seite. Hypertext ist dagegen ein Netz, in dem du per Klick von Text zu Text springst. Das ganze Web ist Hypertext – und dieser Garten auch. 
> 
> ![Hypertext vs Buch.png](/img/user/02%20-%20K%C3%BCnstliche%20Intelligenz/Garten%20erkunden/Bilder/Hypertext%20vs%20Buch.png)


## Das ARPANET: Computer lernen, miteinander zu reden

Dieses Netz entsteht Ende der 1960er in den USA – bezahlt vom Militär, gebaut von Universitäten.

- **1958 – Der Sputnik-Schock:** Die Sowjetunion hat wenige Monate zuvor den ersten Satelliten ins All geschossen, die USA fühlen sich technisch abgehängt. Als Antwort gründet das Verteidigungsministerium die ARPA (Advanced Research Projects Agency), eine Behörde, die Spitzenforschung finanziert.
- **1969 – Es geht LO…:** Am 29. Oktober 1969 sollen zum ersten Mal zwei Rechner über das neue Netz Daten austauschen. Ein Student an der Universität von Los Angeles (UCLA) will sich dafür auf einem Rechner am Stanford Research Institute einloggen[^Engelbart], rund 500 Kilometer entfernt. Er möchte „LOGIN“ eintippen, doch nach „L“ und „O“ stürzt das System ab. Die allererste Nachricht im Vorläufer des Internets lautet also: „LO“.
- **Ende 1969 – vier Rechner, ein Netz:** Zum Jahresende sind vier Universitätsrechner miteinander verbunden. In den folgenden Jahren wächst das ARPANET auf Dutzende, später Hunderte Rechner.
- **1971 – Die erste E-Mail:** Der Programmierer Ray Tomlinson schickt die erste Nachricht von einem Rechner zu einem anderen. Die Adresse muss dabei zweierlei verraten: an wen die Nachricht geht und auf welchem Rechner diese Person zu finden ist. Um beides sauber zu trennen, wählt Tomlinson ein Zeichen, das in Namen nie vorkommt: das @. E-Mail wird schnell zur beliebtesten Anwendung im ARPANET.

### Mythos-Check: Gebaut für den Atomkrieg?

Die Legende, das Internet sei entwickelt worden, um einen Atomkrieg zu überstehen, hält sich hartnäckig. Das stimmt nur teilweise. Das ARPANET sollte vor allem teure Großrechner für Forschende an verschiedenen Orten nutzbar machen, denn Rechenzeit war knapp und kostbar. Einen wahren Kern hat die Legende aber: Die Paketvermittlung geht unter anderem auf den Ingenieur Paul Baran zurück, der Anfang der 1960er im Umfeld des US-Militärs an einem Kommunikationsnetz forschte, das auch einen Atomangriff übersteht.[^Paul-Baran] Die Technik war also teils militärisch inspiriert, der Zweck des ARPANET vor allem wissenschaftlich.

> [!info] Was ist Paketvermittlung?
>
> Stell dir vor, du willst ein Buch verschicken, aber die Post nimmt nur Postkarten. Also schreibst du jede Seite auf eine eigene Karte, nummerierst sie und wirfst sie ein. Jede Karte kann einen anderen Weg nehmen, beim Empfänger werden sie wieder sortiert. Genau so reisen Daten bis heute durchs Internet: zerlegt in kleine Pakete. Fällt eine Leitung aus, nehmen die Pakete einfach eine andere.

Das ARPANET bekam bald viele Geschwister: Überall entstanden weitere Netze. Nur verstanden sie sich nicht besonders gut – sie sprachen nicht dieselbe Sprache.

## TCP/IP: Eine gemeinsame Sprache für alle Netze

Damit sich die Netze untereinander verständigen konnten, brauchte es Regeln, die jedes von ihnen verstand, egal welche Technik darin steckte.

- **1974 – Eine neue Sprache entsteht:** Die US-Informatiker Vint Cerf und Bob Kahn veröffentlichen das Konzept für TCP/IP, über das sich beliebige Netze zusammenschließen lassen. Aus dem englischen „internetworking“, dem Zusammenschalten von Netzen, wird später der Name: Internet. Cerf und Kahn gelten heute als „Väter des Internets“.
- **1983 – Der große Umstellungstag:** Am 1. Januar 1983 stellen alle Rechner im ARPANET auf TCP/IP um. Das Datum gilt oft als Geburtstag des Internets.
- **1983 – Namen statt Nummern:** Jeder Rechner im Internet hat eine Nummer, die IP-Adresse, zum Beispiel 192.0.2.44. Weil sich Menschen Namen leichter als Zahlenreihen merken können, wird das DNS (Domain Name System) erfunden. Es funktioniert wie eine Art Telefonbuch: Du tippst einen Namen wie wikipedia.org, das DNS schlägt die passende Nummer nach.
- **1984 – Das Internet erreicht Deutschland:** Am 3. August 1984 übermittelt das noch junge Netz die erste E-Mail an die Universität Karlsruhe: ein Willkommensgruß aus den USA.
- **1990 – Das ARPANET wird abgeschaltet:** Seine Aufgabe ist erledigt. Das Internet besteht längst aus vielen anderen Netzen und braucht seinen Vorläufer nicht mehr.

> [!info] Was ist TCP/IP?
>
> Ein **Protokoll** ist eine Sammlung fester Regeln, an die sich alle Beteiligten halten, damit Kommunikation funktioniert. TCP/IP sind eigentlich zwei Protokolle, die zusammenarbeiten. Bleiben wir bei den Postkarten aus dem letzten Abschnitt:
>
> - **IP (Internet Protocol)** ist die Adresse auf jeder Karte. Es sorgt dafür, dass jedes Paket seinen Weg zum richtigen Rechner findet.
> - **TCP (Transmission Control Protocol)** ist der sorgfältige Absender und Empfänger. Es nummeriert die Karten, prüft, ob alle angekommen sind, fordert fehlende nach und bringt sie wieder in die richtige Reihenfolge.

### Wie sah das Internet ohne Web aus?

Das Internet stand also. Aber es war ein Ort für Fachleute, Seiten zum Anklicken gab es nicht. Stattdessen gab es mehrere einzelne Dienste, jeder mit eigenem Programm und eigenen Befehlen:

- **E-Mail:** Nachrichten verschicken, lange die mit Abstand beliebteste Anwendung.
- **Telnet:** Man loggt sich aus der Ferne auf einem anderen Rechner ein und arbeitet dort per Befehl, als säße man davor. So ließen sich zum Beispiel die Bibliothekskataloge anderer Universitäten durchsuchen.
- **FTP (File Transfer Protocol):** Dateien von einem anderen Rechner herunterladen. Man hangelte sich per Befehl durch dessen Ordner, holte sich etwa einen Forschungsbericht und las ihn dann auf dem eigenen Rechner.
- **Usenet:** Tausende Diskussionsforen, nach Themen sortiert in sogenannte Newsgroups. Hier wurde gefragt, gefachsimpelt und gestritten – das soziale Netzwerk seiner Zeit.

Das größte Problem: Man musste vorher wissen, auf welchem Rechner und in welchem Ordner etwas lag. Fundorte sprachen sich allenfalls per E-Mail oder im Usenet herum; kein Dokument konnte auf ein anderes verweisen. Das Internet glich einer riesigen Bibliothek ohne Katalog: Wer den Regalplatz kannte, kam ran. Alle anderen hatten Pech.

Das sollte sich bald ändern, denn das Web stand schon vor der Tür. 

> [!info] Was ist ein Terminal?
>
> Maus, Fenster, Symbole zum Anklicken: Für uns ist eine schicke Benutzeroberfläche selbstverständlich. Engelbart hatte sie zwar schon 1968 vorgeführt, im Alltag setzte sie sich aber erst ab Mitte der 1980er durch. Davor arbeitete man am **Terminal**: einem Bildschirm mit Tastatur, auf dem nur Text zu sehen war. Man tippte einen Befehl ein, drückte Enter, und der Computer antwortete in Textzeilen.
> 
> ![Terminal.png](/img/user/02%20-%20K%C3%BCnstliche%20Intelligenz/Garten%20erkunden/Bilder/Terminal.png)
>
> Ganz verschwunden ist das Terminal übrigens nie: Als Programm steckt es bis heute in jedem Computer. Für Programmierer gehört es zum Alltag, und mit der zunehmenden Popularität von [[02 - Künstliche Intelligenz/3 - Work on tomorrow/Vibecoding\|Vibecoding]] entdecken es auch mehr und mehr Nicht-Techies.

## Das World Wide Web: Ein Geschenk an die Welt

Ende der 1980er arbeitet Tim Berners-Lee am CERN, dem europäischen Forschungszentrum für Teilchenphysik bei Genf. Dort herrscht ein ständiges Kommen und Gehen: Forschende aus aller Welt arbeiten ein paar Jahre mit und ziehen dann weiter, ihr Wissen oft mit ihnen. Was an Unterlagen bleibt, liegt verstreut auf unzähligen Computern unterschiedlicher Bauart, die kaum miteinander kompatibel sind. Wer etwas sucht, muss erst einmal herausfinden, wer es weiß und auf welchem Rechner es liegt. Berners-Lee hat eine Idee: Was, wenn man all diese Dokumente per Link miteinander verknüpft, ganz gleich, wo sie gespeichert sind? Die alte Hypertext-Vision, verbunden mit dem Internet.

- **1989 – „Vage, aber spannend“:** Berners-Lee reicht bei seinem Chef einen Vorschlag für ein verlinktes Informationssystem ein. Der notiert darauf nur drei Wörter: „Vague but exciting“. Das reicht, um weitermachen zu dürfen.
- **1990 – Drei Erfindungen auf einen Streich:** Berners-Lee entwickelt die Bausteine, auf denen das Web bis heute läuft: [[02 - Künstliche Intelligenz/0 - Final Check/HTML (Hypertext Markup Language)\|HTML]], HTTP und die URL. Dazu programmiert er den ersten Browser und den ersten [[Server\|Webserver]]. Auf dem Server-Rechner klebt ein Zettel: „This machine is a server. DO NOT POWER IT DOWN!!“ – wer ihn ausschaltet, schaltet das komplette Web ab.
- **1991 – Das Web stellt sich vor:** Die erste Webseite geht unter der Adresse [info.cern.ch](https://info.cern.ch/) online. Ihr Thema: das World Wide Web selbst – was es ist und wie man mitmacht. Sie ist bis heute abrufbar. [^erste-Webseite]
- **1993 – Das Geschenk:** Am 30. April 1993 gibt das CERN die Technik des Webs frei, ohne Patente und ohne Lizenzgebühren. Jeder darf nun Browser, Server und Webseiten bauen, ohne jemanden um Erlaubnis zu fragen oder zu bezahlen.

> [!info] Die drei Bausteine des Webs
>
> - **HTML (Hypertext Markup Language)** beschreibt, wie eine Seite aufgebaut ist: Überschriften, Absätze, Links.
> - **URL (Uniform Resource Locator)** gibt an, wo eine Seite zu finden ist, zum Beispiel [https://info.cern.ch](https://info.cern.ch). Der Name darin, hier `info.cern.ch`, wird per DNS in die IP-Adresse übersetzt (die Nummer des Rechners, auf dem die Seite liegt).
> - **HTTP (Hypertext Transfer Protocol)** regelt, wie Browser und Server sich unterhalten: Der Browser fragt „Gib mir bitte diese Seite“, der Server schickt sie.

Jetzt konnte also jeder mitbauen. Nur sah das Web noch ziemlich karg aus: Text, Links, kaum Bilder. Aber nicht mehr lange.


## Vom Forschungsnetz zum Massenmedium

Ab Mitte der 1990er geht alles sehr schnell. Innerhalb weniger Jahre wird aus dem Werkzeug für Forschende ein Alltagsmedium für Milliarden Menschen.

- **1993 – Bilder mitten im Text:** Studierende an der University of Illinois entwickeln den Browser Mosaic, der Bilder direkt zwischen den Text setzt. Plötzlich sieht eine Webseite aus wie eine Zeitschrift und nicht mehr wie ein Fachdokument. Das Web wird für normale Menschen interessant.
- **Mitte der 1990er – Der Browserkrieg:** Der Browser Netscape Navigator erobert den Markt. Microsoft antwortet mit dem Internet Explorer, legt ihn jedem Windows-Rechner kostenlos bei – und gewinnt. Ein Schachzug, der Microsoft später eine Klage der US-Justiz wegen Missbrauchs seiner Marktmacht einbringt.
- **Ende der 1990er – Goldrausch und Crash:** Amazon, eBay und Google werden gegründet. Anleger stecken Milliarden in fast jede Firma mit „.com“ im Namen. Im Jahr 2000 platzt die sogenannte Dotcom-Blase, viele Firmen verschwinden wieder.
- **1996 – Schönes Design für alle:** Im Browserkrieg sieht dieselbe Webseite im Netscape Navigator oft ganz anders aus als im Internet Explorer. Aus diesem Grund wird [[02 - Künstliche Intelligenz/0 - Final Check/CSS (Cascading Style Sheets)\|CSS]] eingeführt: eine gemeinsame Sprache für Farben, Schriften und Anordnung. HTML ist nun ausschließlich für die Struktur zuständig, CSS für das Aussehen.
- **2000er – Das Mitmach-Web:** Mit Wikipedia (2001), Facebook (2004) und YouTube (2005) werden Nutzerinnen und Nutzer selbst zu Autoren. Dafür setzt sich der Begriff „Web 2.0“ durch.
- **2007 – Das Netz wird mobil:** Mit dem iPhone beginnt der Siegeszug der Smartphones. Wer bislang online sein wollte, setzte sich an den Computer. Jetzt reicht ein Griff in die Hosentasche.

> [!info] Was ist ein Browser?
>
> Ein Browser (engl. „to browse“, stöbern) ist ein Programm wie Firefox, Chrome oder Safari, mit dem du Webseiten ansiehst. Er fragt per HTTP beim Server nach einer Seite, bekommt HTML und CSS zurück und baut daraus die Seite, die du auf dem Bildschirm siehst.

Heute[^Stand 2025] nutzen rund 6 Milliarden Menschen das Internet, etwa drei Viertel der Weltbevölkerung. 2,2 Milliarden sind allerdings noch immer offline. Und das Netz, das einmal als offenes Projekt von Forschenden begann, sieht heute ziemlich anders aus, als seine Erfinder es sich vorgestellt hatten.

## Und heute? Zwischen Plattformen und KI

Das Web wurde als offenes, dezentrales System gebaut: Jeder kann eine Seite veröffentlichen und auf jede andere verlinken, niemand muss um Erlaubnis fragen. Gut dreißig Jahre später sieht die Wirklichkeit anders aus.

- **Wenige Konzerne, viel Macht:** Ein großer Teil dessen, was Menschen online tun, läuft heute über wenige große Tech-Konzerne. Ihnen gehören die wichtigsten Suchmaschinen, sozialen Netzwerke, Online-Shops und App-Stores. Und auch wo das Web vielfältig wirkt, hängt vieles an genau diesen Konzernen: Unzählige Websites und Apps laufen auf ihren Servern, in der sogenannten „Cloud“. Statt frei im Web zu stöbern, bewegen sich viele Menschen vor allem innerhalb einzelner Apps.
- **Das Web als Trainingsmaterial:** Große Sprachmodelle wie ChatGPT oder Claude lernen zu einem großen Teil aus Texten, die frei im Web stehen. Programme, sogenannte Crawler, durchforsten dafür automatisch Milliarden Webseiten. Ob das ohne Erlaubnis und Bezahlung erlaubt ist, beschäftigt inzwischen Gerichte in vielen Ländern. Autoren, Künstler und Verlage wehren sich, und viele Websites sperren die Crawler aus.
- **Von Links zu Antworten:** Suchmaschinen und KI-Assistenten liefern immer öfter direkt eine fertige Antwort, statt auf Quellen zu verlinken. Für Lesende ist das bequem. Für die Webseiten, auf denen die Antworten beruhen, bedeutet es oft weniger Besuche. Die Grundidee des Hypertexts – von Text zu Text springen – rückt dabei ein Stück in den Hintergrund.

> [!info] Was ist ein Walled Garden?
>
> Ein „ummauerter Garten“: eine Plattform, die ihre Nutzer, Inhalte und Daten möglichst innerhalb der eigenen Mauern hält. Man merkt es an Kleinigkeiten: Beiträge lassen sich nur mit Konto lesen, eigene Daten kann man nicht zu einem anderen Dienst mitnehmen, Apps gibt es nur über den hauseigenen Store. Typische Beispiele sind soziale Netzwerke und App-Stores. Das Gegenmodell ist das offene Web, in dem jede Seite auf jede andere verlinken kann.

### Aber es besteht auch Hoffnung

- **Ritter ohne Furcht und Tadel:** Tim Berners-Lee warnt seit Jahren genau vor dieser Entwicklung: Das Web, das er als offenes Netz für alle gebaut hat, ist zu großen Teilen in die Hände weniger Konzerne geraten. Aus Nutzern sind Datenlieferanten geworden, und die lautesten Inhalte gewinnen, nicht die faktisch richtigen. Mit dem Projekt Solid arbeitet Berners-Lee an einer Technik, mit der Menschen die Kontrolle über ihre eigenen Daten zurückbekommen sollen. 2025 erschienen seine Erinnerungen unter einem Titel, der sein Lebenswerk zusammenfasst: _[[This Is for Everyone\|This Is for Everyone]]_ (wörtlich: _Das ist für alle_).

- **Gegenbewegungen:** Dezentrale Netzwerke wie das [[Fediverse\|Fediverse]] (bekanntester Dienst: Mastodon) setzen auf viele unabhängige Server statt einer zentralen Firma. Und die IndieWeb-Bewegung ruft dazu auf, Texte zuerst auf der eigenen Website zu veröffentlichen statt auf Plattformen, etwa als Blog oder als Digital Garden wie dieser hier. Beide knüpfen damit an die ursprüngliche Idee des Webs an.


> [!quote] Sir Tim
>
> 2004 wurde Tim Berners-Lee von Queen Elizabeth II. zum Ritter geschlagen, „für Verdienste um die weltweite Entwicklung des Internets“. Seitdem heißt er offiziell Sir Tim Berners-Lee. Völlig verdient, wie ich finde: Nicht nur hat er der Welt das Web geschenkt, er setzt sich auch bis heute dafür ein, dass es offen bleibt. Ein echter Edelmann eben.




## Die Zukunft

… ist ungewiss. Sicher ist nur: Sie wird von uns allen geschrieben.

[^Paul-Baran]: 

[^erste-Webseite]: 🕵️ Um genau zu sein: Das Original von 1991 gibt es nicht mehr. Die Seite wurde damals ständig überarbeitet, und niemand dachte daran, eine Kopie aufzuheben. Wer hätte auch ahnen können, dass sie einmal Geschichte schreibt? 2013 hat das CERN sie anhand der ältesten erhaltenen Fassung wiederhergestellt. Was du dort siehst, ist also nicht die allererste Seite, aber ziemlich nah dran.

[^Engelbart]: Fun Fact: Der Rechner stand in Douglas Engelbarts Labor. Genau, der Mann mit der Mutter aller Vorführungen. Sein Team betreute später auch das erste Verzeichnis des ARPANET, eine Art Auskunftsstelle, wer im Netz wo zu finden ist.

[^Paul-Baran]: Stand 2025, laut der Internationalen Fernmeldeunion (ITU), einer Organisation der Vereinten Nationen.