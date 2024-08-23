# Elastic Container Registry

## Log in Docker Engine to ECR 

```bash
aws ecr get-login-password | docker login --username AWS --password-stdin 419456231856.dkr.ecr.us-gov-west-1.amazonaws.com
```