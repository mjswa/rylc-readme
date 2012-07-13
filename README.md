# README für alle RYLC-Repositories #

Dieses README gibt einen Überblick über alle Repositories mit Beispielcode zum Buch [Mobile Web-Apps mit JavaScript](opitz-consulting.com/go_javascriptbuch) und dokumentiert die allgemeinen Voraussetzungen zum Ausführen der Beispiele.

## Überblick ##

*   [rylc-backend](https://github.com/mjswa/rylc-backend): Enthält die Backend-Komponente der Beispielapplikation und wird ab Kapitel 7 Backendkommunikation verwendet. Damit die Backend-Komponente von den anderen Projekten bei Bedarf verwendet werden kann, muss man in diesem Projekt in das Unterverzeichnis `rylc-backend-jar` wechseln und das Projekt mit Maven (siehe Voraussetzungen) mit dem Kommandozeilen-Befehl `mvn clean install -Pproduction` bauen.
*   [rylc-tdd](https://github.com/mjswa/rylc-tdd): Enthält den Beispielcode zum Kapitel 4 Testen.
*   [rylc-ui](https://github.com/mjswa/rylc-ui): Enthält den Beispielcode zum Kapitel 5 Oberflächenkomponenten
*   [rylc-binding](https://github.com/mjswa/rylc-binding): Enthält den Beispielcode zum Kapitel 6 Data Binding
    *   Branch [plain](https://github.com/mjswa/rylc-binding/tree/plain): Enthält den Code zu Abschnitt 6.1
    *   Branch [minimal](https://github.com/mjswa/rylc-binding/tree/minimal): Enthält den Code zu den Abschnitt 6.2 und 6.3
    *   Branch [master](https://github.com/mjswa/rylc-binding): Enthält den Code zum Abschnitt 6.4
*   [rylc-services](https://github.com/mjswa/rylc-services): Enthält den Code zum Kapitel 7 Backendkommunikation    
    *   Branch [inmemory](https://github.com/mjswa/rylc-services/tree/inmemory): Enthält den Code zu den Abschnitten 7.1 und 7.2
    *   Branch [master](https://github.com/mjswa/rylc-services): Enthält den Code zu den Abschnitten 7.3 und 7.4
*    [rycl-html5](https://github.com/mjswa/rylc-html5): Enthält den Code zu den Kapiteln 8 und 9
     *   Branch [baseline](https://github.com/mjswa/rylc-html5/tree/baseline): Enthält den Code zum Kapitel 8 Die fertige Web-App
     *   Branch [master](https://github.com/mjswa/rylc-html5): Enthält den Code zum Kapitel 9 Modularisierung und Build
*    [rylc-html5-phonegap](https://github.com/mjswa/rylc-html5-phonegap) enthält den Code zu Kapitel 10, Abschnitte 10.1, 10.2, 10.5 und folgende.
*    [rylc-android-phonegap](https://github.com/mjswa/rylc-android-phonegap) enthält den Code zu Kapitel 10, Abschnitte 10.3 bis 10.5.

## Voraussetzungen ##

*   [Java Development Kit 1.6 oder neuer](http://www.oracle.com/technetwork/java/javase/downloads/index.html).
*   [Apache Maven 3.0.4 oder neuer](http://maven.apache.org/).
*   [Google Chrome](http://www.google.com/chrome)
*   Für das Bauen der Projekte mit Maven sollte Google Chrome möglichst von der Kommandozeile aus mit dem Befehl `chrome` gestartet werden können. Unter Linux-Systemen kann dazu beispielsweise ein Alias für das Executable von Chrome erstellt werden. 
    Unter Windows kann das Verzeichnis, das `chrome.exe` enthält, der Umgebungsvariable PATH hinzugefügt werden.
    Alternativ kann man beim Aufruf von Maven den Kommandozeilenparameter `-Dbrowser=<Pfad zu Chrome>` angeben, für OS X beispielsweise so:
      
    <pre><code>$ mvn clean install -Pintegration -Dbrowser=/Applications/Google\ Chrome.app/Contents/MacOS/Google\ Chrome</code></pre>

    Details zum Bauen der Projekte finden sich im jeweiligen Projekt.      
*   Einzelne Projekte haben gegebenenfalls noch weitere Voraussetzungen. Dies ist in dem jeweiligen Projekt dokumentiert.