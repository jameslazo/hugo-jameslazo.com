---
title: "API Server"
link: "https://medium.com/@james.lazo/day-4-devops-challenge-containerized-api-73a6006c6ca2"
image: "/img/api-server.png"
description: "Served parsed API game data in multi-AZ load-balanced configuration"
tags: ["DevOps","AWS","IaC","GitHub Actions","Terraform","Python","containers","Docker","ALB","load-balancing","high availability"]
fact: "a"
featured: false
---

- Provisioned entire data lake pipeline as IaC with Terraform
- Automated CI/CD workflow deploying Lambda functions to AWS with GitHub Actions
- Decoupled API call function from data extraction function with S3 bucket trigger
- Configured CloudWatch logs for observability & troubleshooting
