# Environments Documentation

## Overview
This document describes Company ABC's development, staging, and production environments.

## Environment Details
1. **Development (Dev)**
   - URL: `dev.app.abc.com`
   - AWS Account: `aws-dev-123456`
   - Purpose: Local and integration testing for Repo 1 and Repo 2.
   - Access: All engineers have read/write access.

2. **Staging**
   - URL: `staging.app.abc.com`
   - AWS Account: `aws-staging-456789`
   - Purpose: Pre-production testing and QA.
   - Access: Restricted to senior engineers and QA team.

3. **Production (Prod)**
   - URL: `app.abc.com`
   - AWS Account: `aws-prod-789012`
   - Purpose: Live customer-facing application.
   - Access: Read-only for most engineers; write access requires approval.

## Setup Instructions
- **Dev**: Clone Repo 1/Repo 2 and run `make setup-dev` (see [Tools README](../tools/README.md)).
- **Staging/Prod**: Use deployment pipelines (see [Pipelines README](../pipelines/README.md)).
- **Credentials**: Retrieve from AWS Secrets Manager (`abc/env/secrets`).

## Best Practices
- Test all changes in Dev before promoting to Staging.
- Avoid direct commits to Prod; use CI/CD pipelines.
- Monitor logs via CloudWatch: `aws.amazon.com/cloudwatch`.

## Contacts
- **Infra Team**: infra@abc.com
- **Slack**: #infra-support

Last Updated: October 15, 2025
