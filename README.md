# imcm-mitschrift.1bhk

Das ist das README.md File unseres Repositories. Die Dateieendung .md steht für Markdown - eine heute sehr weit verbreitete [Auszeichnungssprache] (https://de.wikipedia.org/wiki/Auszeichnungssprache) Weitere bekannte Auszeichnungssprachen sind:

-Hypertext Markup Language (HTML)
-Extensible Markup Language (XML)
-Yet Another Markup Language (YAML, YML)

> **ACHTUNG!**
> Die Abkürzung ML steht nicht immer für _Markup Language_, sie kann auch _Machine Learning_ heißen.

## Playlist zur funktionsweise des Internets

![TCP-IP-Modell](/assets/wa.png)

### Teil 1 - What is the Internet?

- Das internet wurde in den 1970er-Jahren entwickelt

- Motivation : Schaffung eines dezentralen Netzwerks, das auch nach einem Atomschlag noch funktioniert ( Kontext des Kalten Krieges)

- Funktionsweise: Paketvermittlung (_Packet Switching_) - Nachrichten bzw. Dateien werden in kleine Pakete aufgeteilt und unabhängig voneinander über das Netzwerk verschickt

- Internet ist eigentlich: das Netz der Netze - besteht aus vielen kleineren Netzen unterschiedlicher Internetanbieter (_Internet Service Provider - ISP_, z.B.: Salzburg AG, Magenta, A1, ...)

### Teil 2 - Internet: Wires, Cables & WiFi

Informationen werden im Internet als Bits übertragen. Bits haben 2 Werte: 0 und 1. 8 Bits zusammengefasst ergeben 1 Byte. Mit einem Byte kann man 256 verschiedene Werte speichern (2^8).

Bits können über verschiedene Übertragungsmediean zwischen computern versendet werden. die Anzahl der übrtragenen Bits pro Sekunde wird als **Bandbreite** bezeichnet. Bei einer Bandbreite von 300MBit/s können beispielsweise 300 Millionen Bit pro Sekunde über die Leistung laufen.
Übertragungsmedien können sein :

**1. Elektrizität / Kupferdraht (Ethernet)**

- billig
- einfach in der Verarbeitung
- weit verbreitet
- hohe verluste über mittlere und lange Distanzen (hunderte Meter)

**2. Licht / Glasfaserkabel**

- schnelle Übertragung
- verlustfrei
- geeignet für Ozeankabel
- relativ teuer und schwierig in der Verarbeitung

**3. Funk / Radiowellen**

- hohen Komfort, Internet überall

### Teil 3 - Internet: Ip-Adressen & DNS

- Protokolle sind die regeln der Kommunikation
- eines der wichtigsten Protokolle im Internet ist das Internet Protocol (IP)
- jedes Gerät im Internet hat zumindest eine (eindeutige) IP- Adresse, viele Geräte haben aber eine externe IP (ähnlich wie die Hausnummer) und eine interne IP (ähnlich wie die Raumnummer)
- Das Domain Name System (DNS) übersetzt menschenlesbare Domainnamem (zb.: www.google.com) in IP-Adressen
- DNS-Server führen Tabellen mit Domainnamen und den entsprechenden IP-Adressen

### Teil 4 - Packets, Routing & Reliability

- über das Internet versendete Daten werden in Pakete aufgeteilt
- einzelne Pakete haben eine Größe von ca. 1,5kB. D. h., ein Foto mit einer größe von 10 MB wird in ca. 6700 Pakete aufgeteilt bevor es über das Internet versendet wird
- Pakete können unterschiedliche Routen durch das Internet nehmen. Die Route wird je nach Auslastung, Störungen etc. durch spezielle Computer - die Router - dynamisch betimmt.
- jedes Packet enthält die Quell- und Ziel-IP-Adresse sowie eine eindeutige Paketnummer
- das _Transmission Control Protocol_ (TPC) prüft am Ziel, ob alle Pakete einer Übertragung angekommen sind, Falls nPakete fehlen, fordert es diese erneut vom Absender an.
- TCP und IP bilden gemeinsam das Rückgrat des Internets. Man spricht daher auch vom TCP/IP- Modell bzw. _TCP/IP-Stack_.

### Teil 5 - The Internet: HTTP & HTML

- HTTP steht für _Hypertext Transfer Protocol_. HTTP arbeitet nach dem Client-Server-Prinzip:

  - ein Web-Client (browser) sendet eine Anfrage (_Request_) an einen Web-Server
  - der Web-Server verarbeitet die Anfrage und sendet eine Antwort (_response_) zurück. Die Antwort enthält u.a. einen sogenannten [HTTP-Statuscode] (https://de.wikipedia.org/wiki/HTTP-Statuscode), der Auskunft über die Verarbeitung der Anfrage gibt.

  #### HTTP-Statuscodes

  **1xx** - die Anfrage dauert noch an
  **2xx** - die Anfrage war erfolgreich
  **3xx** - Um- oder Weiterleitung
  **4xx** - Clientfehler (z.B. 404 - _Page not found_)
  **5xx** - Serverfehler 💀

- HTTP-Anfragen werden immer mit einer **HTTP-Methode** übertragen
  -Daten (HTML-Seiten,Bilder, Videos,...) werden mit GET-Anfragen angefordert
- Benutzereingaben (z.B aus Formularfelden - z.B. Passwort, Datei-Uploades,...) werden mit POST-Anfragen verschlüsselt versendet
  -es gibt auch andere HTTP-Methoden. Diese lernen wir aber erst später.
  -HTTP-Anfragen und Antworten können auch **Cookies** enthhalten. Cookies sind kleine Textdateien, die aus Schlüssel-Wert-Paaren (_key-value-pairs_) bestehen. Sie werden bei jeder Anfrage vom Client mitgesendet und ermöglichen so u.a. die Identifikation einzelner Nutzer.

### Teil 8 - The internet: How Search Works

- Suchmaschienen-Bots (Crawler) durchstreifen ständig das WWW und katalogisieren Websites. Der entstehende Katalog wird auc **Index**
  genannt.
- Wenn wir einen Suchbegriff bei Google (oder einer anderen _Search Engine_) eingeben, wird NICHT das WWW durchsucht, sondern lediglich der zuvor erstellte Index
- Suchergebnisse werden auf Basis eines (geheimen) Algorithmus geranked - Ergebnisse die weiter oben stehen, werden öfter angeklickt
- Einfluss auf das Ranking haben u.a.:
  - im Text vorkommende Suchbegriffe (_Keywords_)
  - Links die auf meine Seite zeigen (_Backlinks_)
- die Suchergebnisse werden an die Benutzer\*innen angepasst! D.h.: nicht jede/r sieht die gleichen Informationen, selbst wenn sie Indente Suchanfragen durchführen!
- [Startpage] (//https://www.startpage.com/) ist eine datensparsame Suchmaschiene, die ihren Benutzern\*innen die Verwenfung von Google ohne Tracking oder Personalisierung erlaubt
