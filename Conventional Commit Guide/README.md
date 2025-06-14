# Conventional Commit Types Guide

This guide outlines the standardized commit message types used in this project to ensure clarity, consistency, and maintainability.

We follow the [Conventional Commits](https://www.conventionalcommits.org/) specification to help automate versioning, changelogs, and collaboration.

---

## 🚀 Commit Message Format

Each commit message should be structured as follows:

```bash
<type>: <short summary>
```

- Use the imperative mood (e.g., "add", not "added" or "adds").
- Keep the summary concise and relevant.
- Scope and body are optional but can be added for clarity.

---

## ✅ Commit Types

### 1. `feat` — New Feature

Used when adding new features or functionality.

**Example:**

```bash
feat: add user registration endpoint
```


---

### 2. `fix` — Bug Fix

Used for patches or bug fixes that correct unexpected behavior.

**Example:**

```bash
fix: correct typo in settings validation
```


---

### 3. `docs` — Documentation Changes

Used for modifying documentation only. No code changes.

**Example:**

```bash
docs: update README with setup instructions
```


---

### 4. `style` — Code Style Changes

Used for changes that don’t affect the logic or behavior, such as:

- Formatting
- White-space
- Indentation
- Semicolons

**Example:**

```bash
style: reformat code with Prettier
```


---

### 5. `refactor` — Code Refactoring

Used for internal changes that improve code quality or structure without altering behavior.

**Example:**

```bash
refactor: extract authentication logic into a separate service
```


---

### 6. `test` — Adding or Updating Tests

Used when adding, removing, or updating test files.

**Example:**

```bash
test: add unit tests for date parser
```


---

### 7. `chore` — Maintenance Tasks (Detailed)

Used for routine tasks and configurations that do **not** affect application functionality or logic.

#### 🔧 When to Use `chore`

- Updating dependencies:

```bash
chore: upgrade axios to v1.6.0
```

- Changing build scripts or tooling:

```bash
chore: update Vite config for faster builds
```

- Updating CI/CD pipelines:

```bash
chore: fix GitHub Actions deploy job
```

- Modifying linter or formatter settings:

```bash
chore: adjust ESLint rules for consistent spacing
```

- Editing project config files:

```bash
chore: add new fields to package.json
```

- Managing dev tools and environments:

```bash
chore: add .env.example to project
```


#### ⚠️ Don't Use `chore` For:

- Features → use `feat`
- Bug fixes → use `fix`
- Refactors → use `refactor`
- Tests → use `test`
- Documentation → use `docs`

---

## 🛠 Example Workflow

```bash
git commit -m "chore: configure Prettier and ESLint"
git commit -m "fix: handle null values in response parser"
git commit -m "feat: add password reset flow"
```


---

## 🔗 Resources

- [Conventional Commits](https://www.conventionalcommits.org/)
- [Semantic Versioning](https://semver.org/)
- [Commitizen CLI Tool](https://github.com/commitizen/cz-cli)

---

By following this guide, we improve:

- **Team collaboration**
- **Automated changelogs**
- **Version control discipline**

Happy committing! 🚀

---

