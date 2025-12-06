# 🤝 Contributing to PDF-To-Speech-AI-Converter-Web-App

We welcome contributions to the `PDF-To-Speech-AI-Converter-Web-App` project! As a testament to our commitment to excellence, we adhere to the **Apex Technical Authority** standards, ensuring that all contributions are professional, well-tested, and align with our future-proof architecture.

## 🚀 Our Vision & Philosophy

*   **Zero-Defect, High-Velocity, Future-Proof:** We strive for quality and speed without compromising long-term maintainability.
*   **Elite Standards:** All code, documentation, and contributions must meet FAANG-level quality benchmarks.
*   **Professional Archival:** Even retired features are treated as valuable, well-documented assets.

## 🛠️ Development Environment Setup

To contribute effectively, you'll need to set up a local development environment that mirrors our production stack.

1.  **Clone the Repository:**
    bash
    git clone https://github.com/chirag127/PDF-To-Speech-AI-Converter-Web-App.git
    cd PDF-To-Speech-AI-Converter-Web-App
    

2.  **Install Dependencies:**
    This project uses **Node.js** and **npm** (or yarn/pnpm). Ensure you have Node.js v20+ installed.
    bash
    npm install
    # or
    # yarn install
    # or
    # pnpm install
    

3.  **Environment Variables:**
    Some features, particularly AI integrations, might require API keys. Create a `.env` file in the root directory. Refer to `.env.example` for structure.
    bash
    cp .env.example .env
    # Populate your API keys in .env
    

## ✅ Contribution Workflow

Follow these steps for all contributions:

1.  **Fork the Repository:** Create your own fork of `chirag127/PDF-To-Speech-AI-Converter-Web-App`.
2.  **Create a New Branch:** Create a descriptive branch for your feature or bug fix.
    bash
    git checkout -b feature/your-feature-name
    # or
    # git checkout -b fix/your-bug-fix
    
3.  **Make Your Changes:** Implement your solution, adhering to our coding standards.
4.  **Test Your Changes:** Ensure all existing tests pass and add new tests for your modifications.
    bash
    npm run test
    
5.  **Lint and Format:** Ensure your code is clean and adheres to our style guide.
    bash
    npm run lint
    npm run format
    
6.  **Commit Your Changes:** Write clear, concise commit messages.
    bash
    git add .
    git commit -m "feat: Add new PDF processing capability"
    
7.  **Push to Your Fork:** Push your branch to your forked repository.
    bash
    git push origin feature/your-feature-name
    
8.  **Open a Pull Request:** Create a Pull Request against the `main` branch of the `chirag127/PDF-To-Speech-AI-Converter-Web-App` repository.

## 📜 Coding Standards & Principles

We expect all code to adhere to the following principles:

*   **SOLID Principles:** (Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, Dependency Inversion)
*   **DRY (Don't Repeat Yourself):** Avoid redundant code.
*   **KISS (Keep It Simple, Stupid):** Prioritize simplicity and clarity.
*   **YAGNI (You Ain't Gonna Need It):** Implement only what is necessary now.
*   **Type Safety:** Utilize TypeScript's strict typing features to prevent runtime errors.
*   **Error Handling:** Implement robust error handling, especially for external API calls (e.g., Gemini AI) and user input.

## 🤖 AI Agent Directives

Our development process is augmented by AI agents. Refer to the `AGENTS.md` file for detailed directives that guide their operation and how they interact with the codebase. When contributing, ensure your changes are compatible with these directives.

## 📈 Testing

Comprehensive testing is crucial. We utilize the following testing frameworks:

*   **Vitest:** For fast unit and integration testing.
*   **Playwright:** For end-to-end (E2E) testing of the user interface and workflows.

Run all tests before submitting a Pull Request:

bash
# Run unit and integration tests
npm run test

# Run end-to-end tests (requires separate setup or specific script)
# npm run test:e2e


## 🐞 Bug Reports

If you find a bug, please open an issue using the `bug_report.md` template. Provide as much detail as possible, including steps to reproduce, expected behavior, and actual behavior.

## ✨ Feature Requests

For new feature ideas, please open an issue and describe your proposed feature, its benefits, and potential implementation ideas.

## ⚖️ License

By contributing to this project, you agree that your contributions will be licensed under the **CC BY-NC 4.0** license, as specified in the `LICENSE` file.

---