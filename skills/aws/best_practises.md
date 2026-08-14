# AWS Best Practices

## Security

Always enable least privilege.

Rotate credentials.

Use MFA.

Encrypt data at rest.

Encrypt data in transit.

Never commit credentials.

---

## Compute

Prefer managed compute.

Avoid running idle EC2 instances.

Use Auto Scaling.

---

## Storage

Enable versioning.

Enable lifecycle rules.

Encrypt S3 buckets.

Block public access unless explicitly required.

---

## Networking

Separate production and development environments.

Use private subnets.

Restrict inbound traffic.

Avoid opening unnecessary ports.

---

## Monitoring

Enable:

CloudWatch

CloudTrail

AWS Config

GuardDuty

for production systems.

---

## Reliability

Deploy across multiple AZs.

Use health checks.

Enable automatic recovery.

Implement backups.

---

## Cost

Review idle resources.

Delete unused snapshots.

Use lifecycle policies.

Use Savings Plans for predictable workloads.

Monitor billing regularly.

---

## Infrastructure

Use Infrastructure as Code.

Keep templates version-controlled.

Review changes before deployment.

---

## IAM

Prefer roles over users.

Never share credentials.

Review permissions periodically.

---

## Databases

Enable backups.

Enable encryption.

Use Multi-AZ for production.

Monitor slow queries.

---

## Serverless

Keep Lambda functions small.

Reuse execution environments.

Minimize cold starts.

Use environment variables.

---

## Containers

Keep container images small.

Scan images.

Use ECR.

Avoid running containers as root.

---

## Architecture

Design for failure.

Automate deployments.

Automate recovery.

Automate monitoring.

Document architecture decisions.