# Pipelines Documentation

## Overview
This document describes Company ABC's CI/CD pipelines for deploying Repo 1 and Repo 2.

## Pipeline Overview
- **Tool**: GitHub Actions
- **Repos**: Repo 1 (Backend), Repo 2 (Frontend)
- **Workflows**: Lint, Test, Build, Deploy

## Pipeline Details
1. **Repo 1 (Backend)**
   - Workflow File: `.github/workflows/backend.yml`
   - Stages:
     - Lint: Runs `eslint` on pull requests.
     - Test: Runs `jest` for unit tests.
     - Build: Creates Docker image (`abc/backend:tag`).
     - Deploy: Pushes to Dev (`dev.app.abc.com`) or Staging (`staging.app.abc.com`).
   - Prod Deploy: Manual approval required via GitHub UI.

2. **Repo 2 (Frontend)**
   - Workflow File: `.github/workflows/frontend.yml`
   - Stages:
     - Lint: Runs `prettier` and `eslint`.
     - Test: Runs `cypress` for E2E tests.
     - Build: Creates static assets (`dist/`).
     - Deploy: Syncs to S3 bucket (`s3://abc-frontend`).
   - Prod Deploy: Restricted to release managers.

## Running Locally
- Install GitHub Actions Runner: [docs.github.com/actions](https://docs.github.com/en/actions).
- Simulate pipeline: `act -j test` (requires `act` CLI).

## Best Practices
- Always create a pull request for code changes.
- Monitor pipeline status in GitHub Actions tab.
- Tag releases with `vX.Y.Z` format for Prod deploys.

## Contacts
- **DevOps Team**: devops@abc.com
- **Slack**: #cicd-support

Last Updated: October 15, 2025
