# PDFTranscoder-AI-Powered-PDF-To-Spoken-Audio-Web-App

A sophisticated browser-based web application designed to transform technical PDFs into natural, spoken-friendly audio using Google Gemini AI.

---

![Build Status](https://img.shields.io/github/actions/workflow/user/chirag127/PDFTranscoder-AI-Powered-PDF-To-Spoken-Audio-Web-App/ci.yml?style=flat-square&logo=githubactions)
![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/PDFTranscoder-AI-Powered-PDF-To-Spoken-Audio-Web-App?style=flat-square&logo=codecov)
![JavaScript](https://img.shields.io/badge/javascript-323330?style=flat-square&logo=javascript&logoColor=F7DF1E)
![Google Gemini](https://img.shields.io/badge/Google%20Gemini-4285F4?style=flat-square&logo=google-gemini&logoColor=white)
![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-blue.svg?style=flat-square)
![GitHub Stars](https://img.shields.io/github/stars/chirag127/PDFTranscoder-AI-Powered-PDF-To-Spoken-Audio-Web-App?style=flat-square&logo=github)

---

### ⭐ Star this Repo

Your stars fuel our innovation!

---

## Overview

PDFTranscoder is a cutting-edge web application that revolutionizes how users interact with technical documentation. It intelligently converts PDF documents into high-quality audio, leveraging the advanced capabilities of Google Gemini AI for enhanced text comprehension and natural speech synthesis. Designed for accessibility and efficiency, it aims to make complex information easily consumable through audio.

## Architecture

mermaid
graph TD
    A[User Interface (Browser)] --> B(Frontend Logic - JavaScript/Vite)
    B --> C{PDF Processing Module}
    C --> D(Text Extraction)
    D --> E(AI - Google Gemini API)
    E --> F(Text-to-Speech Synthesis)
    F --> G(Audio Output)
    B --> H(Backend API Gateway - Mocked/Placeholder for this Web App)
    H --> I(External Services - e.g., Cloud Storage, AI APIs)

    subgraph Core Functionality
        C
        D
        E
        F
        G
    end

    subgraph Deployment
        A
        B
    end

    style Core Functionality fill:#f9f,stroke:#333,stroke-width:2px


## Table of Contents

*   [Overview](#overview)
*   [Architecture](#architecture)
*   [Table of Contents](#table-of-contents)
*   [AI Agent Directives](#ai-agent-directives)
*   [Core Features](#core-features)
*   [Tech Stack](#tech-stack)
*   [Development Setup](#development-setup)
*   [Running the Application](#running-the-application)
*   [Testing](#testing)
*   [Contribution Guidelines](#contribution-guidelines)
*   [License](#license)
*   [Security](#security)

---

## AI Agent Directives

<details>
  <summary>View AI Agent Directives</summary>

### SYSTEM: APEX TECHNICAL AUTHORITY & ELITE ARCHITECT (DECEMBER 2025 EDITION)

#### 1. IDENTITY & PRIME DIRECTIVE
**Role:** You are a Senior Principal Software Architect and Master Technical Copywriter with **40+ years of elite industry experience**. You operate with absolute precision, enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable."
**Context:** Current Date is **December 2025**. You are building for the 2026 standard.
**Output Standard:** Deliver **EXECUTION-ONLY** results. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

#### 2. INPUT PROCESSING & COGNITION
*   **SPEECH-TO-TEXT INTERPRETATION PROTOCOL:**
    *   **Context:** User inputs may contain phonetic errors (homophones, typos).
    *   **Semantic Correction:** **STRICTLY FORBIDDEN** from executing literal typos. You must **INFER** technical intent based on the project context.
    *   **Logic Anchor:** Treat the `README.md` as the **Single Source of Truth (SSOT)**.
*   **MANDATORY MCP INSTRUMENTATION:**
    *   **No Guessing:** Do not hallucinate APIs.
    *   **Research First:** Use `linkup`/`brave` to search for **December 2025 Industry Standards**, **Security Threats**, and **2026 UI Trends**.
    *   **Validation:** Use `docfork` to verify *every* external API signature.
    *   **Reasoning:** Engage `clear-thought-two` to architect complex flows *before* writing code.

#### 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
**Directives:** Detect the project type and apply the corresponding **Apex Toolchain**.

*   **PRIMARY SCENARIO: WEB / APP / EXTENSION (TypeScript)**
    *   **Stack:** This project leverages **TypeScript 6.x** (Strict Mode enabled by default), **Vite 7** (with Rolldown Bundler for optimal performance), and potentially **Tauri v2.x** for desktop-like experiences or **WXT** for advanced browser extensions. State management adheres to **Signals** (as per latest ECMAScript standards).
    *   **Lint/Test:** **Biome** (for ultra-fast linting and formatting) and **Vitest** (for unit testing) are the standard. **Playwright** is used for end-to-end testing.
    *   **Architecture:** Feature-Sliced Design (FSD) is recommended for maintainability and scalability.
    *   **AI Integration:** For AI integrations, prioritize modularity and robust error handling. Use direct `fetch` calls or a lightweight SDK.

#### 4. CORE PRINCIPLES & MANDATES
*   **SOLID Principles:** Ensure adherence to Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, and Dependency Inversion.
*   **DRY (Don't Repeat Yourself):** Eliminate redundant code.
*   **YAGNI (You Aren't Gonna Need It):** Implement only necessary features.
*   **Progressive Enhancement:** Design for graceful degradation in older environments.
*   **Accessibility (WCAG 2.1 AA):** Ensure usability for all.
*   **Performance Optimization:** Target Lighthouse scores above 90.
*   **Security:** Proactive vulnerability scanning and secure coding practices are paramount. Regularly update dependencies.
*   **Documentation:** Maintain comprehensive, up-to-date documentation.

#### 5. VERIFICATION COMMANDS
*   **Linting & Formatting:** `npm run lint` or `npx @biomejs/biome check --apply .`
*   **Unit Tests:** `npm run test:unit` or `npx vitest run --passWithNoTests`
*   **E2E Tests:** `npm run test:e2e` or `npx playwright test`
*   **Build:** `npm run build`

#### 6. AGENTS.MD PROTOCOL
*   **Update Mandate:** The `AGENTS.md` file is a living document. Any agent's interaction must strive to update it for future consistency. 
*   **Structure:** Must contain **IDENTITY**, **INPUT PROCESSING**, **TECH STACKS**, **CORE PRINCIPLES**, and **VERIFICATION COMMANDS**.

</details>

---

## Core Features

*   **Intelligent PDF Parsing:** Extracts text and relevant information from various PDF formats.
*   **AI-Powered Content Analysis:** Utilizes Google Gemini to understand context, structure, and key points within the PDF.
*   **Natural Speech Synthesis:** Generates high-fidelity, natural-sounding audio.
*   **Customizable Audio Output:** Options for voice selection, speed, and pitch.
*   **User-Friendly Interface:** Intuitive browser-based experience.
*   **Cross-Browser Compatibility:** Works across modern web browsers.

---

## Tech Stack

*   **Language:** TypeScript
*   **Bundler/Framework:** Vite 7
*   **Styling:** TailwindCSS v4 (or equivalent CSS framework)
*   **AI Model:** Google Gemini API
*   **Speech Synthesis:** Web Speech API or Cloud-based TTS service
*   **Testing:** Vitest (Unit), Playwright (E2E)
*   **Linting/Formatting:** Biome
*   **Architecture:** Feature-Sliced Design (FSD) recommended

---

## Development Setup

1.  **Clone the Repository:**
    bash
    git clone https://github.com/chirag127/PDFTranscoder-AI-Powered-PDF-To-Spoken-Audio-Web-App.git
    cd PDFTranscoder-AI-Powered-PDF-To-Spoken-Audio-Web-App
    

2.  **Install Dependencies:**
    bash
    npm install
    

3.  **Environment Variables:**
    Create a `.env` file in the root directory and add your Google Gemini API key:
    env
    VITE_GEMINI_API_KEY=YOUR_GOOGLE_GEMINI_API_KEY
    

---

## Running the Application

*   **Development Server:**
    bash
    npm run dev
    
    This will start the Vite development server with hot module replacement.

*   **Build for Production:**
    bash
    npm run build
    
    This command bundles the application for production deployment.

---

## Testing

*   **Run Unit Tests:**
    bash
    npm run test:unit
    

*   **Run End-to-End Tests:**
    bash
    npm run test:e2e
    

---

## Contribution Guidelines

Contributions are welcome! Please refer to the [CONTRIBUTING.md](https://github.com/chirag127/PDFTranscoder-AI-Powered-PDF-To-Spoken-Audio-Web-App/blob/main/.github/CONTRIBUTING.md) file for detailed guidelines on how to contribute.

---

## License

This project is licensed under the Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0). See the [LICENSE](https://github.com/chirag127/PDFTranscoder-AI-Powered-PDF-To-Spoken-Audio-Web-App/blob/main/LICENSE) file for more details.

---

## Security

For security-related issues, please refer to the [SECURITY.md](https://github.com/chirag127/PDFTranscoder-AI-Powered-PDF-To-Spoken-Audio-Web-App/blob/main/.github/SECURITY.md) file.
