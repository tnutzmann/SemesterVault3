---
tags:

---

![[Pasted image 20230202134151.png]]
- Verarbeiten Eingaben (Input) zu Ausgaben (Output)
	- ggf. siehe [[Ein und Ausgabe]]
	- **Output = f(Input)**
- sind wiederverwendbar
- ermöglichen [[Rekursion]]
- Parameter enthalten **Werte**, keine Variablen -> *call-by-value*!
- C erlaubt nur einen Rückgabewert (Output)

## Call-by-Value
der Code:
```c
#include <stdio.h>

void addOne(int n) {
	n++;
	printf("Wert von n innerhalb von addOne(): %d\n", n);
}

int main(void) {
	int x = 1;
	printf("x vor addOne: %d\n", x);
	addOne(x);
	printf("x nach addOne: %d\n", x);
	return 0;
}
```
führt zu der Ausgabe:
```shell
x vor addOne: 1
Wert von n innerhalb von addOne(): 2
x nach addOne: 1
```
>An die Funktion *addOne()* wird nur der Wert von **x** übergeben und nicht seine Referenz. Daher wird der Wert von x zwar in er Funktion *addOne()* um eins erhöht aber ist außerhalb des Funktionsblocks wieder wir vor dem Funktionsaufruf.

---
[[C]]