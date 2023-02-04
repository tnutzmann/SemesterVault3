## If/else/else if
- einfache Verzweigung
- *If* Prüft auf einen Wahrheitswert
	- in C: (!=0)
- *Else* beschreibt alternativ code
	- Ausführung wenn: *false* (==0)
- *Else if* verzweigt weiter
```C
void checkOneOrZero(int n) {
	if(n == 0) {
		puts("Is zero!");
	} else if (n == 1) {
		puts("Is one!");
	} else {
		puts("Not One or Zero!");
	}
}
```

## switch/case
- *switch* prüft Inhalt eines Ausdrucks auf verschiedene Werte
- *Case* prüft gegen Konstanten
- *Break* beendet den Block
- *Default* wird aufgerufen wenn kein *case* zutreffend war
```C
void checkOneOrZero(int n) {
	switch(n) {
		case 0:
			puts("Is zero!");
			break;
		case 1:
			puts("Is one!");
			break;
		default:
			puts("Not One or Zero!");
			break;
	}
}
```

---
[[C]]