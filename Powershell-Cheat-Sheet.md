# Powershell-Cheat-Sheet

## Verzeichnis
`cd`: **change directory**: wechselt das Verzeichnis
___
`ls`: **list**: zeigt den Inhalt eines Verzeichnisses/Ordners
___
## Ordner
`mkdir NAME`: **make directory**: erstellt in dem Aktuellen Verzeichnis einen Ordner NAME
___
`rename-Item NAME TEST`: Der Ordner, im aktuell ausgewähltem Verzeichnis, NAME wird in TEST umbenannt
___
`rmdir TEST`: **remove directory**: Der Ordner, im aktuell ausgewähltem Verzeichnis, TEST wird gelöscht
___
## Dateien
`new-Item TEST.txt`: erstellt, im aktuell ausgewähltem Verzeichnis, eine TEST Textdatei
___
`rename-Item TEST.txt HALLO.md`: benennt und ändert die TEST Textdatei in eine HALLO Markdown Datei
___
`add-Content HALLO.md -value "# Hallo Welt!"`: fügt der HALLO.md Datei den Text #Hallo Welt! hinzu, dieses wird in einer neuen Zeile angehängt und der vorherige Inhalt nicht gelöscht!
___
`set-Content HALLO.md -value "# Dies ist ein Test!"`: (falls keine HALLO.md datei in dem Verzeichnis existiert, wird diese erstellt) fügt der HALLO.md Datei den Text # Dies ist ein Test! hinzu, **ACHTUNG:** vorheriger Inhalt wird gelöscht!
___
`remove-Item HALLO.md`: löscht die HALLO.md Datei. **ACHTUNG:** Die Datei wird nicht in den Papierkorb verschoben, sonder direkt gelöscht!
___