# Day 1 – GitHub Actions Secrets and Variables

## Overview

This repository demonstrates the implementation and usage of **GitHub Actions Secrets and Variables** as part of DevOps learning.

The objective is to understand how to securely manage sensitive information, configure environment variables, and use secrets in GitHub Actions workflows.

## Objectives

- Understand GitHub Actions Secrets and Variables.
- Learn how to create and manage repository secrets.
- Configure environment variables in GitHub Actions.
- Understand the difference between Secrets and Variables.
- Securely manage Docker Hub credentials.
- Implement secrets in CI/CD workflows.
- Understand how GitHub masks sensitive information in workflow logs.

## Topics Covered

### 1. GitHub Actions

GitHub Actions is a CI/CD automation platform that helps automate software development workflows directly within GitHub repositories.

### 2. GitHub Secrets

GitHub Secrets are used to store sensitive information securely.

Examples:
- Docker Hub Username
- Docker Hub Password or Access Token
- API Keys
- Access Tokens

Secrets can be accessed inside workflows using:

```yaml
${{ secrets.SECRET_NAME }}
```

### 3. GitHub Variables

GitHub Variables are used to store non-sensitive configuration information.

Examples:
- Application Name
- Environment Name
- Docker Image Name
- Deployment Environment

Variables can be accessed using:

```yaml
${{ vars.VARIABLE_NAME }}
```

### 4. Difference Between Secrets and Variables

| GitHub Secrets | GitHub Variables |
|---|---|
| Store sensitive information | Store non-sensitive information |
| Masked in workflow logs | Not automatically masked |
| Used for passwords and tokens | Used for configuration |
| Accessed using `secrets` | Accessed using `vars` |

### 5. Docker Hub Authentication

Docker Hub credentials are stored as GitHub repository secrets.

Example secret names:

- `DOCKER_USERNAME`
- `DOCKER_PASSWORD`

These credentials can be used in GitHub Actions to authenticate with Docker Hub without exposing sensitive information in the workflow file.

### 6. Secret Masking

GitHub Actions automatically masks registered secrets in workflow logs to help prevent accidental exposure.

Sensitive values should never be hardcoded or printed in workflow files.

## Technologies Used

- Git
- GitHub
- GitHub Actions
- YAML
- Docker
- Docker Hub
- CI/CD

## Repository Structure

```text
Day-1-screts-varabiles/
│
├── .github/
│   └── workflows/
│       └── main.yml
│
└── README.md
```

*Note: Update the workflow filename and structure according to your actual repository files.*

## Implementation Steps

1. Created a GitHub repository for Day 1 Secrets and Variables practice.
2. Explored GitHub Actions workflows and YAML configuration.
3. Created repository secrets and variables.
4. Configured Docker Hub credentials as GitHub Secrets.
5. Accessed secrets and variables inside the workflow.
6. Practiced secure credential management and secret masking.
7. Executed the GitHub Actions workflow and verified its execution.

## Expected Outcome

Successfully understood and implemented GitHub Actions Secrets and Variables.

Learned how to securely manage Docker Hub credentials, access environment variables, and protect sensitive information in CI/CD workflows.

## Key Learnings

- Understanding GitHub Actions fundamentals.
- Managing repository-level secrets and variables.
- Secure handling of credentials.
- Using secrets and variables in YAML workflows.
- Understanding secret masking.
- Integrating Docker Hub authentication with GitHub Actions.

## Author

**Sharmila Medapati**

DevOps Learning – Day 1

