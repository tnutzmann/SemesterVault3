---
tags:
- Kommunikation
---

Web-Sockets: Web-Sockets ermöglichen es, eine bidirektionale Kommunikation zwischen einem Client (z.B. einem Webbrowser) und einem Server herzustellen. Dies ermöglicht z.B. die Echtzeitübertragung von Daten zwischen einem Client und einem Server.

- full-duplex communication channel that operates over a single socket
- exposed via a javascript interface in compliant browsers
- UTF-8
- Not a raw TCP socket
- Starts as HTTP, switches to Websocket via "upgrade request"
- Supports >1 connections over 1 TCP socket

---
[[Kommunikationsmodelle]]