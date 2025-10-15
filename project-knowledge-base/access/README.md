# Access Requirements

Before contributing to the project, ensure you have the following access:

## 1. Source Control
- Platform: `git.example.com`
- Repositories: `repo1`, `repo2`, `repo-common`
- Access Level: **Write** for developers, **Admin** for leads
- Request via: `#access-requests` Slack channel or internal access portal

## 2. CI/CD Server
- Server: `jenkins.example.com`
- Group: `project-alpha-builders`
- Permissions: View, Build, Configure jobs (depending on your role)
- Contact: `jenkins-admins@example.com`

## 3. Artifact Repository
- URL: `artifacts.example.com`
- Namespace: `project-alpha`
- Required Roles: `developer` (pull/push)
- Request access through: internal **DevOps Access Portal**

## 4. Cluster Access (Kubernetes/OpenShift)
- Cluster: `alpha-cluster-prod`
- Namespace: `alpha-runtime`
- Login Example:
```bash
oc login --token=<TOKEN> --server=https://cluster.example.com
```

Permissions: view or edit

Request via: cluster-access@example.com
