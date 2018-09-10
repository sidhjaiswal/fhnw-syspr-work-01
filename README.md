# System-Programmierung
## Hands-on zu Lektion 1
Für Slides und Code Beispiele, siehe [Lektion 1](../../../fhnw-syspr/blob/master/01/README.md)

> *Achtung: Arbeiten Sie nicht direkt auf diesem Repository.*

### a) int Wertebereich, 20'
* Hardware bzw. Compiler-abhängige Konstanten:<pre>
    #include <limits.h></pre>
* Schreiben Sie ein Programm *my_range.c*, das für die Typen char, int, long, short Wertebereiche so ausgibt:<pre>
    type: TYPE_SIZE byte, TYPE_MIN .. TYPE_MAX</pre>
* Erweitern Sie das Programm für unsigned Typen.
* Tipp: $ gcc FILE.c -M zeigt include Pfade an.

### b) Argumente lesen, 20'
* Command-Line Argumente als Parameter von main:<pre>
    int main(int argc, char *argv[]);</pre>
* Schreiben Sie ein Programm *my_args.c*, das alle Command-Line Argumente mit Index ausgibt:<pre>
    $ ./my_args hoi => 0: ./my_args, 1: hoi</pre>
* Erweitern Sie das Programm, dass es einen Fehler ausgibt, falls ein Argument nicht aus [a-z]* besteht.

### c) Bäume, 20'
* Erstellen Sie eine Datei *my_tree.c* mit einem Struct Typ Tree mit Zeigern auf left, right vom selben Typ.
* Modellieren Sie die [Fussball WM](https://www.fifa.com/worldcup/matches/#knockoutphase) mit dem Tree Typ.
* Erweitern Sie den Tree Typ für Bäume mit variabler Anzahl Ästen, wie [Darwin's Tree of Life](https://en.wikipedia.org/wiki/%20Tree_of_life_(biology)#/media/File:On_the_Origin_of_Species_diagram.PNG).

### d) BLE Pakete, 30'
* Erstellen Sie ein C Struct Typ für BLE Pakete gemäss: https://devzone.nordicsemi.com/f/nordic-q-a/12211/ble-packet-structure in einer neuen Datei *my_ble.c*
* Zudem eine C Union, um auf Heart Rate Messwerte zuzugreifen, gemäss: https://www.bluetooth.com/
specifications/gatt/viewer?attributeXmlFile=org.bluetooth.characteristic.heart_rate_measurement.xml

### Abgabe (optional)
* Lokale Änderungen [committen und pushen](#git).
* GitHub [Issue erstellen](../../issues/new) mit "Bitte um Review, @tamberg".
* Offene Fragen ausformulieren, was geht nicht, was haben Sie versucht.
* GitHub mailt mir (@tamberg) automatisch, ich versuche in weniger als 24h zu antworten :)

## Tools
### Git
Auf Ihrem Computer
* Zu Beginn jeder Lektion wird der Hands-on Repository Link freigeschaltet
* Nachdem Sie das "Assessment" annehmen, bekommen Sie per Email ein Repository
* Die REPO_URL enthält Ihren GitHub Account USER_NAME und Ihre Klasse 3ia oder 3ib, z.B.<br/>
            https://github.com/fhnw-syspr-3ia/fhnw-syspr-work-01-tamberg

Auf dem Raspberry Pi
* Repository klonen<pre>
    $ cd ~
    $ git clone REPO_URL</pre>
* Neue Datei kreieren<pre>
    $ git add FILE</pre>
* Änderungen committen<pre>
    $ git commit FILE -m "Fixed all bugs"</pre>
* Änderungen hochladen<pre>
    $ git push</pre>

### Nano
Auf dem Raspberry Pi
* Neue oder bestehende Datei öffnen mit $ nano FILE
* Editieren (Achtung, nano hat kein Undo)
* Speichern mit `CRTL-X` `Y` `RETURN`

### SSH
Auf Ihrem Computer
* Terminal öffnen (Mac) oder `WINDOWS` `R` cmd `RETURN` (Windows)
* SSH Session starten mit<pre>
    $ ssh pi@raspberrypi.local</pre>

## Support
- [FHNW Syspr Slack](https://fhnw-syspr.slack.com/)
