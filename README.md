# 🚀 React App CI/CD with GitHub Actions & Azure App Service

Welcome to this project! This repository demonstrates a full CI/CD pipeline for a React application using:

- GitHub Actions for automation  
- Azure App Service for deployment  
- Feature-based branching and PR approvals  
- Zero manual deployment steps

---

## 📘 What This Project Does

This project is set up to automate everything from code push → to pull request → to production-ready deployment:

### ✅ Key Highlights:
- Auto-creation of pull requests on any `feature/*` branch push
- Waits for 1 approval and merges to `dev` automatically
- Deployment to Azure happens **only from the `dev` branch**

> You write code → push → get coffee ☕ → your app is deployed 🚀

---

## 🧠 Branch Structure

| Branch        | Purpose                                  |
|---------------|-------------------------------------------|
| `main`        | Project overview and documentation only  |
| `feature/*`   | Developer work branches with auto PR      |
| `dev`         | Auto-deployment branch to Azure App Service |

> ✨ Detailed explanations about what happens in each of these branches are available in their respective README files.

---

## 📂 Guide Navigation

📄 In this `main` branch, you’ll find:
- Project overview
- Architecture insight
- Intro to workflows and structure

📄 In the `feature/*` branch, you’ll see:
- How auto PR and auto merge works using `feature-to-dev-pr.yml`

📄 In the `dev` branch, you’ll see:
- How the React app is built and deployed via `dev-deploy.yml`

Let’s deep dive into those branches to explore how everything works behind the scenes!
