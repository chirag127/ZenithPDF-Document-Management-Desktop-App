# 🤝 Contributing to ZenithPDF-Document-Management-Desktop-App

Thank you for considering contributing to ZenithPDF! We welcome contributions of all kinds, from bug reports and feature requests to code contributions and documentation improvements.

## 1. Our Development Standards

This project adheres to the **Apex Technical Authority Standards**, emphasizing **Zero-Defect, High-Velocity, Future-Proof** development.

*   **Technology Stack:** TypeScript, Vite, Tauri (Late 2025 Standards)
*   **Linting & Formatting:** Biome
*   **Testing:** Vitest (Unit), Playwright (E2E)
*   **Architecture:** Feature-Sliced Design (FSD)
*   **Code Quality:** SOLID, DRY, YAGNI principles are paramount.
*   **Version Control:** Gitflow workflow is recommended for feature development.

## 2. Getting Started

1.  **Fork the Repository:** Create your own fork of the `chirag127/ZenithPDF-Document-Management-Desktop-App` repository.
2.  **Clone Your Fork:** Clone your forked repository to your local machine:
    bash
    git clone https://github.com/chirag127/ZenithPDF-Document-Management-Desktop-App.git
    cd ZenithPDF-Document-Management-Desktop-App
    
3.  **Set Upstream Remote:** Add the original repository as an upstream remote to keep your fork updated:
    bash
    git remote add upstream https://github.com/chirag127/ZenithPDF-Document-Management-Desktop-App.git
    
4.  **Install Dependencies:** Install project dependencies using Vite:
    bash
    npm install
    
5.  **Run in Development Mode:** Start the application with hot-reloading:
    bash
    npm run dev
    

## 3. Contribution Workflow

We follow a standard Git workflow:

1.  **Create a New Branch:** For every new feature or bug fix, create a descriptive branch from the `main` branch:
    bash
    git checkout -b feature/your-feature-name
    # or
    git checkout -b fix/your-bug-description
    
2.  **Make Your Changes:** Write your code, ensuring it adheres to project standards and includes relevant tests.
3.  **Test Your Changes:** Run the test suite locally:
    bash
    npm run test # For unit tests
    npm run test:e2e # For end-to-end tests
    
4.  **Lint and Format:** Ensure your code is clean and well-formatted:
    bash
    npm run lint
    npm run format
    
5.  **Commit Your Changes:** Commit your changes with clear and concise messages. Use conventional commits if possible.
    bash
    git add .
    git commit -m "feat: Add user authentication module"
    
6.  **Push Your Branch:** Push your branch to your fork:
    bash
    git push origin HEAD
    
7.  **Open a Pull Request (PR):** Open a Pull Request from your branch to the `main` branch of the `chirag127/ZenithPDF-Document-Management-Desktop-App` repository.
    *   **PR Template:** Please fill out the Pull Request template completely.
    *   **CI/CD:** Ensure all GitHub Actions checks pass.

## 4. Pull Request Guidelines

*   **One Feature/Fix Per PR:** Keep PRs focused on a single logical change.
*   **Descriptive Title & Body:** Clearly explain *what* your PR does and *why*.
*   **Link Issues:** Reference any related issues using keywords like `Fixes #123` or `Closes #456`.
*   **Code Reviews:** Be prepared to discuss your changes and address feedback from reviewers.

## 5. Issue Reporting

When reporting an issue:

*   **Use the Issue Template:** File a bug report using the provided issue template (`.github/ISSUE_TEMPLATE/bug_report.md`).
*   **Be Specific:** Provide clear, concise details about the problem, including steps to reproduce it.
*   **Environment Details:** Include your OS, Node.js version, and any other relevant information.
*   **Screenshots/GIFs:** If applicable, attach visual evidence.

## 6. Code of Conduct

This project adheres to a Code of Conduct. By participating, you are expected to uphold this Code. Please refer to the [CODE_OF_CONDUCT.md](https://github.com/chirag127/ZenithPDF-Document-Management-Desktop-App/blob/main/CODE_OF_CONDUCT.md) file for details.

## 7. Questions & Support

If you have any questions, please open an issue or reach out on the project's discussion forum (if available).

We appreciate your contributions!
