# Security Policy for PDF-To-Speech-AI-Converter-Web-App

## Our Commitment

The project maintainers take the security of the `PDF-To-Speech-AI-Converter-Web-App` seriously. We are committed to investigating and addressing all verified security vulnerabilities in a timely and responsible manner. We believe in and encourage responsible disclosure from the security community.

## Supported Versions

As a web-based application, only the latest version deployed to our primary production environment is considered supported. Vulnerabilities found in previous or un-deployed states of the code are not typically eligible for remediation unless they persist in the current version.

| Version | Supported          |
| ------- | ------------------ |
| Latest  | :white_check_mark: |

## Reporting a Vulnerability

We ask that you do not report security vulnerabilities through public GitHub issues. Instead, please use one of the private methods below.

### Primary Method: GitHub Private Vulnerability Reporting

We strongly prefer to receive vulnerability reports through GitHub's private vulnerability reporting feature. This ensures the information is kept confidential until we can address the issue.

**[Submit a private report via GitHub](https://github.com/chirag127/PDF-To-Speech-AI-Converter-Web-App/security/advisories/new)**

### What to Include

To help us resolve the issue quickly, please provide a detailed report that includes:

- A clear description of the vulnerability and its potential impact.
- Step-by-step instructions to reproduce the issue, including any required setup.
- Proof-of-concept (PoC) code, screenshots, or videos that demonstrate the vulnerability.
- Any suggestions for a potential fix, if you have any.

### What to Expect

After you submit a report, you can expect the following:

1.  **Acknowledgement:** We will acknowledge receipt of your report within 48 hours.
2.  **Triage & Validation:** We will investigate and validate the vulnerability.
3.  **Communication:** We will maintain an open line of communication, providing updates on our progress.
4.  **Resolution:** We will work to release a patch or mitigation as quickly as possible.
5.  **Disclosure & Credit:** Once the vulnerability is resolved, we will publish a security advisory and credit you for your contribution, unless you prefer to remain anonymous.

## Security Best Practices

We actively employ several security measures to protect our users and our application:

-   **Dependency Scanning:** We use **GitHub Dependabot** to automatically scan our dependencies for known vulnerabilities and create pull requests to update them.
-   **Static Code Analysis (SAST):** Our CI/CD pipeline includes automated code scanning with **GitHub CodeQL** to identify potential security flaws before they reach production.
-   **API Key Management:** All interactions with third-party services, such as the Gemini AI API, are handled through a secure backend proxy. API keys are never exposed on the client-side.
-   **Content Security Policy (CSP):** We enforce a strict Content Security Policy to mitigate the risk of cross-site scripting (XSS) and other code injection attacks.
-   **Input Sanitization:** All user-provided data, particularly the content from uploaded PDF files, is rigorously sanitized and validated to prevent injection attacks.
