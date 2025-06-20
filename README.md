# DevSecOps Vulnerable Pipeline

A **free**, beginner-friendly Application Security CI/CD pipeline built with GitHub Actions.

---

## Overview

This project demonstrates how to integrate automated security testing into your CI/CD workflow. It helps developers identify security vulnerabilities early by running multiple security tools automatically on every code change.

The pipeline runs on every push or pull request to the `main` branch, scanning both source code and the deployed web application.

---

## Security Tools Integrated

- **Semgrep** — Static Application Security Testing (SAST) for finding vulnerabilities directly in your source code.
- **OWASP ZAP** — Dynamic Application Security Testing (DAST) to scan running web applications for real-world security issues.
- **npm audit** — Checks project dependencies for known vulnerabilities.
- **ESLint** — Enforces code quality and catches potential security pitfalls in JavaScript.
- **Gitleaks** — Detects accidentally committed secrets in your repository.

---

## What the Pipeline Does

- Performs static code analysis with Semgrep to detect security issues early.  
- Runs OWASP ZAP Baseline Scan against the OWASP Juice Shop demo app (`https://juice-shop.herokuapp.com`) to identify runtime vulnerabilities such as missing security headers and insecure cookies.  
- Scans npm dependencies for vulnerabilities using `npm audit`.  
- Lints JavaScript code with ESLint to ensure quality and avoid common mistakes.  
- Scans the repository for secrets using Gitleaks.

---

## Getting Started

1. **Fork or clone** this repository to your GitHub account.  
2. **Customize** the workflow YAML if needed (e.g., change target URL for ZAP scans).  
3. **Push** your changes or open a pull request to trigger the pipeline.  
4. **Review** scan results and reports in the GitHub Actions tab.

---

## Reports & Artifacts

- OWASP ZAP generates detailed HTML reports available as build artifacts for easy review.  
- Semgrep, npm audit, ESLint, and Gitleaks output logs and warnings directly visible in the workflow logs.

---

## What I Learned

- How to integrate and orchestrate multiple security tools in a CI/CD pipeline.  
- The difference between static and dynamic application security testing.  
- Automating vulnerability scanning to reduce manual effort.  
- Handling GitHub Actions permissions and Docker image management.

---

## Future Enhancements

- Add more scanning tools like Snyk, Trivy, or CodeQL for broader coverage.  
- Automate remediation suggestions or enforce stricter failure policies.  
- Add notifications (Slack, email) for faster team awareness.  
- Extend support for multiple programming languages and frameworks.

---

## Contribution

Contributions, improvements, and suggestions are welcome! Feel free to open issues or pull requests.

---

*This project is ideal for beginners to gain hands-on experience with DevSecOps and Application Security using fully free and open-source tools.*

---

## Contact

For any questions or feedback, reach out to me at:

**LAKSHAN SAMEER** — lakshan.sam28@gmail.com — [GitHub Profile](https://github.com/Lsam18)

---

