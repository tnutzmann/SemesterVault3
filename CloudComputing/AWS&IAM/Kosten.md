---
tags:
- AWS
- AWS-Dienste
- Cost
---

## relative Kosten

| **viel** | **wenig** | **nichts** |
|---|---|---|
|  Loadbalancer | EC2 | Security Group |
| RDS Datenbank | S3 | Key Pairs |
|| Secret Manager | Launch Templates|
|| AMI | Target Groups |
|| SQS* | Auto Scaling Group |
|| CloudFront* |
*\*keine Kosten bis zu einem Limit*

> Kosten für AWS-Dienste entstehen nur dann, wenn diese tatsächlich genutzt werden. Es gibt unterschiedliche Preismodelle für die verschiedenen Dienste, die sich z.B. nach der Art und Größe der genutzten Ressourcen, der Nutzungsdauer oder dem Datenverkehr richten können.

---
[[AWS & IAM]]