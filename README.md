# Übung 15 - Arrays

# 1. Aufgabe

Folgendes Klassendiagramm soll umgesetzt werden:

<p align="center">
  <img src="/assets/images/UML1.png" alt="Bildbeschreibung" />
</p>

**Folgende Bedingungen gelten für die Klasse `ZahlenVerwaltung`:**
- Im Konstruktor wird der Speicherplatz für `anzahl` Elemente im Array `ar` angefordert.
- `fuellen()`: Befüllt das Array mit Zufallszahlen im Bereich von `-100.0` bis `100.0`. 
- `eingeben()`: Befüllt das Array mit Zahlen, die vom Benutzer eingegeben werden. Achten Sie darauf, dass nicht zu viele Zahlen eingegeben werden. Sollte eine ungültige Zahl eingegeben werden, wird die Eingabe beendet und die verbleibenden Stellen sollen mit Zufallszahlen befüllt werden.
- `ausgeben()`: Gibt alle Werte des Arrays aus. Nach jeder fünften Zahl soll ein Zeilenumbruch erfolgen. Achten Sie darauf, dass die Kommas untereinanderstehen.
- `double mul()`: Multipliziert die Zahlen im Array und gibt das Ergebnis zurück.
- `double durch()`: Ermittelt den Durchschnitt aller Zahlen im Array und gibt das Ergebnis zurück.
- `double min()`: Ermittelt die kleinste Zahl im Array und gibt sie als Ergebnis zurück.
- `double max2()`: Ermittelt die zweitgrößte Zahl im Array und gibt sie als Ergebnis zurück.
- `sort()`: Sortiert das Array nach folgenden Algorithmus:
    - Durchlaufen Sie das Array von `0` bis `anzahl - 1` – falls Sie während des Durchlaufs feststellen, dass ein Element größer ist als das nachfolgende Element, so tauschen Sie diese.
    - Nach diesem Durchlauf steht an letzter Stelle das größte Element.
    - Durchlaufen Sie nun das Array von `0` bis `anzahl - 2` – falls Sie während des Durchlaufs feststellen, dass ein Element größer ist als das nachfolgende Element, so tauschen Sie diese.
    - Nach diesem Durchlauf steht an der Stelle `anzahl - 2` das zweitgrößte Element.
    - Wiederholen Sie dieses Vorgehen, bis nur noch ein Element zu durchlaufen ist.
    - Überlegen Sie sich, wie man Elemente innerhalb eines Arrays tauschen kann und implementieren Sie eine `private` Methode dafür, welche Sie immer wieder aufrufen.

Um Ihr Programm zu testen, erstellen Sie eine `Main`-Klasse, welche die `main`-Methode beinhaltet:
- `main(String[] args)`: Testen Sie Ihr Programm.

## 2. Aufgabe

Folgendes Klassendiagramm soll umgesetzt werden:

<p align="center">
  <img src="/assets/images/UML2.png" alt="Bildbeschreibung" />
</p>

**Folgende Bedingungen gelten für die Klasse `StringArray`:**
- `StringArray(String[] a)`:  Konstruktor initialisiert das Array mit dem Array `a`.
- `print()`: Gibt das Array aus (Index und Wert). 
- `umdrehen()`: Dreht das Array um, d.h. `a[0]` tauscht mit `a[length - 1]` usw.
- `rechtsSchieben()`: Alle Elemente werden um eine Stelle nach rechts verschoben. Das letzte Element kommt wieder an die Position mit dem Index `0`.
- `linksSchieben(int s)`: Alle Elemente werden um `s` Stellen nach links verschoben.
- `boolean suchen(String s)`: Sucht nach `s` im Array. Wird das Element gefunden wird `true` zurückgegeben. Sonst `false`.
- `String zufall(int l)`: Erzeugt einen zufälligen String von Großbuchstaben der Länge `l`. Ein zufälliges Zeichen kann folgendermaßen erzeugt werden:
<p align="center">
  <img src="/assets/images/COD1.png" alt="Bildbeschreibung" />
</p>

Um Ihr Programm zu testen, erstellen Sie eine `Main`-Klasse, welche die `main`-Methode beinhaltet:
- `main(String[] args)`: Testen Sie Ihr Programm.


## 3. Aufgabe

Bauen Sie Aufgabe 3 aus Übung 13 um. Die `Baum`-Klasse dürfen Sie so übernehmen, jedoch 
soll das `alter` nun `int` als Datentyp haben. Anstatt der Klasse `MiniWald` schreiben Sie nun 
eine Klasse `Wald`. Das Attribut `name` bleibt bestehen, jedoch gibt es jetzt anstatt drei Bäume 
ein Array von Bäumen. Der Wald fasst maximal `100` Bäume. Die Methoden bleiben gleich, 
jedoch gibt es eine neue Methode `double wert(double preis)`. Diese Methode soll den 
Wert des Waldes zurückgeben. Der Parameter beschreibt den Preis pro Kubikmeter. Bauen Sie 
beide Klassen so um, dass diese mit dem Array funktionieren. 

Um Ihr Programm zu testen, erstellen Sie eine `Main`-Klasse, welche die `main`-Methode beinhaltet:
- `main(String[] args)`: Testen Sie Ihr Programm.
