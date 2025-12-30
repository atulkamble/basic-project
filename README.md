# 🚀 Very Basic Project – Create, Run, Host (CLI Only)

## 🧱 Project Type

We’ll use **HTML + Shell script** because:

* No dependencies
* Runs on **any OS**
* Perfect for demos, students, DevOps basics

---

## 1️⃣ Create Project from CLI

```bash
mkdir hello-git
cd hello-git
```

Verify:

```bash
pwd
```

---

## 2️⃣ Create Code Files

### 🔹 Create HTML file

```bash
nano index.html
```

Paste:

```html
<!DOCTYPE html>
<html>
<head>
  <title>Hello Git</title>
</head>
<body>
  <h1>Hello from Git CLI 🚀</h1>
  <p>This project was created and run from terminal.</p>
</body>
</html>
```

Save → `CTRL + O` → `ENTER` → `CTRL + X`

---

### 🔹 Create Shell Script (Runnable Code)

```bash
nano run.sh
```

```bash
#!/bin/bash
echo "================================="
echo " Hello! Project is running 🚀"
echo " Current Directory: $(pwd)"
echo " Date: $(date)"
echo "================================="
```

Make it executable:

```bash
chmod +x run.sh
```

---

## 3️⃣ ▶️ RUN THE PROJECT (LOCAL)

### ✅ Run Shell Script

```bash
./run.sh
```

📌 Output:

```
Hello! Project is running 🚀
Current Directory: /Users/atul/hello-git
Date: Mon Dec 30 11:20:00 IST 2025
```

✔️ **This proves the project runs locally**

---

### ✅ Run HTML File

Option 1 (Mac/Linux):

```bash
open index.html
```

Option 2 (Linux server):

```bash
python3 -m http.server 8080
```

Open browser:

```
http://localhost:8080
```

✔️ HTML page is running locally

---

## 4️⃣ Initialize Git

```bash
git init
git status
```

---

## 5️⃣ Commit Code

```bash
git add .
git commit -m "Initial basic project with run details"
```

---

## 6️⃣ Create GitHub Repo (Manual Way)

1. Open **github.com**
2. Click **New Repository**
3. Name: `hello-git`
4. Public
5. ❌ Do NOT add README
6. Create

---

## 7️⃣ Push Project to GitHub

```bash
git branch -M main
git remote add origin https://github.com/<your-username>/hello-git.git
git push -u origin main
```

✔️ Code is now **hosted on GitHub**

---

## 8️⃣ ▶️ RUN FROM GITHUB (Hosting)

### 🌐 Option A: GitHub Pages (HTML Hosting)

```bash
git checkout -b gh-pages
git push origin gh-pages
```

Then:

* Repo → **Settings**
* Pages → Source → `gh-pages`
* Save

🔗 Live URL:

```
https://<your-username>.github.io/hello-git/
```

✔️ Project is **running from GitHub (public)**

---

### 🖥️ Option B: Clone & Run Anywhere

Anyone can run your project:

```bash
git clone https://github.com/<your-username>/hello-git.git
cd hello-git
./run.sh
```

✔️ Works on **any Linux/Mac system**

---

## 📂 Final Repo Structure

```
hello-git/
├── index.html   # Runs in browser
├── run.sh       # Runs from terminal
└── README.md    # (optional)
```

---

## 🔥 What You Can Say in Interview

> “I created a project fully from CLI, ran it locally using shell scripts and HTTP server, version-controlled it with Git, and hosted it on GitHub with GitHub Pages.”

---

## 🧠 Key Commands to Remember

```bash
mkdir project
git init
git add .
git commit -m "msg"
git push
./run.sh
python3 -m http.server
```

---
