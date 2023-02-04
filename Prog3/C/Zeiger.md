---
alias: pointer
---

## Allgemein
- ermöglichen direkten zugriff auf den Speicher
	- Laufzeit und Speicheroptimierung
	- Achtung: Gefahr kritischer Sicherheitslücken
- Manuelle [[Speicherverwaltung]] wird in höheren Sprachen durch Compiler und Garbage-Collection ersetzt
 ![[Pasted image 20230201195212.png]]

## Pointer
- zeigen auf eine direkte Speicheradresse
	- der *wert* eines Pointer ist die Speicheradresse
	- dieser *wert* wird mit **&** zurückgegeben
```C
int main() {
	int* pvar = NULL;
	int var = 42;
	pvar = &var;
	// pvar enthält nun die adresse bon var
}
```

---
[[C]]