
### Der Ablauf enthält hauptsächlich Notizen für mich
#### Also bitte nicht wundern, wenn die einzelnen Punkte wenig Inhalt haben

## 1. Vorbereitung

- Prüfen, ob Python installiert ist
- Python installieren und nochmal prüfen
- Pycharm installieren
- Vorteile von PyCharm
- Gelegenheit es zu installieren


- Allgemein Vor- und Nachteile von Python
  - Einfach, aber langsam


- Python Terminal
  - Rechnen mit Variablen
  - int deklarieren
  - `+ - * / ** //`
  - Klammern
  - float deklarieren
  - Übung 1.1

### Jetzt in PyCharm

- Oberfläche erklären (Ausgabefenster)
- Ein Skript ausführen


- print()
  - Klammern hinter Funktionen
  - Mehrere Argumente
- Strings definieren
- input()
  - input("...")
- Strings definieren
- Übung 1.2

## 2. Variablentypen

- Verschiedene Variablentypen
  - int
  - str
  - float
  - bool
- Typecasting (str in int umwandeln, etc.)
  - type()
- Übung 2.1
- Übung 2.2

## 3. Bedingungen und Verzweigungen

- bool-Variablen/Bedingungen
  - True, False
- Vergleiche
  - ==, !=
  - <, >, <=, >=
  - and, or
  - not
- Übung 3.1


- if-Verzweigung
  - else
  - elif
  - Test, ob Variable einen Wert hat mit bool()
  - pass
  - while-Schleifen
- Übung 3.2

## 4. Listen


- Indexe aufrufen
  - Mehrere Indexe aufrufen
  - Von...bis
  - Schrittweite bei Indexen
- Listen "Addieren"
  - Listen "Multiplizieren"
- del
- Übung 4.1
- .copy()
- Element appendieren
  - Häufiger Fehler: Liste an Liste appendieren
- len()
- sort()
  - sorted()
- in-Operator 
- Übung 4.2 
- Übung 4.3

## 5. Strings

- str()
- Besondere Zeichen  “\n” und “\t”
- "Rechnen" mit Strings
- replace()
- upper(), lower() und capitalize()
- list()
- len()
- split()
- .join()
- in - Operator bei Strings
- f-Strings
- Übungen 5.1 - 5.3


## 6. Schleifen

- while-Schleifen
- break, continue
- for-Schleifen
- range()
- enumerate()
- zip()
- Übung 6.1
- List Comprehension: Einzeilige for-Schleifen zum Erstellen einer Liste
- Unterstrich als Variablenname
- Übungen 6.2

## 7. Dateien

- Was sind Dateiendungen?
- Dateien auslesen
  - with open… as f: …
- Übung 7.1
- Ordner erstellen
- JSON Modul

## 8. Dictionaries

- Elemente anhängen
  - Elemente löschen
- values(), keys() und items()
- in - Operator
- .get()
- .copy()
- Übung 8.1

## 9. Funktionen

- Warum Funktionen? Wann sollte eine Funktion verwendet werden?
- Grundlegende Funktionen
- Argumente
  - Optionale Argumente / Standardwerte
  - Unendlich viele Argumente
- \* und ** vor Listen/dicts
- Veränderbare / Nicht-Veränderbare Datentypen
- Tuples vs lists
- Docstrings und Typehints
  - any
  - “oder”
  - list[]
  - dict[int:int]
- Übung 9.1

### Lokale und Globale Variablen

- isinstance()
- Map-Funktion
- Key beim sortieren
- Übungen 9.2, 9.3
- (Rekursion zum Knobeln) Übung 9.4

## 10. Try-Except

- Warum Try-Except?
- Try-Except
  - Fehler-Art herausfinden
  - Warum nicht um gesamtes Skript Try-Except packen?
- Fehler-Obergruppen
  - https://docs.python.org/3/library/exceptions.html#exception-hierarchy
- Exception in Variablen “catchen” 
- Übung 10.1 
- raise
  - assert (Komma, um Beschreibung anzufügen)
- Übungen 10.2, 10.3

## 11. Klassen und Objektorientierung (OOP)

- Grundlagen (Karton-Analogie)
  - Was bedeutet das self bei jeder Methode?
  - Von “außen” auf Attribute und Methoden zugreifen/erstellen
- `__init__()`
- isInstance()
- Mal wieder veränderbar/nicht-veränderbar
- Übung 11.1
- Vererbung
  - super()
- Übung 11.2, 11.3
- Dunder-Methoden (“Magic”-Methoden)
  - str
  - len
  - add, mul
- Übung 11.4
- `self.__dict__` nutzen, um Instanz zu kopieren
- pickle Modul
- Mehrere Funktions-Rückgaben
- Lambda-Funktionen
- Übungen 11.5, 9.4

# Ende der Grundlagen
### Ab jetzt bist du fortgeschritten. Herzlichen Glückwunsch!

## 12. Benutzeroberflächen mit PySimpleGUI

Wir nutzen FreeSimpleGUI, ist aber identisch zu PySimpleGUI

- Grundlegende Struktur von PySimpleGUI
- Grundlegende Elemente
  - Text
  - Input
  - Button
  - Separators
  - Checkbox
  - Elemente auslesen
  - Keys setzen
- Elemente beschreiben
- enableEvents
- Fenster schließen
- Themes
- Übung 12.1
- Listen-Elemente
- List (ist Schrott)
- Table
  - size
  - col_width
  - headings
  - justification
- Übungen 12.2, 12.3
- TKinter Events
  - https://web.archive.org/web/20201111211515id_/https://effbot.org/tkinterbook/tkinter-events-and-bindings.htm#events
- timeout-event
- .update()
  - color, button_color
- Übung 12.4
- sg-Popups
- Columns
- Frames
- vertical_alignment
- element_justification
- TabGroups
- Übung 12.5

[Weitere Tutorials zur Bibliothek](https://docs.pysimplegui.com/en/latest/cookbook/original/)


Multithreading/Multiprocessing

Mit Abstand das komplizierteste Thema des Kurses, aber trotzdem wichtig für vernünftige Projekte.

Multithreading
Warum Multithreading?
Beispiel an meinem Inventarsystem
Unterschied zwischen Multithreading und Multiprocessing
Numba jit
Zusätzliche Threads starten
daemonic Threads
Informationen vom einen Thread zum nächsten Transportieren
Argumente an den Thread übergeben
Globale Variablen
Übung 13.1
Synchronisation: https://docs.python.org/3/library/threading.html#event-objects
Warum ist Synchronisation nötig?
.join()
Lock
Semaphore
Barrier
Event (Ein-/Ausschalter)
Timer
cancel
Übungen 13.2, 13.3
Threads mit PySimpleGUI
Übung 13.4 (Wird übersprungen)

Multiprocessing
Was ist anders zum Multithreading?
Pools
map
https://docs.python.org/3.11/library/multiprocessing.html#module-multiprocessing.pool
Übung 13.5


Iterators

Wofür Generators?
Aufbau von Iteratoren
iter, next und StopIteration
Erstes Element aus einem Generator bekommen
Einfache Generator mit Funktionen
Wie funktionieren zip und enumerate?
Übung 14.1
Stand 06.08.2024
Iteratoren aus eigener Klasse		(Wird übersprungen)
Generator Comprehension		(Wird übersprungen)

RegEx

Wofür RegEx?
Aufteilung: 1. Einheit nur RegEx, 2. Einheit Kombination mit Python
… Präsentation über RegEx


Numpy und Pyplot 

Liste in Array umwandeln
Einfache Array-Erstellung
zeros, ones, full, empty
_like
arange, linspace
astype
Shape
reshape
flatten
Transponieren
Grundlegendes Indexen
Wiederholung zum normalen Indexen
Teil eines Arrays ersetzen
Gesamtes Array auf eine Zahl setzen
Übung 16.1
Rechnen mit Numpy-Arrays
sin, cos
Grundlegende Plots
plt.plot
plt.scatter
Mehrere Linien in ein Fenster
Stand 03.09.2024
Übung 16.2
Mehrdimensionale Plots
Was sind Skalarfelder?
Was sind Vektorfelder?
meshgrid
pcolor
pcolormesh
colorbar
contour
quiver
streamplot
Übung 16.3
Boolsche Funktionen
Indexen nach booleschen Funktionen
np.where
& und |
Übung 16.4, 16.5
Stand 17.09.2024
Mathematische Funktionen
min, max
mean
sum
log, log10, ln
Achsen bei den Funktionen angeben
Random
plt.hist
bins
Gleichverteilung (random.random)
randint
Normalverteilung (random.normal)
np.clip
random.choice
Übung 16.7 + 16.8 (Ja, vor 16.6)
Datetime
dt.date und dt.datetime
datetime in date umwandeln
.day, .month, .year, etc.
.now()
.replace()
Rechnen mit Daten
- (Minus)
< > (Vergleiche)
Timedelta
Strings in Daten umwandeln und umgekehrt
https://www.geeksforgeeks.org/python-strftime-function/
Übung 16.6
Anhängen
concatinate
Plots verschönern
Subplots
Legend
Title
xLabel, yLabel
xTicks, yTicks


Spezielle Themen

Dataklassen
Decorators
staticmethod
exec
hash
Closures


Hilfreiche Module

Hier gehen wir einige kleinere Module durch, die man immer mal wieder braucht

Fernet
Datetime
strsimpy (String matching)
pyautogui

Pyplot

X. Anderes/Fortgeschrittenes

Themenübergreifende Inhalte, die man erst nach den Grundlagen wirklich verstehen kann

Lambda-Funktionen
filter
keys beim Sortieren
Decorators
Eigene Dateien importieren
Mehrere Rückgabewerte von Funktionen


