# System-Programmierung
## Hands-on zu Lektion 1
Für Slides und Code Beispiele, siehe [Lektion 1](../../../fhnw-syspr/blob/master/01/README.md)

> *Achtung: Arbeiten Sie nicht direkt auf diesem Repository.*<br/>
> *[Prüfen Sie die vorhandenen Forks, um das Repository für Ihre Klasse zu finden.](../../network/members)*

### a) int Wertebereich, 15'
* Schreiben Sie ein Programm *my_range.c*, das den Wertebereich des Typs *int* ausgibt, z.B. mittels *while*:<pre>
    $ ./my_range
    INT_MIN, INT_MAX</pre>
* Nutzen Sie aus, dass *INT_MAX + 1 = INT_MIN* gilt.
* Die Ausgabe eines *int* Werts *i* ist möglich mit *%d*<pre>
    printf("%d\n", i); // \n = newline character</pre>

### b) Argumente lesen, 15'
* Command-Line Argumente als Parameter von main:<pre>
    int main(int argc, char *argv[]);</pre>
* Schreiben Sie ein Programm *my_args.c*, das alle Command-Line Argumente mit Index ausgibt:<pre>
    $ ./my_args hoi => 0: ./my_args, 1: hoi</pre>
* Erweitern Sie das Programm, dass es einen Fehler ausgibt, falls ein Argument nicht aus [a-z]* besteht.

### c) Bäume, 15'
* Erstellen Sie eine Datei *my_tree.c* mit einem Struct Typ Tree mit Zeigern auf *left*, *right* vom selben Typ, und einem String *label* von maximal 32 Byte Länge.
* Instanzieren Sie einen binären Baum mit 3 Blättern, verwenden Sie dazu die Funktionen malloc und free.
* Erweitern Sie den Node Typ für Bäume mit variabler Anzahl (N > 2) Ästen, wie [Darwin's Tree of Life](https://en.wikipedia.org/wiki/%20Tree_of_life_(biology)#/media/File:On_the_Origin_of_Species_diagram.PNG).

### d) BLE Pakete, 15'
* Erstellen Sie ein C Struct Typ für BLE Pakete gemäss: https://devzone.nordicsemi.com/f/nordic-q-a/12211/ble-packet-structure in einer neuen Datei *my_ble.c*

### e) Makefile, 15'
* Erstellen Sie ein *makefile* für Ihren Hands-on Code.
* Verwenden Sie die Compiler Flags aus dem Script.
* Korrigieren Sie allfällige neue Kompilationsfehler.
* Führen Sie *make clean* aus, vor dem *git commit*.
