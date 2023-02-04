---
tags:
- AWS-Dienst
- AWS
- Stoarage
- CDN
---

Eine Möglichkeit, auf geschützte Objekte in S3 zuzugreifen, besteht darin, eine signierte URL zu generieren, die einen begrenzten Zeitraum gültig ist.

- Signed URLs: sharing objects, all objects are private by default
	- *presigned URL:* sharing objects using their own security credentials (permissions for specific users)
		- provide your own credentials, bucket name, HTTP method, expiration date and time or token
		- CloudFront Policy
	- same permission as AMI user
	- Single File

---
[[S3 & CloudFront]]