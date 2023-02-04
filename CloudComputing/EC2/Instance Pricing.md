---
tags:
- AWS-Dienst
- Computing
- VM
- Virtualisierung
- Cost
---
![[Pasted image 20230130171718.png]]
## Family
- F: fast
	- Genomics research, financial analysis, realtime video, processing, big data
- I: IOPS
	- NoSQL DB, DWH
- G: Graphics
	- Video Encoding, 3D, App Streaming
- H: High Disc
	- MR, DFS/HDFS, MR-FS
- T: BrusTable
	- Web Servers, small DB
- D: Data
	- Heavy Data Usage
- R: RAM
	- Memory intensive Apps
- M: Main
	- App Servers
- C: Compute
	- CPU intensive Apps
- P: GPU
	- ML (machine learning), Bitcoin Mining
- X: EXtreme RAM
	- SAP HANA, Apache Spark

## Generation
höhere Zahl <==> neuerer Instanz-Typ

## Size
xlarge > large > medium > small > micro > nano

## Kosten
- größer == teurer
	- mehr RAM mehr teuer
	- mehr CPU mehr teuer
- family abhängig
- Volume kostet unabhängig von der Instanz
- ggf. Lizenzkosten für Betriebsystem

## Commitment

---
[[EC2]]