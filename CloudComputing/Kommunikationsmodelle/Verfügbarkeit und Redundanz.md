---
tags:
- wichtig
---
>availability - can i use it now?
>reliability - can i use it?

## failure modes: 
- request lost 
- server crash before execution,
- server crash during execution
- reply lost 
- client crashes before receiving reply

## failure handling: 
- retransmit 
- re-execute 
- restart client / server
- keep history
- ignore

## Terms
### AFR - Annualized Failure Rate:
- estimated probability that a device or component will fail during a full year of use
- AFR = 1/MTTF

### MTTF: Mean-Time-To-Failure
- MTTF = 1 / AFR (in years) 
	- 1 year = 365.25
	- 1 year in hours = 365.25 24 = 8766

### MTBF: Mean Time Between Failures
### MTTR: Mean-Time-To-Repair

### Availability: 
A = Uptime / (Uptime + Downtime)
A = MTTF / (MTTF + MTTR)

### Multi-Device:
- AFR(system) = ∑(AFR component)
- Availability(system) = ∏(Availability of component)
- Availability(redundant system) = 1 - ∏(Availability of component)

## Redundanz
- physical: 
	- active redundancy (each component works as state machine, mutual monitoring)
	- passive redundancy (standby)
- Information / Data
- temporary

---
[[Kommunikationsmodelle]]

