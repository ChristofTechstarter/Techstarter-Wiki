# Netzwerk-Wiki
## Netzwerkarten
- `WAN`: Wide Area Network: Ein zusammenschluss von mehreren einzelnen Netzwerken
___
- `LAN`: Local Area Network: Ein auf ein bestimmten Bereich (z.B. Wohnhaus oder Büro) beschränktes Netzwerk
___
- `PAN`: Personal Area Network: Ein "Persönliche" Netzwerk mit geringer Reichweite, z.B. Kopfhörer mit Smartphone oder Tastatur mit Rechner
___
## Addressen
### IP-Addresse:
- Eine Internet Protocol-Adresse ist eine Art digitale Adresse, die Geräten hilft, miteinander im Internet oder in einem Netzwerk zu kommunizieren. Jedes Gerät, das mit einem Netzwerk verbunden ist, wie ein Computer, ein Smartphone oder ein Drucker, braucht eine IP-Adresse, um Daten senden und empfangen zu können.
___
### MAC-Addresse: 
- Eine Media Access Control-Adresse ist eine Art serienmäßige Kennung, die jedem Gerät, das sich mit einem Netzwerk verbinden kann, zugewiesen wird. Sie ist einzigartig und wird von dem Hersteller des Geräts festgelegt.
- Sie besteht aus 6 Paaren im hexadezimalsystem, getrennt durch Doppelpunkte oder Bindestriche. <br>
00:1A:2B:3C:4D:5E oder 00-1A-2B-3C-4D-5E.
- Einzigartig: Keine zwei Geräte haben die gleiche MAC-Adresse, selbst wenn sie vom gleichen Hersteller stammen.
- **Merksatz**: Die MAC-Adresse ist wie der Fingerabdruck (Bei jedem menschen einzigartig) eines Geräts im Netzwerk, während die IP-Adresse wie die Postadresse ist, die sich manchmal ändern kann.
___
### Subnetzmaske: 
- Eine Subnetzmaske teilt die IP-Adresse in zwei Teile:
- **Netzwerkanteil**: Der Teil, der alle Geräte im gleichen Netzwerk identifiziert.
- **Hostanteil**: Der Teil, der jedes einzelne Gerät innerhalb dieses Netzwerks unterscheidet.
- Die Subnetzmaske ist wie ein Netzwerkplan, der entscheidet, wie groß ein Netzwerk ist und wer dazugehört
- Sie arbeitet immer mit der IP-Adresse zusammen, um zu bestimmen, wer im gleichen Netzwerk "wohnt"
___
### DNS
- Das **Domain Name System (DNS)** ist wie das Telefonbuch des Internets. Es hilft deinem Computer, die richtige Adresse (IP-Adresse) zu finden, wenn du eine Website aufrufen möchtest.

1. **Deine Anfrage**: Du gibst in deinem Browser "www.google.com" ein.
2. **DNS-Suche**: Dein Computer fragt das DNS: "Welche IP-Adresse gehört zu www.google.com?"
3. **Antwort des DNS**: Das DNS sagt deinem Computer z. B.: "Die IP-Adresse ist 142.250.185.68".
4. **Verbindung zur Website**: Dein Computer nutzt die IP-Adresse, um die Verbindung zum Google-Server herzustellen und die Website zu laden.
___
### NAT
- **Network Address Translation (NAT)** ist wie ein Übersetzer für IP-Adressen in einem Netzwerk. Es wird verwendet, um Geräte in einem privaten Netzwerk mit dem Internet zu verbinden.
- **Nach draußen telefonieren (vom privaten Netzwerk ins Internet):**

- Du (z. B. dein Computer) willst eine Website besuchen.
Dein Router (mit NAT-Funktion) merkt sich, welches interne Gerät (z. B. dein Computer mit IP 192.168.1.10) die Anfrage gestellt hat.
- Der Router ersetzt deine private IP-Adresse mit seiner öffentlichen IP-Adresse (z. B. 203.0.113.1) und schickt die Anfrage ins Internet.
- **Antwort zurück ins Büro (vom Internet ins private Netzwerk):**

- Der Server im Internet (z. B. die Website) antwortet an die öffentliche IP-Adresse des Routers.
- Der Router schaut in seine "Liste" und weiß: "Diese Antwort ist für den Computer 192.168.1.10".
- Er schickt die Antwort an dein Gerät im privaten Netzwerk.
___
## Protokolle
### ARP (Address Resolution Protocol): 
- Ein Protokoll, dass die IP Addresse eines im Netzwerk verbundenem Gerät sucht und die dazugehörige MAC-Addresse als Antwort zurück schickt
___
### IP (Internet Protocol): 
- Das Internet Protocol ist wie die Sprache, die Computer und Geräte im Internet verwenden, um miteinander zu kommunizieren. Es ist dafür verantwortlich, dass Daten, wie zum Beispiel eine Nachricht, ein Video oder eine Datei, von einem Gerät zum anderen geschickt werden können
___
### ICMP (Internet Control Message Protocol)
- Das ICMP ist ein Protokoll der Vermittlungsschicht (Network Layer), das für Fehlerbehandlung, Diagnose und Kontrollmeldungen zwischen Netzwerkgeräten verwendet wird. Es hilft bei der Identifizierung von Netzwerkverbindungsproblemen und bei der Verwaltung des Datenpaketflusses. Es werden keine Daten übertragen.
___
## Sub-Netzwerke
- Ein Subnetz ist ein kleinerer Teil eines Netzwerks. Es hilft, ein großes Netzwerk (z. B. das Internet oder ein Firmennetzwerk) in kleinere, handlichere Teile zu unterteilen
___
### Private Sub-Netzwerke:
- Ein privates Subnetz enthält Geräte, die nicht direkt aus dem Internet erreichbar sind. Sie verwenden private IP-Adressen, die nur innerhalb eines lokalen Netzwerks funktionieren.

- **Merkmale:**

- **Private IP-Bereiche:**<br>
10.0.0.0 – 10.255.255.255<br>
172.16.0.0 – 172.31.255.255<br>
192.168.0.0 – 192.168.255.255<br>
- **Sicher vor direktem Zugriff:**<br> Geräte in einem privaten Subnetz sind durch NAT und/oder Firewalls vom öffentlichen Internet abgeschirmt.
- **Beispiele für Geräte:**<br>
Computer in einem Heimnetzwerk.
Datenbanken oder Anwendungsserver in einer Cloud-Umgebung.
- **Nutzung:**<br> Für interne Kommunikation, die nicht direkt von außen zugänglich sein soll. 
___
### Öffentliche Sub-Netzwerke:
- Ein öffentliches Subnetz enthält Geräte, die direkt aus dem Internet erreichbar sind. Sie verwenden öffentliche IP-Adressen, die weltweit eindeutig sind.

- **Merkmale:**
- **Öffentliche IP-Bereiche:**<br> Werden von einer zentralen Organisation (IANA) zugewiesen und dürfen direkt mit dem Internet kommunizieren.
- **Erreichbarkeit:**<br> Geräte in einem öffentlichen Subnetz können direkt aus dem Internet angesprochen werden.
Beispiele für Geräte:
Webserver (z. B. eine Website, die jeder erreichen soll).
- **Nutzung:**<br> Für Dienste, die öffentlich verfügbar sein müssen.
___
## Ports
- Ein Port ist wie eine Tür oder ein Eingangspunkt für die Kommunikation zwischen verschiedenen Geräten oder Programmen in einem Netzwerk. Jedes Gerät (z. B. dein Computer, Server) hat eine IP-Adresse, und Ports helfen dabei, den Datenverkehr zu den richtigen Programmen oder Diensten auf diesem Gerät zu leiten.
- Ein Port ist also ein nummerierter Eingang, der bestimmt, welche Art von Kommunikation (oder Dienst) ein Datenpaket anspricht. Ohne Ports wüsste dein Computer nicht, welches Programm die ankommenden Daten verarbeiten soll.
___
### Hard-/Software Ports:
- **Hardware-Ports:** Physische Anschlüsse an einem Gerät (z. B. USB- oder HDMI-Ports).
- **Software-Ports:** Rein virtuell, sie existieren innerhalb der Software und werden verwendet, um Daten in einem Netzwerk oder auf einem Gerät weiterzuleiten.

___
### Software Ports:
1. **Bedeutung von Ports in der Software:**
- Ports sind keine physischen Komponenten, sondern rein virtuelle, in der Software definierte Ein- und Ausgänge.
- Sie helfen dabei, den Netzwerkverkehr an die richtige Anwendung oder den richtigen Dienst weiterzuleiten.
2. **Verbindung zu einer IP-Adresse:**
- Jeder Software-Port ist mit einer IP-Adresse verbunden.
- Gemeinsam (IP-Adresse + Portnummer) bilden sie einen sogenannten Socket. Ein Socket ist eine eindeutige Adresse für eine Netzwerkverbindung.
3. **Kommunikation über Ports:**
- Wenn ein Programm Daten senden oder empfangen möchte, "hört" es auf einem bestimmten Port.
- Andere Geräte können Daten an diesen Port schicken, und die Software verarbeitet die eingehenden Informationen.
___