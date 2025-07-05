# React App CI/CD Pipeline (Azure + GitHub Actions)

This repo showcases a CI/CD pipeline using GitHub Actions and Azure App Services.

## 🔁 Workflow Summary
- Feature branches trigger auto-pull requests → require 2 approvals → auto-merge to `dev`
- `dev` branch triggers React build and deployment to Azure

## 📦 Tools Used
- GitHub Actions
- Azure App Services
- Node.js + Vite
- jq, curl

## 🚀 Deployment Trigger
```bash
git checkout -b feature/my-ui-change
# make changes
git push origin feature/my-ui-change
