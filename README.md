# Demo Node.js Application Deployment to Azure

This repository contains a demo Node.js application and a GitHub Actions workflow for deploying the application to Azure Web Service.

## Prerequisites

- GitHub repository with the NodeJs application code.
- An Azure account with an active subscription.
- An Azure Web App already created for deployment.

##Configure GitHub Secrets
In your GitHub repository, go to Settings > Secrets and variables > Actions.
Add a new secret named AZURE_WEBAPP_PUBLISH_PROFILE and paste the content of your Azure publish profile which was obtained while creating web app service

##5. GitHub Actions Workflow
The GitHub Actions workflow file is located at .github/workflows/deploy.yml. This workflow will:

Install dependencies.
Run tests.
Fix vulnerabilities.
Deploy the application to Azure Web App.

Once deployed you can access the application at default domain name configured at azure portal
