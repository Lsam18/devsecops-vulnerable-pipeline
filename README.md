# DevSecOps Vulnerable Pipeline

This project demonstrates how to build a **free**, beginner-friendly Application Security CI/CD pipeline using GitHub Actions.

## Overview

The pipeline integrates automated security scanning tools to help identify vulnerabilities early in the development process. It runs on every push or pull request to the repository.

## Tools Used

- **Semgrep** — Static Application Security Testing (SAST) tool to analyze source code for security issues.  
- **OWASP ZAP** — Dynamic Application Security Testing (DAST) tool to scan live web applications for vulnerabilities.  
- **GitHub Actions** — Automates the CI/CD workflow to run security scans automatically.

## What It Does

- Runs Semgrep to check the source code for common security issues.  
- Runs OWASP ZAP baseline scan against the OWASP Juice Shop demo app (`https://juice-shop.herokuapp.com`) to detect real-world vulnerabilities such as missing security headers and insecure cookies.

## How to Use

1. Fork this repository.  
2. Make changes or add your own code.  
3. On every push or pull request, the pipeline runs automated security scans.  
4. Review the scan results in the GitHub Actions tab.

## Learnings

- How to integrate security tools into a CI/CD pipeline.  
- Basics of SAST and DAST in application security.  
- Practical hands-on with GitHub Actions workflows.  
- Understanding of vulnerabilities detected in web apps.

---

Feel free to fork, improve, and customize this pipeline to fit your projects!

---

*This project is perfect for beginners looking to build DevSecOps and Application Security skills using fully free and open-source tools.*
