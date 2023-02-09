---
tags:

---

- definiert Strukturen mit mehreren Membervariablen
	- ähnlich zu Objekten in JAVA nur ohne Methoden, Vererbung usw.
```C
typedef struct Exam {
	int id;
	char name[256];
	char topic[256];
	float grade;
} Exam;

Exam prog3;
prog3.id = 4;
prog3.name = "Programmierung 3
// usw...
```
- im Beispiel mit  [[Typedef]] verbunden
---
[[C]]