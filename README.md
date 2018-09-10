# System-Programmierung
## Hands-on zu Lektion 1
Für Slides und Code Beispiele, siehe [Lektion 1](../../../fhnw-syspr/blob/master/01/README.md)

### Hands-on, 20': int Wertebereich
* Hardware bzw. Compiler-abhängige Konstanten:
    #include <limits.h>
* Schreiben Sie ein Programm my_range.c, das für die Typen char, int, long, short Wertebereiche so ausgibt:
    type: TYPE_SIZE byte, TYPE_MIN .. TYPE_MAX
* Erweitern Sie das Programm für unsigned Typen.
* (Tipp: $ gcc FILE.c -M zeigt include Pfade an.)

## Tools
### Git
Auf Ihrem Computer
* Zu Beginn jeder Lektion wird ein Hands-on Repository Link bekannt gegeben
* Nachdem Sie das "Assessment" annehmen, bekommen Sie per Email ein Repository
* Die REPO_URL enthält Ihren GitHub Account USER_NAME und Ihre Klasse 3ia oder 3ib, z.B.<br/>
            https://github.com/fhnw-syspr-3ia/fhnw-syspr-work-01-tamberg

Auf dem Raspberry Pi
* $ cd ~
* $ git clone REPO_URL
* $ git add FILE
* $ git commit FILE -m "Fixed all bugs"
* $ git push

### Nano
Auf dem Raspberry Pi
* Neue oder bestehende Datei öffnen mit $ nano FILE
* Editieren
* Speichern mit `CRTL-X` `Y` `RETURN`

### SSH
Auf Ihrem Computer
* Terminal öffnen (Mac) oder `WINDOWS` `R` cmd `RETURN` (Windows)
* $ ssh pi@raspberrypi.local

## Support
- [FHNW Syspr Slack](https://fhnw-syspr.slack.com/)
