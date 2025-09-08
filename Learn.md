# GitHub Workflow via Terminal (Step-by-Step Guide)

step-by-step guide to create and manage a GitHub repository entirely via the terminal.


## 1. Create a New Repo on GitHub
1. Go to **GitHub.. New Repository**.  
2. Name it, e.g., `repo-terminal`.  
3. Leave it empty.  
4. Copy the **HTTPS URL** of the repo.  


## 2. Set Up Local Project

# Create a new folder and navigate into it
mkdir hello-world-terminal
cd hello-world-terminal

# Initialize git
git init

## 3. Add your first file
echo "# Learning GitHub via Terminal" > README.md

## 4. Stage & Commit
git add README.md
git commit -m "Initial commit: add README"

## 5. Link Local Repo to GitHub
git remote add origin <repo-url>

## 6. Push to GitHub
git branch -M main
git push -u origin main

## 7. Basic Daily Operations

# Check repo status

git status

# Add a new file

echo "print('Hello, GitHub!')" > app.py
git add app.py
git commit -m "Add app.py with hello message"
git push origin main


# Pull latest changes

git pull origin main

# Create a new feature branch

git checkout -b feature/new-feature

git add .
git commit -m "Implement new feature"
git push origin feature/new-feature

