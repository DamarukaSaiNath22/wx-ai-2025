# Tools Documentation

## Overview
This document lists the tools used by Company ABC's engineering team and provides setup instructions.

## Core Tools
1. **Git**
   - Version: 2.30+
   - Setup: Install via `brew install git` (Mac) or `apt-get install git` (Linux).
   - Config: `git config --global user.email "john.doe@abc.com"`

2. **Docker**
   - Version: 20.10+
   - Setup: Install from [docker.com](https://docker.com).
   - Usage: Run `docker-compose up` in Repo 1/Repo 2 for local services.

3. **Node.js**
   - Version: 16.x
   - Setup: Install via `nvm install 16` (see [nvm](https://github.com/nvm-sh/nvm)).
   - Usage: Required for Repo 2 frontend development.

4. **VS Code**
   - Recommended Extensions: ESLint, Prettier, AWS Toolkit.
   - Setup: Download from [code.visualstudio.com](https://code.visualstudio.com).

## Additional Tools
- **Postman**: For API testing (`api.abc.com` endpoints).
- **AWS CLI**: Install via `pip install awscli` for AWS access.

## Setup Checklist
1. Install Git, Docker, Node.js, and VS Code.
2. Configure AWS CLI with your IAM credentials: `aws configure`.
3. Clone Repo 1 and Repo 2: `git clone github.com/abc/repo1`.
4. Verify setup by running `make test` in each repo.

## Support
- **Tool Issues**: Contact tools@abc.com.
- **Slack**: #tools-help

Last Updated: October 15, 2025
