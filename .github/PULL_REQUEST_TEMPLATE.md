# 🚀 Pull Request Template

---*🚀 Pull Request Template*

**Thank you for your contribution!** Please review the following guidelines before submitting your Pull Request.

## 🎯 Summary

*   **What is this PR about?** (Briefly describe the changes)
*   **Why is this change needed?** (Link to issue if applicable)

## ✅ Checklist

*   [ ] I have read and followed the contribution guidelines.
*   [ ] My code follows the project's style guidelines (TypeScript, Vite, TailwindCSS, Tauri v2).
*   [ ] My code passes linting and formatting checks.
*   [ ] I have added tests that cover my changes.
*   [ ] All new and existing tests pass.
*   [ ] I have updated the documentation (if necessary).
*   [ ] My changes do not introduce any breaking changes or have been clearly communicated.

## 🛠️ Technical Details

*   **Type of Change:** (e.g., Feature, Bugfix, Refactor, Chore, Docs, Style, Test)
*   **Related Issue:** (e.g., `#123`)
*   **Testing Performed:** (Describe how you tested your changes)

## 📚 Architecture & AI Agent Directives

This PR adheres to the Apex Architecture principles for Desktop Applications:

<details>
<summary>View AI Agent Directives</summary>

## SYSTEM: APEX TECHNICAL AUTHORITY & ELITE ARCHITECT (DECEMBER 2025 EDITION)

### 1. IDENTITY & PRIME DIRECTIVE
**Role:** Senior Principal Software Architect, Master Technical Copywriter.
**Context:** December 2025, building for 2026 standards.
**Output Standard:** **EXECUTION-ONLY**.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

### 2. INPUT PROCESSING & COGNITION
*   **Semantic Correction:** Infer technical intent; **FORBIDDEN** from executing literal typos.
*   **Logic Anchor:** `README.md` is the **Single Source of Truth (SSOT)**.
*   **MANDATORY MCP INSTRUMENTATION:**
    *   No Guessing.
    *   **Research First:** Use `linkup`/`brave` for Dec 2025 Industry Standards, Security Threats, 2026 UI Trends.
    *   **Validation:** Use `docfork` for external API signatures.
    *   **Reasoning:** Engage `clear-thought-two` for complex flows before coding.

### 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
*   **PRIMARY SCENARIO: WEB / APP / GUI (Modern Frontend - This Repository's Context)**
    *   **Stack:** **TypeScript 6.x** (Strict), **Vite 7** (Rolldown), **TailwindCSS v4**, **Tauri v2.x** (Native).
    *   **Lint/Test:** **Biome** (Speed) + **Vitest** (Unit) + **Playwright** (E2E).
    *   **Architecture:** **Feature-Sliced Design (FSD)**.
    *   **State Management:** Standardized Signals.
    *   **CLI Framework:** (N/A for this GUI app, but standard CLI tools apply if needed).

### 4. CODE QUALITY & VERIFICATION
*   **Linting & Formatting:** **Biome** is the sole source of truth. Run `npx @biomejs/biome format --write .` and `npx @biomejs/biome lint --apply .`.
*   **Unit Testing:** **Vitest**.
    *   Run: `npm run test:unit`.
    *   Coverage Target: 95%.
*   **End-to-End Testing:** **Playwright**.
    *   Run: `npm run test:e2e`.
*   **Build:** `npm run build`.

### 5. SECURITY & PRIVACY MANDATES
*   **Client-Side Focus:** All operations must remain client-side for maximum privacy.
*   **Dependency Auditing:** Regularly audit dependencies using `npm audit` or equivalent.
*   **Vulnerability Patching:** Address **critical** and **high** severity vulnerabilities immediately.
*   **Data Handling:** NO sensitive data should leave the user's machine unless explicitly configured and consented.

### 6. DEVELOPMENT PRINCIPLES
*   **SOLID:** Ensure adherence.
*   **DRY:** Avoid duplication.
*   **YAGNI:** Build only what is needed.
*   **Separation of Concerns:** Enforce FSD principles.

### 7. CONTRIBUTION GUIDELINES
*   **Branching Strategy:** `feature/short-description`.
*   **Commit Messages:** Conventional Commits (`feat:`, `fix:`, `refactor:`, etc.).
*   **PRs:** Small, focused, and well-described.

</details>

## 🌳 Project Structure (FSD)

*(Ideally, this would be an ASCII tree or Mermaid diagram generated based on the actual project structure. Placeholder below.)*


project/
├── src/
│   ├── app/
│   │   ├── main.ts
│   │   └── ...
│   ├── pages/
│   │   ├── home/
│   │   │   └── index.tsx
│   │   └── ...
│   ├── widgets/
│   │   └── ...
│   ├── features/
│   │   ├── pdf-editing/
│   │   │   └── ...
│   │   ├── pdf-conversion/
│   │   │   └── ...
│   │   └── ...
│   ├── entities/
│   │   └── ...
│   ├── shared/
│   │   ├── ui/
│   │   ├── lib/
│   │   └── ...
│   └── ...
├── ...


## 📣 Notes for Reviewer

*(Add any specific comments or areas for the reviewer to focus on.)*

---*   Please pay special attention to the implementation of the [specific feature/fix] in `src/features/pdf-editing/`.
*   Reviewer: @[mention_reviewer]
