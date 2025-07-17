#  Lint-Test Deployment Pipeline

[![CI/CD Pipeline](https://github.com/melvinsamuel070/lint-test-dplmt/actions/workflows/main.yml/badge.svg)](https://github.com/melvinsamuel070/lint-test-dplmt/actions)
[![Pages Deployment](https://img.shields.io/github/deployments/melvinsamuel070/lint-test-dplmt/github-pages?label=GitHub%20Pages)](https://melvinsamuel070.github.io/lint-test-dplmt/)

This project demonstrates a complete **CI/CD workflow** using **GitHub Actions** for a simple React app, with automated deployment to **GitHub Pages**.

---

##  Project Overview

This repository contains a static React application with the following CI/CD pipeline components:

- **Linting** using ESLint
- **Testing** using Jest (or React Testing Library)
- **Build** process for production
- **Deployment** to GitHub Pages

---

##  CI/CD Pipeline Details

The GitHub Actions workflow is triggered **on every push** to the `master` branch.

###  Steps Performed

| Step            | Description                                                             |
|-----------------|-------------------------------------------------------------------------|
|  Checkout      | Clones the repository to the runner                                     |
|  Setup Node.js | Initializes Node.js version 20                                           |
|  Install       | Installs dependencies via `npm install`                                 |
|  Lint          | Runs ESLint checks for code quality                                     |
|  Test          | Executes unit tests (via `npm test`)                                    |
|  Build         | Compiles the app into the `build/` folder using `npm run build`         |
|  Deploy        | Deploys the `build/` folder to GitHub Pages via `gh-pages` branch       |

---

##  Live Site

 **[View Deployed Site](https://melvinsamuel070.github.io/lint-test-dplmt/)**  
Deployed automatically after each push to `master`.

---

##  Workflow File

The GitHub Actions configuration is located at:

```bash
.github/workflows/deploy.yml
Testing deployment
