---
tags:
- cloud 
- AWS
- AWS-Dienst
---
## Serverless
- a cloud-native platform for 
	- short-running, stateless computation 
	- event-driven applications  
- scales up and down instantly and automatically
- charges for actual usage at a millisecond granularity 
- still runs on servers, but management is done by AWS 

## AWS Lambda
- Lambda functions: 
	- consist of code and any associated dependencies 
	- configuration information is associated with the function 
	- API provided for updating configuration data 
	- amount of memory specified at creation 
	- CPU power ~ memory (same ratio as a general purpose EC2) 
	- need an IAM role 
- Lambda Limits 
	- maximum execution timeout 
		- Max is 15 minutes (900 seconds), default is 3 seconds 
	- pay for run time 
	- Lambda terminates the function at the timeout
- Languages
	- Node.js
	- Python
	- Java
	- C# (.Net Core)
	- GoLang
![[Pasted image 20230131115211.png]]

---
[[Webservices]]