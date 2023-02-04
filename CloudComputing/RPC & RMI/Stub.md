---
tags:
- protokoll
- middleware
---

>An der Implementierung eines [[RPC|Remote Procedure Calls]] sind auf Sender- und Empfängerseite spezielle Instanzen beteiligt, die als Stubs (dt. „_Stummel“_) bezeichnet werden. Der **Client-Stub** agiert auf der Client-Seite als Stellvertreter der entfernten Server-Prozedur. Der **Server-Stub** ist der serverseitige Stellvertreter des aufrufenden Client-Codes. Die Stubs simulieren operativ eine funktionale lokale Einheit, indem sie das „Entferntsein“ des Codes auf der jeweils anderen Seite kaschieren. Zugleich fungieren sie als Prozedur-Schnittstellen.

---
[[RPC & RMI]]