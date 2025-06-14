
# 🔧 Git & GitHub Workflow Guide (By Gurubabu)

This guide explains the standard Git workflow followed in professional development environments. It ensures consistent collaboration, code quality, and secure access control.

---

## 🚀 Git Workflow: Step-by-Step

### ✅ Step 1: Request Access

If you need access to a private repository:

```
Hi DevOps team, I need access to the `rental-listing` repository.
My GitHub username is `gurubabu-dev`. Thanks!
```

The DevOps/IT team grants access and responds:

```
Hi Gurubabu, you've been granted read-write access to `rental-listing`.
You may now clone and push changes.
```

---

### ✅ Step 2: Clone Repository

```bash
git clone https://github.com/company/rental-listing.git
cd rental-listing
```

---

### ✅ Step 3: Create a Branch

```bash
git checkout -b feature/add-user-profile
```

**Branch Naming Conventions:**
- `feature/<name>` for new features  
- `fix/<name>` for bug fixes  
- `hotfix/<name>` for urgent production issues

---

### ✅ Step 4: Make and Commit Changes

Make your code changes:

```javascript
// user-profile.js
console.log("User Profile feature added by Gurubabu");
```

Then commit them:

```bash
git add .
git commit -m "Added user profile feature"
```

---

### ✅ Step 5: Push to Remote

```bash
git push origin feature/add-user-profile
```

---

### ✅ Step 6: Create Pull Request (PR)

- Go to GitHub
- Click **"Compare & Pull Request"**
- Add a **title** and **description**
- Assign reviewers

---

### ✅ Step 7: Code Review

Your team lead or reviewer (e.g., Emily) reviews the changes and leaves comments.  
Address feedback by making additional commits to the same branch.

---

### ✅ Step 8: Merge Changes

Once approved:

```bash
git checkout main
git merge feature/add-user-profile
git push origin main
```

Or use the **"Merge Pull Request"** button on GitHub.

---

### ✅ Step 9: CI/CD Deployment

Once merged, the CI/CD pipeline (e.g., Jenkins, GitHub Actions) will deploy the changes to staging or production automatically.

---

### ✅ Step 10: Monitor and Maintain

Monitor the deployed application for bugs or issues.  
For any hotfixes, create a branch like `hotfix/fix-issue-name` and follow the same process.

---

## 🔐 Access Levels in Git

| Permission | Description                    |
|------------|--------------------------------|
| Read       | Clone & pull code              |
| Write      | Push commits, create PRs       |
| Admin      | Manage settings & access       |

---

## 👥 Who Handles What?

| Role             | Responsibility                             |
|------------------|---------------------------------------------|
| Developer        | Feature/bug development, PR creation        |
| DevOps Engineer  | CI/CD, access control, repo settings        |
| Project Manager  | Timeline, resourcing, high-level oversight  |
| Reviewer/Lead    | Code reviews, merges, release approvals     |

---

## 📌 Example Developer Workflow (Gurubabu)

1. **Access Request:**  
   Gurubabu sends a request for access to `rental-listing`.

2. **Access Granted:**  
   DevOps grants Gurubabu read-write access.

3. **Feature Development:**  
   Creates a branch: `feature/add-user-profile`

4. **Code Commit:**  
   Adds a console log:  
   ```js
   console.log("Feature added by Gurubabu");
   ```

5. **Push & PR:**  
   Pushes branch and opens a PR titled:  
   `"Added user profile feature"`

6. **Code Review & Merge:**  
   Reviewer (Emily) reviews and merges the PR.

7. **Deployment & Monitor:**  
   CI/CD pipeline deploys it, and Gurubabu monitors logs.

---

## 🧑‍🏫 For New Team Members

- Follow this guide for all code contributions.
- Always create a feature or fix branch.
- Never commit directly to `main` or `master`.

---

## ✍️ Created by:

**Gurubabu Vallam** – Java Full Stack Developer  
📧 gurubabu@example.com  
🔗 [LinkedIn](https://linkedin.com/in/gurubabu-vallam)
