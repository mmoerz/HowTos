# SOLID

sind ein Satz von Prinzipien, die zusammen verwendbar sind und sich 
auch reibungslos miteinander kombinieren lassen.

ein oder mehrere Qualitaetsattributen werden addressiert.
schwer auswaehlbar welche 

Roberts Simatin
Barbara Liskov
Bernd Romanier

Prinzip | Kurzbeschreibung
--------| ----------------
Single Responsibility Principle | 
Open-Closed Principle |
Liskov Substitution Principle |
Interface Segregation Principle |
Dependency Inversion Principle |

Dient zur Steigerung der Software Qualitaet.


# SRP - verwendet
Platz 1.
Prinzip *einer* Verantwortung.
D.h. ein System (Methode, Klasse, Komponete, eine Schicht, ein Dienst) 
  uebernimmt immer nur *eine* Aufgabe (*eine* Verantwortung).

- Einfach zu warten
- Einfach zu testen
- Einfach zu verstehen

SRP hilft durch das richtige Aufteilen Software besser analysierbar,
erweiterbar und damit besser austauschbar zu machen.

# OCP
Platz 3.
Offen fuer Erweiterungen - Stellen wo erweiterungen gemacht werden koennen 
sollen bei der Entwicklung schon festgelegt werden
geschlossen fuer Veraenderungen - d.h. sonst keine Veraenderungen

Veraenderungsstellen sollen so entworfen und implementiert werden, dass
dort Weiterentwicklung gemachten werden koennen soll ohne grossartige
Veraenderungen im Source Code zu benoetigen.


# LSP
LSP beschreibt die Verantwortung einer abgeleiteten Klasse oder einer 
Klasse welche eine Schnittstelle implementiert bezueglich ihrer Basisklasse.
Sowohl bei der Ableitung als auch bei der Implementierung der Schnittstelle
muss ein Kontrakt eingehalten werden und dieser sinnvoll implementiert werden.
(= keine abstrakten Funktionen)

stellt sicher, dass hinter einem jeden Kontrakt jede beliebige Implementierung
genutzt werden kann, ohne dass der Aufrufer dies gar nicht erst bemerkt.
Erweiterbarkeit und Austauschbarkeit wird gefoerdert.

# ISP
Platz 4.
ISP regelt granularitiert von Kontrakten (meist Schnittstellen)
  fuer jeden Konsument muss ein eigener Kontrakt erstellt werden
  Um die Auswirkungen der Aenderungen der Schnittstelle gegenueber dem Rest der
  Applikation in Grenzen zu halten.
  wird nicht befolgt, FAT Interfaces negativ fuer Wartbarkeit, Erweiterbarkeit

# DIP - verwendet
Platz 2.
niemals gegen Implementierung sonder nur gegen Schnittstellen implementieren
Sobald man von einer Implementierung abhaengig ist, kann man nicht mehr
erweitern oder austauschen.
DIP sorgt fuer Entkopplung solcher Abhaengigkeiten und dass diese nur 
gegen diese Kontrakte bestehen und die benoetigen Kontrakte per 
Implementierung zur verfuegung gestellt bekommen

DIP  einer App nur Abhaengikeiten gegen Kontrakte und nicht Implementierung

