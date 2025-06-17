# Mini Project
# 🖌️ Drawing Canvas Web App

A lightweight web-based drawing canvas tool that lets users draw using customizable brush sizes, select colors, use an eraser, and save their artwork. Built using HTML5, CSS3, and JavaScript.

---

## 📚 Project Objectives

This project was created as part of the Digital Transformation in Industry (DTI) open elective course at BMSIT&M. The main objectives were:

- Learn Git & GitHub for version control
- Create a Continuous Integration (CI) workflow using GitHub Actions
- Containerize the application using Docker
- Deploy a static site using GitHub Pages

---

## 📁 Project Structure


---

## ✅ Tasks Overview

| Task No. | Description                              | Tools Used            |
|----------|------------------------------------------|------------------------|
| Task 1   | Git & GitHub version control              | Git CLI, GitHub       |
| Task 2   | CI/CD pipeline setup                      | GitHub Actions        |
| Task 3   | Containerization                          | Docker, Nginx         |
| Task 4   | Static website hosting                    | GitHub Pages          |

---

## 🧪 Task Details

### 🧩 Task 1: Git Version Control

- Git repository initialized
- Changes tracked and committed
- Branch `dev` created
- Code pushed to GitHub

**Commands Used**:
```bash
git init
git add .
git commit -m "Initial commit"
git branch dev
git push origin dev


name: Check HTML File

on: [push]

jobs:
  validate:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout Code
        uses: actions/checkout@v3

      - name: Check index.html Exists
        run: |
          if [ -f "index.html" ]; then
            echo "index.html exists ✅"
          else
            echo "❌ index.html is missing"
            exit 1
          fi

