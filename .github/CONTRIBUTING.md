# Contributing to ZenithPDF-Desktop-Document-Manager-Tauri-App

We welcome contributions to ZenithPDF-Desktop-Document-Manager-Tauri-App! As per Apex Technical Authority standards, we maintain a high bar for code quality, architectural integrity, and contribution clarity. Please adhere to the following guidelines.

## 1. Code of Conduct

This project adheres to the Contributor Covenant Code of Conduct. For more details, please see the `CODE_OF_CONDUCT.md` file. By participating, you are expected to uphold this code.

## 2. Getting Started

Before you contribute, please ensure you have the following installed:

*   **Node.js:** Version 18 or higher.
*   **npm/yarn/pnpm:** Your preferred package manager.
*   **Rust:** For Tauri development (Rustup recommended).
*   **Tauri CLI:** `cargo install tauri-cli`.

Clone the repository:

bash
git clone https://github.com/chirag127/ZenithPDF-Desktop-Document-Manager-Tauri-App.git
cd ZenithPDF-Desktop-Document-Manager-Tauri-App


Install dependencies:

bash
npm install
# or yarn install, or pnpm install


## 3. Development Workflow

1.  **Fork the Repository:** Create your own fork of the `chirag127/ZenithPDF-Desktop-Document-Manager-Tauri-App` repository.
2.  **Create a New Branch:** Make your changes on a descriptive branch (e.g., `feat/add-ocr-support`, `fix/incorrect-text-extraction`).
    bash
    git checkout -b my-feature-branch
    
3.  **Make Your Changes:** Implement your feature or fix. Ensure your code adheres to the project's architectural principles (e.g., adhering to the TypeScript best practices, Vite configuration, Tauri guidelines).
4.  **Test Your Changes:** Run the test suite to ensure your changes haven't introduced regressions.
    bash
    # Run linters and formatters
    npm run lint
    npm run format

    # Run unit tests
      # (Example: Assuming Vitest is configured)
    npm run test:unit

    # Run E2E tests if applicable
      # (Example: Assuming Playwright is configured)
    npm run test:e2e
    
5.  **Commit Your Changes:** Write clear, concise commit messages. Follow conventional commits if possible.
    bash
    git commit -m "feat: Add new PDF merging functionality"
    
6.  **Push to Your Fork:** Push your branch to your fork.
    bash
    git push origin my-feature-branch
    
7.  **Submit a Pull Request:** Open a Pull Request from your feature branch to the `main` branch of the `chirag127/ZenithPDF-Desktop-Document-Manager-Tauri-App` repository.

## 4. Architectural Principles

*   **TypeScript (Strict Mode):** All TypeScript code must be written with strict type checking enabled. Aim for predictable, maintainable code.
*   **Vite:** Leverage Vite's performance benefits for development and build processes.
*   **Tauri v2:** Follow Tauri's best practices for building secure and performant desktop applications. Understand the security implications of client-side operations.
*   **Feature-Sliced Design (FSD) / Modular Architecture:** Organize code into features, layers, and slices for scalability and maintainability. Refer to the project's `tree` diagram in the `README.md` for current structure.
*   **SOLID Principles:** Adhere to SOLID principles in your code design.
*   **DRY (Don't Repeat Yourself):** Avoid code duplication.
*   **YAGNI (You Ain't Gonna Need It):** Focus on current requirements; avoid over-engineering for future, unconfirmed needs.

## 5. Testing

*   **Unit Tests:** Write comprehensive unit tests for components, utilities, and business logic using Vitest.
*   **End-to-End (E2E) Tests:** If applicable, write E2E tests using Playwright to simulate user interactions and validate critical workflows.
*   **Coverage:** Aim for high code coverage. Ensure critical paths are well-tested.

## 6. Pull Request Guidelines

*   **Single Responsibility:** Each PR should ideally address one specific issue or feature.
*   **Clear Description:** Provide a detailed description of your changes, including the problem solved and the approach taken.
*   **Link to Issue:** If your PR addresses an existing issue, please link to it (e.g., `Closes #123`).
*   **CI/CD Checks:** Ensure all automated checks (linting, testing, building) pass before submitting your PR.

## 7. Reporting Issues

When reporting an issue, please provide:

*   **Clear Title:** A concise summary of the problem.
*   **Environment Details:** Operating System, Tauri version, Node.js version.
*   **Steps to Reproduce:** Detailed, step-by-step instructions to trigger the bug.
*   **Expected vs. Actual Behavior:** What you expected to happen and what actually happened.
*   **Screenshots/Logs:** Attach any relevant visual aids or console logs.

## 8. Architectural Decisions & AI Agent Directives

Future contributions will be evaluated against the directives outlined in the `AGENTS.md` file. This ensures alignment with the project's strategic goals and technical vision. Adherence to these directives is mandatory for all contributions.

Thank you for contributing to ZenithPDF!
