---
tags:
- middleware
- protokoll
---
![[Pasted image 20230131085934.png]]
- No architectural support for remote procedure calls
- Simulate it with local procedure calls
	-	Simulation makes RPC a language-level construct, not aoperating system construct
	-	Create stub functions to make it appear to the user that the call is local
	-	[[Stub]] function contains the function’s interface

## Pros
- Procedure call Interface
- Writing applications is simplified
	- RPC hides all network-code behind stub functions
	- Application programmers don't have to worry about details
		- Socket, Port, Byte-Order
- RPC -> Presentation-Layer (OSI-ISO)

## Problems 
#### 1.	DATA REPRENSENTATION
- No incompatibility problems on local system
- But remote machine may have:
	- Different byte ordering
	- Different sizes of integers and other types
	- Different floating point representations
	- Different character sets	
- **SOLVED BY**:
	- Need standard encoding to enable communication between heterogeneous systems
- Implicit typing
	- only values are transmitted, not data types or parameter info
	- e.g., Sun XDR
- Explicit typing
	- Type is transmitted with each value
	- e.g., ISO’s ASN.1, XML
#### 2.	BINDING SERVER TO CLIENT
- Need to locate host and correct server process
- Alternative 1:
	- Maintain centralized DB that can locate a host that provides
	- a particular service (Birrell & Nelson’s 1984 proposal)
- Alternative 2:
	- A server on each host maintains a DB of locally provided services
#### 3. ERROR HANDLING
- Local procedure calls do not fail
	- If they core dump, entire process dies
	- Local procedure call Semantics: exactly once
- More fault opportunities for RPC
- Transparency breaks à Applications should be prepared to deal with RPC failures
- A remote procedure call may be called:
	- 0 times: server crashed or server process died before executing server code
	- 1 time: everything worked well
	- 1 or more: excess latency or lost reply from server and client retransmission
- Most RPC systems will offer either:
	- at least once semantics
	- or at most once semantics
#### 4. Performance
#### 5. Security
#### 6. Language Support
- Most programming languages (C, C++, …) have no concept for remote procedure calls
- Language compilers will not generate client and server stubs
- **Solved By**:
	- Use a separate compiler to generate stubs (pre-compiler)

---
[[RPC & RMI]]