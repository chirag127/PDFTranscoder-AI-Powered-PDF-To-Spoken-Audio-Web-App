<div align="center">
  <img src="https://raw.githubusercontent.com/chirag127/PDFTranscoder-AI-Powered-PDF-To-Spoken-Audio-Web-App/main/.github/assets/logo.png" alt="PDFTranscoder Logo" width="200">
  <h1>PDFTranscoder: AI-Powered PDF-to-Audio Web App</h1>
</div>

<div align="center">
  <a href="https://github.com/chirag127/PDFTranscoder-AI-Powered-PDF-To-Spoken-Audio-Web-App/actions/workflows/ci.yml">
    <img src="https://github.com/chirag127/PDFTranscoder-AI-Powered-PDF-To-Spoken-Audio-Web-App/actions/workflows/ci.yml/badge.svg?style=flat-square" alt="Build Status">
  </a>
  <a href="https://codecov.io/gh/chirag127/PDFTranscoder-AI-Powered-PDF-To-Spoken-Audio-Web-App">
    <img src="https://img.shields.io/codecov/c/github/chirag127/PDFTranscoder-AI-Powered-PDF-To-Spoken-Audio-Web-App?style=flat-square&token=PLACEHOLDER" alt="Code Coverage">
  </a>
  <img src="https://img.shields.io/badge/Tech-TypeScript%20%26%20Gemini%20AI-3178C6?style=flat-square" alt="Tech Stack">
  <img src="https://img.shields.io/badge/Lint-Biome-blueviolet?style=flat-square" alt="Linter">
  <a href="https://github.com/chirag127/PDFTranscoder-AI-Powered-PDF-To-Spoken-Audio-Web-App/blob/main/LICENSE">
    <img src="https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey?style=flat-square" alt="License">
  </a>
  <a href="https://github.com/chirag127/PDFTranscoder-AI-Powered-PDF-To-Spoken-Audio-Web-App/stargazers">
    <img src="https://img.shields.io/github/stars/chirag127/PDFTranscoder-AI-Powered-PDF-To-Spoken-Audio-Web-App?style=flat-square&label=Stars" alt="GitHub Stars">
  </a>
</div>

<div align="center">
  <br>
  <a href="https://github.com/chirag127/PDFTranscoder-AI-Powered-PDF-To-Spoken-Audio-Web-App/stargazers"><strong>Star ⭐ this Repo</strong></a> to support its development!
</div>

---

**PDFTranscoder transforms dense technical PDFs into clear, spoken-friendly audio directly in your browser. It uses Google Gemini AI to intelligently process complex layouts, formulas, and text, ensuring a natural and accessible listening experience for on-the-go learning.**

This tool is designed for professionals, students, and researchers who need to consume large volumes of technical documentation efficiently. Stop straining your eyes and start listening to your documents anytime, anywhere.

## Table of Contents

- [✨ Core Features](#-core-features)
- [🏛️ Architecture](#️-architecture)
- [🛠️ Technology Stack](#️-technology-stack)
- [🚀 Getting Started](#-getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [⚙️ Available Scripts](#️-available-scripts)
- [🤖 AI Agent Directives](#-ai-agent-directives)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)

## ✨ Core Features

- **🧠 AI-Powered Text Analysis:** Leverages Google Gemini to understand document structure, correctly interpret formulas, and handle complex technical jargon.
- **🗣️ Natural Speech Synthesis:** Converts processed text into high-quality, natural-sounding audio for an enjoyable listening experience.
- **🌐 Fully Browser-Based:** No software installation required. All processing happens securely in your browser, ensuring data privacy.
- **⚡ High-Performance Frontend:** Built with a modern TypeScript stack (Vite + React) for a blazing-fast and responsive user interface.
- **🔒 Secure & Private:** Your PDF files are processed locally and are never uploaded to a server, guaranteeing the confidentiality of your documents.

## 🏛️ Architecture

This project follows the **Feature-Sliced Design (FSD)** methodology, ensuring a scalable, maintainable, and highly-organized codebase. This modular approach isolates features and promotes low coupling between different parts of the application.

plaintext
src/
├── app/         # App-wide logic, providers, and global styles
├── pages/       # Complete pages (e.g., HomePage, ResultsPage)
├── widgets/     # Composite UI components (e.g., Header, PDFUploader)
├── features/    # Business logic features (e.g., processPdf, playAudio)
├── entities/    # Business entities (e.g., User, Document)
└── shared/      # Reusable modules, UI kit, APIs, and configs
    ├── api/     # API layer (e.g., geminiApi.ts)
    ├── ui/      # Core UI components (Button, Input, Spinner)
    └── lib/     # Helper functions and utilities


## 🛠️ Technology Stack

| Category          | Technology / Tool                                                                                               |
| ----------------- | --------------------------------------------------------------------------------------------------------------- |
| **Core Language**   | [**TypeScript**](https://www.typescriptlang.org/) (Strict Mode)                                                  |
| **Framework**     | [**React 19**](https://react.dev/)                                                                               |
| **Build Tool**    | [**Vite**](https://vitejs.dev/)                                                                                  |
| **AI Model**      | [**Google Gemini API**](https://ai.google.dev/)                                                                 |
| **Styling**       | [**Tailwind CSS**](https://tailwindcss.com/)                                                                     |
| **Linting/Format**| [**BiomeJS**](https://biomejs.dev/) (Ultra-fast linter & formatter)                                                |
| **Unit Testing**  | [**Vitest**](https://vitest.dev/)                                                                                |
| **E2E Testing**   | [**Playwright**](https://playwright.dev/)                                                                        |
| **Package Manager**| [**npm**](https://www.npmjs.com/)                                                                                |

## 🚀 Getting Started

Follow these steps to set up and run the project locally.

### Prerequisites

- Node.js (v20.x or higher)
- npm (v10.x or higher)
- A Google Gemini API Key

### Installation

1.  **Clone the repository:**
    sh
    git clone https://github.com/chirag127/PDFTranscoder-AI-Powered-PDF-To-Spoken-Audio-Web-App.git
    cd PDFTranscoder-AI-Powered-PDF-To-Spoken-Audio-Web-App
    

2.  **Install dependencies:**
    sh
    npm install
    

3.  **Set up environment variables:**
    Create a `.env.local` file in the root directory and add your Gemini API key:
    env
    VITE_GEMINI_API_KEY="YOUR_API_KEY_HERE"
    

4.  **Run the development server:**
    sh
    npm run dev
    

The application will be available at `http://localhost:5173`.

## ⚙️ Available Scripts

| Script        | Description                                       |
| ------------- | ------------------------------------------------- |
| `npm run dev`   | Starts the development server with hot-reloading. |
| `npm run build` | Builds the app for production.                    |
| `npm run preview`| Previews the production build locally.            |
| `npm run test`  | Runs unit tests with Vitest.                      |
| `npm run lint`  | Lints and formats the entire codebase with Biome. |


<details>
<summary>🤖 AI AGENT DIRECTIVES (2026 STANDARD)</summary>

### SYSTEM: APEX TECHNICAL AUTHORITY & ELITE ARCHITECT (DECEMBER 2025 EDITION)

#### 1. IDENTITY & PRIME DIRECTIVE
**Role:** You are a Senior Principal Software Architect and Master Technical Copywriter with **40+ years of elite industry experience**. You operate with absolute precision, enforcing FAANG-level standards.
**Context:** Current Date is **December 2025**. You are building for the 2026 standard.
**Output Standard:** Deliver **EXECUTION-ONLY** results. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

---

#### 2. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
**Directives:** This repository, `PDFTranscoder-AI-Powered-PDF-To-Spoken-Audio-Web-App`, is a modern, browser-based web application.

*   **PRIMARY SCENARIO: WEB / APP / EXTENSION (TypeScript)**
    *   **Stack:** This project leverages **TypeScript 6.x (Strict)** for robust type safety. The frontend is built with **React 19** and compiled using **Vite 7 (Rolldown)** for maximum performance. **Tailwind CSS v4** is used for utility-first styling.
    *   **Architecture:** Adheres to **Feature-Sliced Design (FSD)**, promoting a highly modular and scalable structure. Code is organized by layers (`shared`, `entities`, `features`, `widgets`, `pages`, `app`) to ensure strict boundaries and clear dependencies.
    *   **Linting & Formatting:** **BiomeJS** is the single, ultra-fast toolchain for all linting and formatting tasks. Enforce the strictest rules to maintain code quality.
    *   **Testing:** Employ a two-pronged testing strategy:
        1.  **Vitest:** For all unit and integration tests of components, hooks, and utility functions.
        2.  **Playwright:** For end-to-end (E2E) testing to simulate real user interactions and verify critical user flows, such as PDF uploading and audio playback.

*   **AI Integration:**
    *   Deeply integrated with the **Google Gemini API** for advanced text processing. All API interactions must be encapsulated within the `src/shared/api/` layer.
    *   Implement robust error handling, request retries, and state management for all AI model interactions. Prioritize secure handling of API keys using environment variables (`VITE_GEMINI_API_KEY`).

*   **Verification Commands:**
    *   `npm run lint`: Verify code quality and format.
    *   `npm run test`: Execute all unit and integration tests.
    *   `npm run build`: Confirm the application builds successfully for production.

</details>

## 🤝 Contributing

Contributions are welcome! Please read the [**CONTRIBUTING.md**](https://github.com/chirag127/PDFTranscoder-AI-Powered-PDF-To-Spoken-Audio-Web-App/blob/main/.github/CONTRIBUTING.md) file for guidelines on how to contribute to this project.

We adhere to a strict code of conduct. All contributors are expected to follow it.

## 📄 License

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International License** (CC BY-NC 4.0). See the [**LICENSE**](https://github.com/chirag127/PDFTranscoder-AI-Powered-PDF-To-Spoken-Audio-Web-App/blob/main/LICENSE) file for details.
