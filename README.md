# DevOps Git Project

This is a simple Node.js project built to demonstrate Git best practices in a DevOps workflow.  
It covers initialization, branching, pull requests, tagging, and markdown documentation.

---

## 📁 Project Structure

devops-git-project/ │ ├── app.js # Simple Node.js file ├── package.json # Node.js 
metadata file ├── .gitignore # Ignored files like node_modules/ ├── README.md 
# Project documentation └── TASKS.md # List of tasks completed


---

## ✅ Tasks Completed

| Task | Status |
|------|--------|
| Initialize project | ✅ |
| Setup Git and GitHub | ✅ |
| Create `dev` and `feature` branches | ✅ |
| Create Pull Requests and merge | ✅ |
| Add `.gitignore` file | ✅ |
| Tag first version `v1.0` | ✅ |
| Document tasks in `TASKS.md` | ✅ |
| Create proper `README.md` | ✅ |

---

## 🔧 Commands Used

### 🔹 Initialize Project
```bash
mkdir devops-git-project
cd devops-git-project
npm init -y

# Create App File
nano app.js
# Inside: console.log("Hello from DevOps Git Project!");


🔹 Initialize Git and Push to GitHub
git init
git remote add origin https://github.com/github-for-challa/devops-git-project.git
git add .
git commit -m "Initial commit with basic Node.js setup"
git branch -M main
git push -u origin main

🔹 Create Branches
git checkout -b dev
git push -u origin dev

git checkout -b feature/add-readme

🔹 Create .gitignore
echo "node_modules/" > .gitignore
echo ".env" >> .gitignore
echo "*.log" >> .gitignore


🔹 Commit & Push Feature Branch
git add .
git commit -m "Add .gitignore file"
git push -u origin feature/add-gitignore

🔹 Create Pull Request via GitHub UI
Merged feature/add-gitignore → dev
Then merged dev → main

🔹 Tagging Version
git checkout main
git merge dev
git push
git tag -a v1.0 -m "Initial version"
git push origin v1.0

📄 Author
github-for-challa
This project is part of a DevOps learning series.
