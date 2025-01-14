# Netzwerk-Wiki
## Netzwerkarten
- `WAN`: Wide Area Network: Ein zusammenschluss von mehreren einzelnen Netzwerken
___
- `LAN`: Local Area Network: Ein auf ein bestimmten Bereich (z.B. Wohnhaus oder Büro) beschränktes Netzwerk
___
- `PAN`: Personal Area Network: Ein "Persönliche" Netzwerk mit geringer Reichweite, z.B. Kopfhörer mit Smartphone oder Tastatur mit Rechner
___
## Addressen
- `IP-Addresse`: Eine Internet Protocol-Adresse ist eine Art digitale Adresse, die Geräten hilft, miteinander im Internet oder in einem Netzwerk zu kommunizieren. Jedes Gerät, das mit einem Netzwerk verbunden ist, wie ein Computer, ein Smartphone oder ein Drucker, braucht eine IP-Adresse, um Daten senden und empfangen zu können.
___
- `MAC-Addresse`: Eine Media Access Control-Adresse ist eine Art serienmäßige Kennung, die jedem Gerät, das sich mit einem Netzwerk verbinden kann, zugewiesen wird. Sie ist einzigartig und wird von dem Hersteller des Geräts festgelegt.
-Sie besteht aus 6 Paaren im hexadezimalsystem, getrennt durch Doppelpunkte oder Bindestriche. <br>
00:1A:2B:3C:4D:5E oder 00-1A-2B-3C-4D-5E.
- Einzigartig: Keine zwei Geräte haben die gleiche MAC-Adresse, selbst wenn sie vom gleichen Hersteller stammen.
- **Merksatz**: Die MAC-Adresse ist wie der Fingerabdruck (Bei jedem menschen einzigartig) eines Geräts im Netzwerk, während die IP-Adresse wie die Postadresse ist, die sich manchmal ändern kann.
___
- `Subnetzmaske`: Eine Subnetzmaske teilt die IP-Adresse in zwei Teile:
1. **Netzwerkanteil**: Der Teil, der alle Geräte im gleichen Netzwerk identifiziert.
2. **Hostanteil**: Der Teil, der jedes einzelne Gerät innerhalb dieses Netzwerks unterscheidet.
- Die Subnetzmaske ist wie ein Netzwerkplan, der entscheidet, wie groß ein Netzwerk ist und wer dazugehört
- Sie arbeitet immer mit der IP-Adresse zusammen, um zu bestimmen, wer im gleichen Netzwerk "wohnt"
___
## Protokolle
- `ARP`: Address Resolution Protocol: Ein Protokoll, dass die IP Addresse eines im Netzwerk verbundenem Gerät sucht und die dazugehörige MAC-Addresse als Antwort zurück schickt
___
- `IP`: Das Internet Protocol ist wie die Sprache, die Computer und Geräte im Internet verwenden, um miteinander zu kommunizieren. Es ist dafür verantwortlich, dass Daten, wie zum Beispiel eine Nachricht, ein Video oder eine Datei, von einem Gerät zum anderen geschickt werden können
___
- `ICMP`: Internet Control Message Protocol ist ein Protokoll der Vermittlungsschicht (Network Layer), das für Fehlerbehandlung, Diagnose und Kontrollmeldungen zwischen Netzwerkgeräten verwendet wird. Es hilft bei der Identifizierung von Netzwerkverbindungsproblemen und bei der Verwaltung des Datenpaketflusses. Es werden keine Daten übertragen.
___