# Aufgabe 1: 

Der Browser sucht mithilfe des DNS-Servers die passende IP-Adresse zur Internetadresse.

Der Browser verbindet sich über das Internet mit dem Server der Schule.

Der Browser sendet eine Anfrage an den Server, um die Startseite abzurufen.

Der Server schickt die Daten der Webseite zurück.

Der Browser verarbeitet die Daten und zeigt die fertige Startseite auf dem Bildschirm an.

---

# Aufgabe 2: 


1. **`[http://www.beispiel.de/bilder/tux.png](http://www.beispiel.de/bilder/tux.png)`**
* **Protokoll:** `http`
* **Domain-Name:** `www.beispiel.de`
* **Pfad:** `/bilder/tux.png`


2. **`[https://www.w3.org/standards/](https://www.w3.org/standards/)`**
* **Protokoll:** `https`
* **Domain-Name:** `www.w3.org`
* **Pfad:** `/standards/`


3. **`[https://wiki.selfhtml.org/wiki/HTML](https://wiki.selfhtml.org/wiki/HTML)`**
* **Protokoll:** `https`
* **Domain-Name:** `wiki.selfhtml.org`
* **Pfad:** `/wiki/HTML`

---

# Aufgabe 3:

Hier ist eine ganz kurze Zusammenfassung:

* **URL-Zerlegung:** Eine Adresse teilt sich in das **Protokoll** (z. B. `https`), den **Domain-Namen** (z. B. `example.com`) und den **Pfad** (z. B. `/bilder/tux.png`).
* **DNS / `nslookup`:**
* Die Hauptdomain (`example.com`) ist die Apex-Domain.
* Eine Subdomain (`[www.example.com](https://www.example.com)`) verweist oft über einen Alias (CNAME) auf die Hauptadresse. Bei vielen Domains liefern beide Abfragen dieselbe IP-Adresse.

---

# Aufgabe 4:

### 1. DNS-Abfrage (nslookup)

Mit dem Befehl `nslookup` in der Eingabeaufforderung lässt sich die IP-Adresse einer Domain herausfinden.

* Die oberste Zeile Server zeigt den DNS-Server, der zuerst gefragt wurde (z. B. der Heim-Router).
* Die Adresse darunter zeigt die zugehörige IP-Adresse des Webservers.



### 2. Der Weg einer Anfrage (Schritt für Schritt)

Wenn du eine URL in den Browser eintippst, läuft im Hintergrund folgender Prozess ab:

1. **DNS-Abfrage:** Der Browser fragt beim DNS nach der IP-Adresse, die zum Domain-Namen gehört.
2. **HTTP-Anfrage:** Der Browser schickt eine Anfrage an die gefundene IP-Adresse des Webservers und teilt mit, welche Datei (z. B. `/`) er haben möchte.
3. **Server-Antwort:** Der Webserver sucht die angeforderte Datei und sendet sie als Antwort an den Browser zurück.
4. **Rendering:** Der Browser liest das HTML-Dokument (sowie nachgeladene Dateien wie CSS, Bilder oder Videos) und baut daraus die sichtbare Webseite zusammen.


### 3. Internet vs. World Wide Web (WWW)

* **Das Internet:** Das weltweite physische Netzwerk aus miteinander verbundenen Rechnern und Infrastrukturen.
* **Das World Wide Web (WWW):** Nur einer von vielen Diensten, die über das Internet laufen – konkret der Dienst, der Webseiten bereitstellt (neben E-Mail, Chats etc.).