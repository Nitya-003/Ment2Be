# Contributing to Ment2Be

First off, thank you for considering contributing to **Ment2Be**! It’s people like you who make this platform a better place for mentors and learners alike.

As part of **ECWOC 2026**, we want to ensure a smooth and collaborative experience for everyone. Please follow these guidelines to get started.

---

## Quick Start: Development Workflow

We follow the standard **GitHub Flow**:

1.  **Fork** the repository to your own GitHub account.
2.  **Clone** your fork locally:
    ```bash
    git clone [https://github.com/YOUR_USERNAME/Ment2Be.git](https://github.com/YOUR_USERNAME/Ment2Be.git)
    ```
3.  **Create a Branch** for your feature or fix:
    ```bash
    git checkout -b feat/your-feature-name
    # OR
    git checkout -b fix/your-bug-fix
    ```
4.  **Commit** your changes using descriptive messages (see [Commit Conventions](#-commit-conventions)).
5.  **Push** to your fork and open a **Pull Request** (PR) against the `main` branch of the original repo.

---

## Technical Setup & Dual-Backend Toggle

Ment2Be supports both **Node.js** and **Java** backends. To contribute effectively, you must configure your local environment correctly.

### 1. Environment Variables
Never commit your `.env` files. Ensure you have created:
* `Backend/.env` (Refer to `README.md` for required keys)
* `Frontend/.env.local` (Required for Vite)

### 2. Switching Backends
If you are testing a feature that relies on a specific backend, navigate to:
`Frontend/src/config/apiConfig.js`

```javascript
// Toggle between 'nodejs' or 'java'
const ACTIVE_BACKEND = 'nodejs';
```

Ensure you have the corresponding server running locally before testing.

---

## Coding Standards
To keep the codebase clean, please adhere to the following:
* **Frontend:** Use Tailwind CSS v3.4+ for styling. Follow the mobile-first responsive approach.
* **Components:** Use functional components with Hooks. Ensure components are modular and stored in src/components/.
* **Icons:** Use Lucide React for consistency.
* **State Management:** Use React Context for global state and standard `useState/useReducer` for local state.
* **Linting:** Run `npm run lint` in the `Frontend/` directory before committing.

---

## Commit Conventions
We use human-readable commit messages:
* `feat:` - A new feature.
* `fix:` - A bug fix.
* `docs:` - Documentation only changes.
* `style:` - Changes that do not affect the meaning of the code (white-space, formatting).
* `chore:` - Updating build tasks, package manager configs, etc.
_Example: `feat: add star rating system to mentor profile`_

---

## Pull Request Checklist
Before submitting your PR, ensure:
- [ ] Your code follows the project's style guidelines.
- [ ] You have performed a self-review of your code.
- [ ] You have commented on your code, particularly in hard-to-understand areas.
- [ ] **UI Changes:** You have attached screenshots or a screen recording of the changes.
- [ ] The PR title follows the commit convention.
- [ ] You have linked the issue your PR resolves (e.g., `Closes #12`).

---

## Community & Support
By contributing, you agree to abide by our [Code of Conduct](/Code_of_Conduct.md). If you have questions, feel free to reach out to the project maintainers or open a discussion in the "Issues" tab.

---

## _Happy Coding!_
