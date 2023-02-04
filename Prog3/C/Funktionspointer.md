---
tags:

---

- Sind [[Zeiger]] welche auf [[Funktionen]] zeigen
	- Funktionen sind im Speicher eine Abfolge von Instruktionen
	- Funktionspointer muss gleiche Signatur haben wie die Funktion
- Aufruf des Funktionspointers mit entsprechenden Parametern anstatt der eigentlichen Funktion
- ermöglicht Dynamische Verwendung von Unterschiedlichen Funktionsimplementierungen
```C
#include <stdio.h>

int add(int a, int b) {
	return a+b;
}

int main() {
	int (*funcPtr)(int, int);
	funcPtr = add;
	int result = funcPtr(5, 10);
	printf("%i", result);
	return 0;
}
```
---
[[C]]