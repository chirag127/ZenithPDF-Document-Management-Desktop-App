<div align="center">

# 🌟 ZenithPDF: Client-Side Document Management Desktop App

_High-Performance, Privacy-First PDF Toolkit Built with Rust and Tauri_

</div>

<div align="center">

[![CI Build Status](https://img.shields.io/github/actions/workflow/status/chirag127/ZenithPDF-Client-Side-Document-Management-Desktop-App/ci.yml?branch=main&label=CI%20Build&style=flat-square)](https://github.com/chirag127/ZenithPDF-Client-Side-Document-Management-Desktop-App/actions/workflows/ci.yml)
[![License: CC BY-NC 4.0](https://img.shields.io/github/license/chirag127/ZenithPDF-Client-Side-Document-Management-Desktop-App?style=flat-square&color=blue)](https://github.com/chirag127/ZenithPDF-Client-Side-Document-Management-Desktop-App/blob/main/LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/chirag127/ZenithPDF-Client-Side-Document-Management-Desktop-App?style=flat-square&color=yellow)](https://github.com/chirag127/ZenithPDF-Client-Side-Document-Management-Desktop-App/stargazers)
[![Framework: Tauri v2](https://img.shields.io/badge/Framework-Tauri%20v2-4c1e4c?style=flat-square&logo=tauri)](https://tauri.app/)
[![Core: Rust](https://img.shields.io/badge/Core-Rust-DEA584?style=flat-square&logo=rust)](https://www.rust-lang.org/)
[![Frontend: Vite/TS](https://img.shields.io/badge/Frontend-Vite%2FTS-646CFF?style=flat-square&logo=vite)](https://vitejs.dev/)
[![Linter: Biome & Clippy](https://img.shields.io/badge/Linter-Biome%20%26%20Clippy-00B2A9?style=flat-square&logo=biome)](https://biomejs.dev/)

<p align="center">
  <a href="https://github.com/chirag127/ZenithPDF-Client-Side-Document-Management-Desktop-App/stargazers">⭐ Star this Repo</a>
</p>

</div>

---

## 📝 Project Summary (BLUF)

**ZenithPDF** is a robust, cross-platform desktop application designed for comprehensive PDF management, utilizing the high performance and security offered by **Rust and Tauri**. It provides essential client-side tooling—including merging, splitting, conversion, and encryption—ensuring that sensitive document data never leaves the user's local machine.

This architecture guarantees privacy and speed, making ZenithPDF the ideal choice for professional document workflows requiring absolute data sovereignty.

## 🚀 Features at a Glance

*   **Privacy-First:** All processing is done locally via the high-speed Rust backend; zero cloud dependency.
*   **PDF Manipulation:** Merge multiple PDFs, split documents by page range, and rearrange pages effortlessly.
*   **Encryption & Security:** Apply strong password protection and digital signatures to secure sensitive files.
*   **Conversion Suite:** Convert PDFs to images (PNG, JPEG) and vice-versa, leveraging efficient Rust libraries.
*   **Cross-Platform:** Deployable on Windows, macOS, and Linux thanks to the Tauri framework.
*   **Modern UI/UX:** Built with TypeScript, Vite, and TailwindCSS for a responsive and intuitive interface.

## 🏛️ Architecture & Structure

ZenithPDF employs a hybrid architectural approach, separating the UI layer from the performance-critical core logic using Tauri's native bridge.

### Core Architecture Flow (Mermaid)

mermaid
graph TD
    A[User Interaction] --> B(Tauri Frontend: TS/Vite/Tailwind);
    B --> C{Tauri IPC Bridge};
    C --> D[Rust Core (Hexagonal Architecture)];
    D --> E(PDF Processing Adapters: PDFium/QPDF);
    E --> F[Local Filesystem I/O];
    D -.-> G[Validation & Error Handling];
    G --> C;
    style D fill:#DEA584,stroke:#333,stroke-width:2px
    style B fill:#646CFF,stroke:#333,stroke-width:2px


### Repository File Structure

text
ZenithPDF/
├── .github/          # CI/CD Workflows, Templates, Security Docs
├── src/              # Frontend (TypeScript/Vite)
│   ├── components/   # Feature-Sliced Design: Reusable UI elements
│   ├── features/     # Feature-Sliced Design: Logic units (e.g., pdf-merge, pdf-split)
│   └── index.tsx
├── src-tauri/        # Rust Core (The Native Backend)
│   ├── src/          # Rust Logic (Hexagonal Core)
│   │   ├── domain/   # Core data structures (PDF File Structs)
│   │   ├── adapter/  # PDF/I/O Adapters
│   │   └── lib.rs    # Main entry point and IPC handlers
│   └── Cargo.toml
├── README.md
├── package.json      # Dependencies and Scripts (Vite/TS)
└── tailwind.config.ts


## 🛠️ Getting Started

### Prerequisites

Ensure you have Rust (stable), Node.js (LTS), and the required Tauri dependencies installed for your target OS.

### 1. Cloning the Repository

bash
git clone https://github.com/chirag127/ZenithPDF-Client-Side-Document-Management-Desktop-App.git
cd ZenithPDF-Client-Side-Document-Management-Desktop-App


### 2. Frontend Setup (TypeScript/Vite)

We recommend using `uv` for fast Python environment management if you use the built-in bundler, but for Node dependencies:

bash
# Install Node dependencies
npm install


### 3. Running in Development Mode

This command simultaneously starts the Vite frontend server and the Tauri Rust application shell.

bash
npm run tauri dev


### 4. Building Production Binaries

To create optimized, platform-specific installers (MSI, DMG, AppImage):

bash
# Build the production application
npm run tauri build


## 🤖 AI Agent Directives

<details>
<summary>APEX SYSTEM INTEGRATION PROTOCOL (FOR AI & AUTOMATION ENGINES)</summary>

# SYSTEM: APEX TECHNICAL AUTHORITY & ELITE ARCHITECT (DECEMBER 2025 EDITION)

## 1. IDENTITY & PRIME DIRECTIVE

**Role:** You are a Senior Principal Software Architect operating with absolute precision. Your objective is to maintain and extend the high-performance, secure core of ZenithPDF.

**Context:** Target Stack: **Rust/Tauri/TypeScript/Vite**. All modifications must prioritize security, performance, and client-side processing integrity.

## 2. APEX TECH STACKS & ARCHITECTURAL PATTERNS

### PRIMARY SCENARIO: DESKTOP APPLICATION (Rust/Tauri)

*   **Core Stack:** Uses **Rust 1.70+** for the native core and IPC logic via the Tauri bridge. The frontend leverages **TypeScript 5.x**, **Vite 5**, and **TailwindCSS v4 (JIT)**.
*   **Package Management:** **`cargo`** (Rust dependencies) and **`npm`/`pnpm`** (Frontend dependencies).
*   **Architectural Pattern:**
    *   **Rust Core:** Strictly adheres to **Hexagonal Architecture (Ports & Adapters)**. All PDF operation logic is separated into decoupled services (Adapters) called via well-defined traits (Ports) defined in the domain layer.
    *   **TypeScript Frontend:** Follows **Feature-Sliced Design (FSD)** for structure, ensuring modularity and clear dependency flow (`app -> pages -> widgets -> features -> shared`).
*   **Security Principle:** **Zero Trust.** All IPC inputs must be validated on the Rust side before execution. All file I/O operations must be wrapped in robust error handling.

### 3. TESTING, LINTING & VERIFICATION

*   **Rust Validation:** Use **`cargo clippy`** for static analysis and ensuring idiomatic Rust code.
*   **Frontend Validation:** Use **`biome check --apply`** for ultra-fast TypeScript formatting and linting.
*   **Testing Frameworks:**
    *   **Rust Unit/Integration:** Standard `cargo test` framework.
    *   **TypeScript Unit:** **Vitest** for frontend component logic.
    *   **E2E/Desktop:** **Tauri Test Runner** (based on Playwright) for verifying native desktop functionalities.

*   **Verification Commands (Required before PR Submission):**
    bash
    # Frontend check
    npm run lint
    npm run test:unit

    # Rust core check
    cargo clippy -- -D warnings
    cargo test
    

</details>

## 🤝 Contribution Guidelines

We welcome high-quality contributions! Please review the documents in the `.github` directory before submitting issues or pull requests.

*   [Contributing Guide](https://github.com/chirag127/ZenithPDF-Client-Side-Document-Management-Desktop-App/blob/main/.github/CONTRIBUTING.md)
*   [Code of Conduct](https://github.com/chirag127/ZenithPDF-Client-Side-Document-Management-Desktop-App/blob/main/.github/CODE_OF_CONDUCT.md)

## 📄 License

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)** License. See the [LICENSE](https://github.com/chirag127/ZenithPDF-Client-Side-Document-Management-Desktop-App/blob/main/LICENSE) file for details.