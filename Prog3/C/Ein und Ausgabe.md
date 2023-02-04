---
tags:

---

![[Pasted image 20230202130721.png]]

## Allgemein
Interaktion mit einem Programm
- Eingaben
	- Parameter
- Ausgaben - geben Ereignisse zurück
	- Konsole
	- Grafik
	- Sound
	- Datenbanken
	- Speicher
	- Logging
	- Netzwerk
	- Peripheriegräte

## Bezug zur [[Turingmaschine]]
- Anfangszustand *q0* einer Turing Maschine wird über **Eingabe** bereitgestellt
- Menge der Endzustände *F* wird über **Ausgaben** des Rechners präsentiert  
- **Turing Maschine sieht keine Interaktion während der Programmausführung vor**

## Funktionen
#### printf()
- Formatierte Ausgabe
#### fgets()
- Zeilenweises einlesen von Konsole
- Einlesen aus Dateien oder anderem *Inputstream*
#### scanf()
- einlesen nur von *stdin*
- teilt Eingabe entsprechend der Formatspezifier
## Ein-/Ausgabe über Argumente
- Parameterübergabe bei Programmstart
- **int argc** enthält die Anzahl an Argumente
- **array agrv[]** enthält Argumente
	- *argv[0]* enthält den Pfad der **exe**cutable
- **$LASTEXITCODE** gibt den Letzten return

---
[[C]]