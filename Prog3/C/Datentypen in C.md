---
tags:

---
> Werte für Windows
## Datentypen
### Character - char
- einzelne Zeichen oder Zahlen
- 1 Byte
### Integer - int
- Natürliche Zahlen
- -2147483648 bis 2147483647
- 4 Byte

#### long & long long
- Größere Integer
- long unter Windows sinnlos
- long long -> 8 Byte

### Float und Double
- Fließkommazahlen -> Gebrochene Zahlen mit Dezimalstellen
- Präzision von 6 bzw 14 Stellen
- float - 4 Byte
- double - 8 Byte

## Modifikatoren
- Signed und unsigned
	- Verwendet für *char* und *int*
	- erstes bit definiert Vorzeichen
- Shot und long
	- Vermindert/erhöht Speicher und damit Wertebereich für *int* und *double*
	- Konkreter Wertebereich abhängig von OS und CPU-Architektur
>**limits.h** beinhaltet die jeweils gültigen Werte

## Casting
>Typumwandlung
```C
int x = 8;
int y = 3;
float z = (float)x/y;
```
**Achtung:** Informationsverlust bei Umwandlung von höherwertigen in niederwertigere Datentypen

## Bezug zur [[Turingmaschine]]
- Eingabealphabet Σ beinhaltet Daten repräsentiert durch Datentypen 
- Bandalphabet Γ ist in einfachster Form binär {0,1} 
- Programmiersprache mappt Σ auf Γ

---
[[C]]