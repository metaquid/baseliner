# BASELINER

### The Code Modernization Ecosystem

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**BASELINER** is a self-contained, single-file web application that transforms the risky and subjective process of refactoring legacy code into a fast, objective, and standards-driven workflow. It's an integrated environment designed to guide developers through the entire modernization lifecycle: **Audit → Explore → Act**.

---

## What is BASELINER?

Every developer faces the challenge of modernizing old codebases. Technical debt, outdated patterns, and deprecated tags make projects hard to maintain. The core problem is uncertainty: *what is the "best practice" today?*

BASELINER solves this by connecting directly to the **Web Platform Baseline**, a live, data-driven source of truth maintained by Google, Mozilla, Microsoft, and others. It transforms refactoring from a subjective chore into a guided, objective, and collaborative process, ensuring your code aligns with current, stable web standards.

## The Workflow: Audit → Explore → Act

BASELINER is built around a powerful and intuitive workflow:

1.  **AUDIT (The 10,000-Foot View):** Start by running a high-level audit on an entire project folder. Baseliner scans your files for outdated patterns and generates a clear report on existing technical debt, giving you a data-driven starting point.

2.  **EXPLORE (Discover & Learn):** Grounded in live data from the `webstatus.dev` API, the "Explore Baseline" feature lets you discover modern alternatives to legacy code (e.g., finding that Flexbox and Grid are the modern successors to `float`). You can read up-to-date documentation and instantly create new, validated detection rules.

3.  **ACT (Precise Refactoring):** Take action with a powerful, dual-workflow approach:
    *   **Automated Workflow (`Apply Quick Fixes`):** For low-risk changes, this feature applies safe, automatic substitutions and shows a clear "Before/After" diff.
    *   **AI-Supervised Workflow (`Generate LLM Prompt`):** For complex issues requiring logic and context, Baseliner acts as an expert prompt engineer. It generates a highly specific prompt for an external LLM and provides an interface to compare, edit, and approve the AI's suggestions, keeping you in full control.

## Key Innovations

*   **Live Baseline Integration:** BASELINER's core innovation is its direct connection to the Web Platform Baseline. This ensures its recommendations are not based on static or opinionated rules, but on live, stable web standards, removing guesswork and building confidence.

*   **Hybrid Human-AI Workflow:** It uniquely combines automation for tedious tasks and AI-augmented supervision for complex ones. It automates the "what" and assists with the "how," keeping the developer in charge.

*   **Iterative Refinement Loop:** The "Continue with Result" feature enables a powerful, multi-pass workflow. You can apply automatic fixes, then use that cleaner code as the input for a more focused, AI-assisted refactoring session.

*   **Intelligent Rule Engine:** The entire system is powered by a fully customizable and transparent JSON rule engine. The editor provides live validation against the Baseline API, ensuring every rule is effective and standards-aligned.

## Getting Started

### 1. Live Demo (Recommended)

The easiest way to try BASELINER is through the live GitHub Pages demo:

**[▶️ Open the Live Application](https://metaquid.github.io/baseliner/)**

### 2. Running Locally

BASELINER is a single, self-contained HTML file. No build steps, no servers, no dependencies.

1.  Download the `baseliner-1.3.6.html` file from this repository.
2.  Open it in a modern web browser (like Chrome, Firefox, or Edge).
3.  That's it! The application is ready to use.

## Tech Stack

*   **Core:** Vanilla JavaScript (ES6+), HTML5, CSS3
*   **Data Source:** `webstatus.dev` API for live Web Platform Baseline data
*   **Diffing:** `diff.js` library for rendering the Before/After view

## Future Roadmap

BASELINER is a powerful foundation, and we have a clear vision for its future:

*   **IDE & CI/CD Integration:** Develop a **VS Code Extension** for in-editor use and a **GitHub Action** to run audits automatically on pull requests.
*   **AI-Powered Rule Creation:** Use AI to suggest regex patterns when creating new rules from the Baseline Explorer.
*   **Team-Based Rule Sets:** Allow teams to create, share, and version their own custom rule sets for project-wide consistency.
*   **Quantitative Modernization Metrics:** Evolve the audit report to provide a "Modernization Score," allowing teams to track their progress over time.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE.md) file for details.
