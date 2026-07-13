# CLAUDE.md

Project guidance for AI assistants working in this repository.

## Tech Stack

| Category | Tools |
|----------|-------|
| **Runtime** | Node.js |
| **Version Control** | Git |
| **Hosting & Collaboration** | GitHub |
| **AI Development Environment** | Cursor |

When adding dependencies or tooling, prefer widely adopted Node.js libraries and keep the stack aligned with what is documented in `README.md`.

## Coding Conventions

- Use **JavaScript** or **TypeScript** consistently within a module; do not mix styles arbitrarily.
- Prefer **ES modules** (`import` / `export`) unless the project is explicitly configured for CommonJS.
- Use **camelCase** for variables and functions, **PascalCase** for classes, and **UPPER_SNAKE_CASE** for constants.
- Name files by purpose: `kebab-case.js` for utilities, `PascalCase.js` for classes when appropriate.
- Keep functions small and focused on a single responsibility.
- Add comments only for non-obvious logic — code should be self-explanatory where possible.
- Match existing patterns in the codebase before introducing new abstractions.
- Do not commit secrets, API keys, or credentials. Use environment variables and `.env` files (never committed).

## Conventional Commits

All commit messages must follow the [Conventional Commits](https://www.conventionalcommits.org/) specification:

```
<type>(<optional scope>): <short description>

[optional body]

[optional footer]
```

**Common types:**

| Type | Use when |
|------|----------|
| `feat` | Adding a new feature |
| `fix` | Fixing a bug |
| `docs` | Documentation only |
| `style` | Formatting, no logic change |
| `refactor` | Code change that neither fixes a bug nor adds a feature |
| `test` | Adding or updating tests |
| `chore` | Maintenance, tooling, or dependency updates |

**Examples:**

```
feat(auth): add JWT token validation
fix(api): handle empty response from upstream service
docs: update setup instructions in README
chore: bump eslint to latest version
```

Keep the subject line under 72 characters, use imperative mood ("add" not "added"), and do not end with a period.

## Keep Code Clean and Modular

- **Minimize scope** — change only what is needed for the task; avoid unrelated edits.
- **Separate concerns** — split routing, business logic, data access, and utilities into distinct modules under `src/`.
- **Avoid duplication** — extract shared logic into reusable functions rather than copying code.
- **No over-engineering** — do not add abstractions, helpers, or error handling for hypothetical future needs.
- **Test meaningful behavior** — place tests in `tests/` and cover real logic, not trivial assertions.
- **Leave the codebase better** — if you touch a file, ensure it remains readable and consistent with surrounding code.

## Explain Changes Before Editing Files

Before making any file changes:

1. **State the goal** — briefly describe what the user asked for or what problem is being solved.
2. **Outline the plan** — list which files will be created or modified and why.
3. **Call out trade-offs** — mention any assumptions, risks, or alternative approaches when relevant.
4. **Confirm scope** — if the request is ambiguous, ask before making large or destructive changes.

After editing:

- Summarize what changed and where.
- Note anything the user should verify manually (e.g. running tests, setting env vars).

Do not silently refactor, rename, or reformat unrelated code without explaining the rationale first.
## Additional Coding Guidelines

- Keep functions small and modular.
- Use meaningful variable names.
- Write clear commit messages following Conventional Commits.
- Document important design decisions.
## Project Rules Learned (Foundation Workflow)

1. Always provide complete requirements before asking AI to generate code.
2. Verify AI-generated code manually before accepting it.
3. Include accessibility and edge-case handling as part of every implementation.
4. Keep project-specific rules documented for future development.