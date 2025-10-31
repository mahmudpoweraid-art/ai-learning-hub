## Repository: ai-learning-hub — Copilot instructions

This file gives concise, actionable guidance to AI coding assistants (Copilot/agents) working on the ai-learning-hub repository.

Context summary
- Minimal repository currently: top-level `README.md` only. No source code, tests or CI detected.
- The project appears to be an "AI based learning app" (per README). No language, framework, or build files are present.

How to be immediately productive
- Look for or create a project scaffold before making feature changes. Recommended initial files to add when expanding the repo:
  - `package.json` (for Node/React), `requirements.txt` or `pyproject.toml` (for Python), or equivalent for other ecosystems
  - `src/` directory with a clear entrypoint (e.g., `src/index.js` or `src/main.py`)
  - `README.md` updates with setup and run instructions
- When guessing a language/framework, prefer asking the user for clarification. If the user doesn't respond, make minimal scaffold changes and explain assumptions in the PR description.

Project-specific patterns and conventions
- Keep changes minimal and explicit. This repo currently lacks conventions; document any conventions you introduce in `README.md` and add a short `CONTRIBUTING.md`.
- Use clear, small commits. Each PR should include: (1) purpose, (2) files changed, (3) how to run locally.

Examples and templates
- If creating a simple Node.js scaffold, include:
  - `package.json` with `start` and `test` scripts
  - `src/app.js` or `src/index.js` with a minimal HTTP server
  - `README.md` instructions to run `npm install` and `npm start`
- If creating a Python scaffold, include:
  - `pyproject.toml` or `requirements.txt`
  - `src/__main__.py` or `src/app.py` and a small `README.md` run example

Integration points & external dependencies
- No external integrations are present in the repository now. If you add third-party services (OpenAI, AWS, Firebase, etc.), add a clear `env.example` and document environment variables in `README.md`.

Debugging and tests
- No tests detected — if you add tests, pick a common test runner for the ecosystem (Jest for JS, pytest for Python) and add a `test` script.

When writing code changes or PRs
- Describe assumptions in the PR body; include how to run and verify changes locally.
- Prefer small, incremental PRs that add one thing at a time (scaffold -> feature -> tests -> docs).

Files to reference when present
- `README.md`: project description and runnable examples
- `package.json`, `pyproject.toml`, `requirements.txt`: dependency and run scripts
- `src/`: implementation code and entrypoints
- `CONTRIBUTING.md`: contribution rules and coding conventions

If you are unsure what to do next
- Ask the repo owner or maintainer for the intended language and target platform.
- Propose a minimal scaffold PR with clear assumptions documented.

Quick checklist for PRs created by AI agents
- Include a short description of assumptions.
- Include setup/run instructions in `README.md`.
- Add at least one basic smoke test (unit or script) demonstrating the feature works.

Feedback
- After creating or updating files, ask the maintainer whether the chosen language/scaffold is correct before broad changes.
