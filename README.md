# 🚀 My First GitHub Actions Workflow

Welcome! This repository was created as part of a hands-on practice task during the **Datacom Virtual Experience Program** on [Forage](https://www.theforage.com/). It demonstrates my understanding of **GitHub Actions** – a key tool in modern DevOps and software development.

---

## 📌 What This Repo Contains

This task showcases a simple GitHub Actions workflow that:

- Triggers on **push** or **pull request** events
- Checks out the repository code
- Runs sample shell commands to validate the pipeline

It's a foundational setup for CI/CD workflows.

---

## 🛠️ Technologies & Tools Used

- **Git** (Version Control)
- **GitHub** (Remote Repository)
- **GitHub Actions** (CI/CD Automation)
- **YAML** (Workflow configuration)
- **VS Code** (for local development)

---

## 🧠 What I Learned

- How to create and clone a GitHub repository
- How to configure Git locally
- How to write a basic GitHub Actions workflow in YAML
- How CI/CD pipelines are triggered and run in GitHub
- The importance of variables in GitHub Actions

---

## 📂 Workflow File Preview

Here’s a snapshot of the workflow used in this repository:

```yaml
name: GitHub Actions Demo

on:
  push:
  pull_request:

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout repository
        uses: actions/checkout@v3
      
      - name: Run a one-line script
        run: echo "Hello, world!"

      - name: Run a multi-line script
        run: |
          echo "Add other actions to build,"
          echo "test, and deploy your project."
---

