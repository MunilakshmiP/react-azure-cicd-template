# 🛠 dev Branch – React App Deployment to Azure

This branch represents the **staging environment** of the app. Any code merged here is **automatically deployed to Azure**.

---

## 🚀 What Happens Here?

When new code is pushed or merged into `dev`:
1. GitHub Actions triggers the `dev-deploy.yml` workflow
2. The workflow:
   - Installs dependencies
   - Builds the React app (via Vite or CRA)
   - Uploads the `dist/` folder
   - Deploys it to Azure App Service

---

## ⚙️ Workflow: `dev-deploy.yml`

Key steps include:
- Checkout code
- Node.js setup and `npm install`
- Run `npm run build`
- Validate that the `dist/` folder exists
- Upload build artifacts and logs
- Use Azure's `webapps-deploy` action to publish the app

---

## 🔐 Required GitHub Secret

| Secret Name             | Description                                                   |
|--------------------------|---------------------------------------------------------------|
| `AZURE_PUBLISH_PROFILE` | From Azure → Web App → "Get publish profile" XML file content |

Used for authentication to Azure App Services.

---

## 📂 What Should Be in `dev` Branch

- ✅ Full React source code (`src/`, `package.json`, etc.)
- ✅ `.github/workflows/dev-deploy.yml`

> ❌ Do not push feature code directly here — it should come from merged PRs via `feature/*`.

---

✅ Once merged here, the app is live on Azure — fully automated.
