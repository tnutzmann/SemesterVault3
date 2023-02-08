---
tags:

---

## Events
- Ereignisse die das System mitteilt auf dem ein Programm läuft
- Bei [[JavaScript]] in Webpages sind das z.B. Nutzeraktionen
	- Mausaktionen
	- Keyboardaktionen
	- Änderungen des Fensters
	- Download einer Ressource ist abgeschlossen
	- Fehler, uvm.
## Eventhandler/-listener
- Funktionen die beim Eintreten eines Events aufgerufen werden
- Werden auf ein Element registriet
	- z.B. Buttons
- Zwei mögliche Arten
	- **onevent property** (onclick)
	- **addEventListener()
- Beide erhalten bei Ereignis ein *Event* Objekt
- **addEventListener** kann mehrere Funktionen registrieren

#### DOM Eventlistener
- **addEventListener** hat zwei erforderliche Parameter
	- Eventtype
	- Listenerfunktion
- kann auf jedem Object aufgerufen werden, das Events emittiert
```JS
function myFunction() {
	document.querySelectorAll("li").forEach((li,i) => {
		let color = (i % 2 == 1 && i < 9) ? "PaleGreen" : "#D0D0D0";
		li.addEventListener("mouseover", () => li.style.background = color);
		li.addEventListener("mouseout", () => li.style.background = "E0E0E0");
	});
}
```

---
[[JavaScript]]