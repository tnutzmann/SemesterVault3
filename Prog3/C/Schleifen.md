---
tags:

---
## for loop
- Wiederholt die Ausführung eines Blockes i-mal
- Definition von i im Schleifenkopf
- Wiederholung kann mit Sprungmarken *(continue)* beeinflusst werden
```C
#include <stdio.h>

int main(){
	for(int i = 0; i < 5; i++) {
		if(i==2) continue;
		print("Hallo Welt %d\n", i);
	}
	return 0;
}
```
Ausgabe:
```
Hallo Welt 0
Hallo Welt 1
Hallo Welt 3
Hallo Welt 4
```


## while loop und do-while loop
- ähnlich der for-schleife
- Wenn Anzahl der Iterationen nit a priori bekannt
- Schleifenabbruchbedingung als boolean
- While evaluiert vor Ausführung des Blocks
- Do-While evaluiert nach Ausführung des Blocks
```C
#include <stdio.h>

int main(void) {
	int n;
	do {
		printf("Bitte eine gerade Zahl eingeben: ");
		scanf("&i", &n);
	} while (n%2 != 0):
	
	while(n%2 == 0) {
		printf("Die Zahl %d ist durch Zwei teilbar.\n", n);
		n /= 2;
	}
	printf("Die Zahl %d ist nicht merh durch zwei teilbar!", n);
	return 0;
}
```
Ausgabe:
```
Bitte eine gerade Zahl eingeben: 123
Bitte eine gerade Zahl eingeben: 1
Bitte eine gerade Zahl eingeben: 2021
Bitte eine gerade Zahl eingeben: 2024
Die Zahl 2024 ist durch Zwei teilbar.
Die Zahl 1012 ist durch Zwei teilbar.
Die Zahl 506 ist durch Zwei teilbar.
Die Zahl 253 ist nicht mehr durch Zwei teilbar.
```

---
[[C]]