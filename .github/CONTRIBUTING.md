# Contributing to PDFTranscoder-AI-Powered-PDF-To-Spoken-Audio-Web-App

Thank you for considering contributing to the PDFTranscoder project! We welcome your contributions to improve this AI-powered PDF to spoken audio web application.

## 1. Code of Conduct

This project adheres to the Contributor Covenant Code of Conduct. Please make sure to read and follow it to ensure a positive and inclusive community. [Code of Conduct](https://github.com/chirag127/PDFTranscoder-AI-Powered-PDF-To-Spoken-Audio-Web-App/blob/main/CODE_OF_CONDUCT.md)

## 2. How to Contribute

We accept contributions in various forms, including:

*   **Bug Reports:** Please submit detailed bug reports via GitHub Issues, including steps to reproduce the issue, expected behavior, and actual behavior.
*   **Feature Requests:** Suggest new features or improvements through GitHub Issues.
*   **Code Contributions:** Submit Pull Requests for bug fixes or new features.

## 3. Development Setup

To set up your development environment:

1.  **Clone the Repository:**
    bash
    git clone https://github.com/chirag127/PDFTranscoder-AI-Powered-PDF-To-Spoken-Audio-Web-App.git
    cd PDFTranscoder-AI-Powered-PDF-To-Spoken-Audio-Web-App
    

2.  **Install Dependencies:**
    Since this is a JavaScript project, you'll typically use npm or yarn.
    bash
    # Using npm
    npm install

    # Or using yarn
    # yarn install
    

3.  **Build and Run:**
    Refer to the `README.md` for specific build and run commands.

## 4. Contributing Guidelines

*   **Branching:** Create a new branch for each feature or bug fix. Use a descriptive name (e.g., `feat/add-new-audio-format`, `fix/resolve-text-extraction-bug`).
*   **Pull Requests:**
    *   Submit PRs against the `main` branch.
    *   Ensure your code is well-commented and follows established JavaScript best practices.
    *   Include clear descriptions of your changes.
    *   Run all tests and ensure they pass before submitting.
*   **Testing:** All contributions must include comprehensive tests.
    *   Unit tests should be written using Vitest.
    *   End-to-end tests should be written using Playwright.
    *   Run tests using `npm test` or `yarn test`.
*   **Linting & Formatting:** Code must adhere to the linting and formatting rules enforced by Biome.
    *   Run the linter: `npm run lint` or `yarn lint`
    *   Run the formatter: `npm run format` or `yarn format`
*   **Code Style:** Follow the principles outlined in the `AGENTS.md` document, particularly regarding AI integration and architectural patterns.

## 5. AI Agent Directives

This project leverages AI, specifically Google Gemini, for core functionality. When contributing:

*   **Model Versioning:** Be mindful of the AI model versions used (e.g., `gemini-3-pro`). Ensure compatibility or clearly document any version changes.
*   **API Keys:** Never commit API keys directly into the codebase. Use environment variables (e.g., `.env` files for local development).
*   **AI Interaction Logic:** Ensure AI interaction logic is modular, well-abstracted, and includes robust error handling and retry mechanisms.
*   **Prompt Engineering:** When modifying prompts, consider clarity, conciseness, and the AI model's capabilities to achieve the desired output for PDF processing and audio generation.
*   **Ethical AI:** Adhere to ethical AI principles, avoiding bias and ensuring responsible use of AI technologies.

## 6. Submitting Your Changes

1.  Ensure your local `main` branch is up-to-date:
    bash
    git checkout main
    git pull origin main
    
2.  Create a feature branch: `git checkout -b my-new-feature`
3.  Make your changes and commit them.
4.  Run tests and linting.
5.  Push your branch: `git push origin my-new-feature`
6.  Open a Pull Request on GitHub.

We look forward to your contributions!
