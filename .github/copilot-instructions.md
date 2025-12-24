<!-- Copilot instructions for example-477-student.github.io -->
# Copilot instructions

Purpose: Help an AI coding agent be immediately productive in this repository.

- **Repo type:** Minimal static GitHub Pages site (single-file site). Primary file: [index.html](index.html).
- **Goal:** Make small, safe edits to the static site; avoid adding heavy toolchains unless requested.

How this project is structured
- Single-page static HTML at [index.html](index.html). There is no build system, package.json, or tests in the repo.
- The repo name follows GitHub Pages pattern (example-477-student.github.io) — content in `main` publishes at `https://example-477-student.github.io/` when Pages is enabled.

Local developer workflow (what works here)
- Serve the site locally with a lightweight static server. Example (used in the dev environment):

```bash
npx http-server -p 8000
# then open http://localhost:8000
```

- No build step required for edits to `index.html` — modify and preview locally.

Project-specific conventions and patterns
- Keep changes small and focused: edits are typically content or small markup fixes inside `index.html`.
- Avoid introducing frameworks, bundlers, or test scaffolding without explicit approval from the repo owner.

Integration points and external dependencies
- There are no external service integrations or dependency manifests in the repo. If adding integrations (analytics, CI, pages config), mention them in the PR description.

Guidance for AI agents
- When editing content, update `index.html` directly and run the static server to verify layout.
- If a user asks to add a build system or tests, propose options (e.g., simple `package.json` + `http-server` or a GitHub Actions workflow) and wait for confirmation before implementing.
- For anything that touches infrastructure (Pages settings, workflows), ask the repo owner for permission.

Examples (explicit)
- Change the page title/heading: edit the `<h1>` in [index.html](index.html).
- Add a new file: create it at the repo root and reference it from `index.html`; do not add a complex routing system.

What not to do
- Do not scaffold React/Angular/Vite projects, add CI workflows, or change repository visibility without confirmation.

If unclear
- Ask these clarifying questions: "Should I keep this repository as a simple static site?", "May I add package tooling or CI?", "Do you want GitHub Pages configured automatically?"

Files to inspect before making changes
- [index.html](index.html)
- [README.md](README.md)

End of instructions.
