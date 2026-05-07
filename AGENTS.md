# AGENTS.md

- No build tooling, package manager, or `package.json` – skip `npm`/`yarn` commands
- No test, lint, typecheck, or formatter tooling configured
- Core source files: `index.html`, `style.css`
- Git: remote `https://github.com/barwin43/webcv.git`, default branch `master`
  - Push to `master` triggers GitHub Pages deployment
  - Commit style: short imperative (e.g., "Add X"), no conventional prefixes
- OpenCode config: `opencode.json` (sets `permission: "ask"`)
Commit only when explicitly requested by the user
- Commit messages: concise, present tense, describe the exact change (e.g., "Update name to Jorge Miralles")
- Never force push to main; warn user if requested
- Push to remote only when explicitly asked

- Commit Types:
Type     Purpose
feat     New feature
fix     Bug fix
docs     Documentation only
style     Formatting/style (no logic)
refactor     Code refactor (no feature/fix)
perf     Performance improvement
test     Add/update tests
build     Build system/dependencies
ci     CI/config changes
chore     Maintenance/misc
revert     Revert commit
- Generate Commit Message
    Type: What kind of change is this?
    Scope: What area/module is affected?
    Description: One-line summary of what changed (present tense, imperative mood, <72 chars)

- Execute Commit

# Single line
git commit -m "<type>[scope]: <description>"
git commit -e  "<feat>[languaje]: <add español basic lenguaje>
