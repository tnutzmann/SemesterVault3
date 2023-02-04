---
tags:
- AWS-Dienst
- AWS
- CDN
---
## Content Distribution Networks
ermöglichen es, statische Inhalte (wie Bilder, Videos, etc) über Edge-Locationen in der Nähe des Endbenutzers zu verteilen und damit die Ladezeiten zu reduzieren. AWS CloudFront ist ein CDN-Dienst von AWS der mit S3 zusammenarbeitet.

- Edge Location -> Nahe am Client
- Origin: 
	- S3 
	- ELB 
	- ec2 
	- Route53 
	- Lambda
- Distribution: name of the CDN which consists of several edge locations for content distribution
	- Unique URL
- TTL
- Invalidation == clear cache -> speparate fee
- Usage: static content (s3), streamed content (s3, media servers), dynamic content (ec2, Lambda, ELB), external servers

---
[[S3 & CloudFront]]