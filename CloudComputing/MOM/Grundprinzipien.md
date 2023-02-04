---
tags:
- queuing
---

## Products:
-   IBM MQS
-   Microsoft Microsoft Message Queuing (MSMQ)
-   Apache ActiveMQ
-   AWS Simple Queue Service (SQS)

## Synchronous communication
- Pros:
	-   Client is informed about message delivery
	-   No buffering necessary
- Cons
	-   Sender and receiver have to run on the same time
	-   Direct connection necessary
	-   Client is blocked
	-   Lower degree of parallelity

## Asynchronous Communication
- Pros:
	-   Loose coupling
	-   Higher degree of parallelity
	-   Enables faster sending than transmitting
	-   May compensate speed deviation between sender and receiver (but not speed differences)
	-   Sender and receiver have not to run on the same time
- Cons
	-   Complicates synchronisation
	-   Sender has no information about message delivery
	-   Possible buffer overflows

---
[[MOM]]