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

```

---
[[C]]