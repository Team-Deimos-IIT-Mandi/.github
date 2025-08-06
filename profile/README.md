# Contributing Guidelines

This guide outlines how we expect all contributors — across all domains (software, mechanical, electrical, simulation, etc.) — to work in a clean, organized, and trackable manner.

---

## 🔁 Git & Workflow Policy

### 🔸 Issue-Driven Development

All changes (features, bug fixes, updates) **must start with an assigned GitHub Issue**.

- **No direct commits** without a corresponding issue.
- Open a GitHub issue **before** starting development and get it assigned to yourself.
- Link the issue to the relevant **Notion task** if applicable.
- All **PRs must reference the issue number** they are solving using GitHub’s linking syntax (e.g., `Fixes #12`).

### 🔸 Branch Naming Convention

Branches must be named using the following format:
```

issue-<issue-number>-<short-description>

```

Examples:
- `issue-42-fix-imu-reading`
- `issue-13-add-path-tracking`
- `issue-101-update-cad-gearbox`

Each PR should:
- Be from one of the above branches.
- Reference the issue it's addressing.
- Be clearly descriptive in its title and body.

### 🔸 Pull Requests (PRs)

- All code or design contributions must go through a **Pull Request to `main` or `master`**.
- No direct commits are allowed on `main`/`master`.
- PR titles and descriptions should clearly state:
  - What the change is doing
  - What issue it addresses
  - Any dependencies or related PRs
  - A short video demo (if applicable)

If multiple PRs address the same issue (for example, different subtasks):
- All of them must reference the **same issue**.
- Link all relevant branches and PRs **within the issue thread**.

---

## 🧠 Task Linking & Traceability

- All **GitHub issues must be linked** to their **corresponding task on Notion**.
- For each GitHub **PR**, add the **PR number and link** in the Notion task.
- This ensures complete traceability across GitHub and Notion for all technical work.

---

## 🎥 Documentation with Videos

For **any contribution** involving domain-specific results, include a **video demo**. Examples include:
- ✅ Mechanical: CAD assembly animation, FEA result walkthrough
- ✅ Electrical: Simulation or schematic demo
- ✅ Software: Terminal demo, UI recording, simulation walkthrough

Attach this video directly in the PR or provide a link to an accessible location.

---

## 📁 Repository Requirements

Each repository **must include and maintain** the following:

### 1. `README.md`
A good `README.md` should contain:
- Project overview
- Architecture diagrams (if applicable)
- Setup and installation instructions
- How to contribute
- Dependencies
- Video demos
- License (if any)

### 2. Clean Folder Structure

Example:
```

.
├── README.md
├── src/
├── hardware/
├── simulations/
├── docs/
├── videos/
└── .github/

```

---

## ✅ Best Practices

- Use meaningful commit messages.
- Do not upload irrelevant or large binary files unless required.
- Keep branches small and focused.
- Rebase or squash commits before merging to `main` if needed.
- Clean up stale branches after merging.

---

## 🔐 Responsibility and Maturity

Branch protection is **not enforced by default**. We trust contributors to:
- Never commit directly to `main`/`master`
- Work on branches and create clean PRs
- Avoid unnecessary or irrelevant commits

Let’s treat the repository as a production-grade collaborative workspace.

---

## 🆘 Need Help?

If anything is unclear or you’re stuck:
- Ask your domain lead
- Discuss in your team’s communication channel (Slack, Discord, WhatsApp)
- Or raise a GitHub Discussion in the repo


Let me know if you want to include automated templates for issues/PRs to help enforce these rules or a GitHub Action to check naming conventions or enforce linking.
