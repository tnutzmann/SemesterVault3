---
tags:

---

## malloc()
- malloc() allokiert Speicher im Heap
	- gibt einen Pointer auf den neuen Speicher zurück

## free()
- gibt Speicher wieder frei

```C
#include <stdio.h>
#include <stdlib.h>

int main(void) {
	char* s = NULL; // an diesem punkt ist kein Speicher allokiert
	s = malloc(6);

	if (s == NULL) return 1; // fehlererkennung wenn kein Speicher zugewiesen werden konnte
	printf("String eingeben!");
	scanf("%s", s);
	printf("Eingegebener String war: %s\n", s);
	free(s);
	return 0;
}
```

## realloc()
- Nachträgliches ändern der Speichergröße einer Variablen
- Komplexität von O(n)
- ermöglicht Dynamische Arrays

---
[[C]]