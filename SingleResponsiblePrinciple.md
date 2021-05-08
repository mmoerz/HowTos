# Single Responsible Principle

ist ein fundamentales Prinzip.
dient zur Wartbarkeit, Wiederverwendbarkeit, Austauschbarkeit, 
Muss den ganzen Tag eingehalten werden.

Anfang der 70er Jahre hat man sich (in der Entwicklung) Gedanken gemacht.

David Parnass
1972 - One criteria to be used in decomposing systems into modules

Dinge so aufzutrennen an den Teilen die unabhaengig von einander zu 
veraendern sein werden.

Ezgard Deistra 

Seperation of Concerns 

Tombli Marko
Page Jones
Aus der Sicht der Kohesion und Kopplung beschrieben.
1979

199x
Robert Simartins
A Class should only have one reason to change

## Responsibility

Zustaendigkeit - was ist das?

## technische Schicht

Responsibility - Aufgabe
Oberflaeche - Logik - Daten
ISO/OSI Schicht Modell

Softwarequalitaet zu steigern
Anwendung in technische Komponenten zerlegen.

## fachliche Schicht
Zustaendigkeit ist eine Aufgabe

Komponenten trennen, die sich getrennt aendern koennen sollen.
Domaenenaufgaben also.

Zustaendigkeit
z.B. Amazon:
- Lagerverwaltung
- Buchhaltung
- shopsystem
- kommissionierung

Aenderung nur an einer Stelle zu machen


SYA - System Architektur
Domaenen angelehnt.

Buchaltung
Logistik
Shop

SWA - Sofware Architektur

- CAI
- Logic - zerlegt sich in Rechnung, Buchhaltung, ...
- Data

- CrossCutting Layer (tauscht mit allen anderen Daten aus)


SWD - Software Design

Namensmuster um Gruppen von zu beschreiben

Rechnungskomponente:

- BillManager
- BillCloner
- BillValidator

## Warum ist das Wichtig?
Weil die Software mehrere Jahrzehnte gepflegt werden koennen soll.
Die Anwendung muss die Komplexitaet sehr leicht beherrschbar machen.


