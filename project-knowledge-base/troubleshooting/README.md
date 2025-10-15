# Troubleshooting Documentation

## Overview
This document provides solutions to common issues encountered in Company ABC's engineering workflows.

## Common Issues
1. **GitHub Access Denied**
   - **Symptom**: `Permission denied` when cloning Repo 1/Repo 2.
   - **Solution**: Ensure your GitHub account is in the `abc-engineering` team. Contact git-admins@abc.com.

2. **AWS CLI Authentication Failure**
   - **Symptom**: `Invalid credentials` when running `aws s3 ls`.
   - **Solution**: Re-run `aws configure` with your IAM credentials or refresh MFA token.

3. **Docker Build Fails**
   - **Symptom**: `docker-compose up` fails with `image not found`.
   - **Solution**: Pull latest images: `docker-compose pull`. Check [Tools README](../tools/README.md).

4. **Pipeline Failure**
   - **Symptom**: GitHub Actions workflow fails on `test` stage.
   - **Solution**: Check logs in GitHub UI. Run `make test` locally to reproduce.

5. **Application Downtime**
   - **Symptom**: `dev.app.abc.com` returns 500 error.
   - **Solution**: Check CloudWatch logs (`aws.amazon.com/cloudwatch`). Notify infra@abc.com.

## Debugging Tips
- Always check logs in CloudWatch or GitHub Actions.
- Reproduce issues locally using `docker-compose`.
- Search Confluence for similar issues: `confluence.abc.com`.

## Escalation
- **Urgent Issues**: Email infra@abc.com or ping #infra-support on Slack.
- **Non-Urgent**: File a Jira ticket: `jira.abc.com`.

Last Updated: October 15, 2025
