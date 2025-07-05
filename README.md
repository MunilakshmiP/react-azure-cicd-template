# 🌿 Feature Branch – Auto Pull Request + Auto-Merge

This is a **feature branch**, such as:
- `feature/login-page`
- `feature/fix-navbar`
- `feature/add-footer`

Every push to a `feature/*` branch triggers an **automated GitHub Actions workflow** that:

1. 📩 Creates a **pull request** to `dev`
2. ⚙️ Enables **GitHub-native auto-merge**
3. ⏳ Waits for the required approval(s)
4. ✅ Once approved, GitHub merges the PR using **squash**

---

