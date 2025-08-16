# Contributing Guidelines

This guide outlines how we expect all contributors — across all domains (software, mechanical, electrical, simulation, etc.) — to work in a clean, organized, and trackable manner.

---

## 🔁 Git & Workflow Policy

### 🔸 Issue-Driven Development

All changes (features, bug fixes, updates) **must start with an assigned GitHub Issue**.

* **No direct commits** without a corresponding issue.
* Open a GitHub issue **before** starting development and get it assigned to yourself.
* Link the issue to the relevant **Notion task** if applicable.
* All **PRs must reference the issue number** they are solving using GitHub’s linking syntax (e.g., `Fixes #12`).
* If any sub-parts or problems arise while working, create **sub-issues** linked to the main issue.

### 🔸 Branch Naming Convention

Branches must be named using the following format:

```
issue-<issue-number>-<short-description>
```

Examples:

* `issue-42-fix-imu-reading`
* `issue-13-add-path-tracking`
* `issue-101-update-cad-gearbox`

Each PR should:

* Be from one of the above branches.
* Reference the issue it's addressing.
* Be clearly descriptive in its title and body.
* Address and resolve all the comments (if any) from the reviewers before the merge (the merge should be made via squash and merge).

### 🔸 Pull Requests (PRs)

* All code or design contributions must go through a **Pull Request to `main` or `master`**.
* No direct commits are allowed on `main`/`master`.
* PR titles and descriptions should clearly state:

  * What the change is doing
  * What issue it addresses (you can also link it in the PR’s Development section)
  * Any dependencies or related PRs
  * A short video demo (if applicable)

**Reviewer & Assignee Rules:**

* Add your **team leads as reviewers** on every PR.
* Add all people working on the PR (including yourself) as **assignees**.

If multiple PRs address the same issue (for example, different subtasks):

* All of them must reference the **same issue**.
* Link all relevant branches and PRs **within the issue thread**.

---

## 🧠 Task Linking & Traceability

* All **GitHub issues must be linked** to their **corresponding task on Notion**.
* For each GitHub **PR**, add the **PR number and link** in its corresponding issue and Notion task.
* This ensures complete traceability across GitHub and Notion for all technical work.

---

## ⚙️ Workflows and Automation (GitHub Actions)

If you add a GitHub Action or CI/CD workflow (e.g. `build.yml`, `test.yml`):

* **Tag the relevant team leads or repository owners** to ensure:

  * The workflow is reviewed and incorporated into **branch protection rules**.
  * **Branch protection rules** will require:

    * Pull Requests to merge
    * The workflow to complete successfully (✅ green tick)

This ensures we maintain a reliable and stable `main`/`master` branch.

---

## 📌 Issue Closure Protocol

Upon completing a task/feature/bug fix:

* **Close the main issue** and all **related sub-issues**.
* Ensure all comments and feedback under the issue thread are addressed.
* While closing an issue:

  * Attach a **video demonstration** that proves the issue has been fully resolved.
  * Clearly state what was done and that all sub-issues have been completed.

---

## 🎥 Documentation with Videos

For **any contribution** involving domain-specific results, include a **video demo**. Examples include:

* ✅ Mechanical: CAD assembly animation, FEA result walkthrough
* ✅ Electrical: Simulation or schematic demo
* ✅ Software: Terminal demo, UI recording, simulation walkthrough
* ✅ Life Science: ML models predicions, driller mechanism assembly/working simulation

Attach this video directly in the PR or provide a link to an accessible location.

---

## 📁 Repository Requirements

Each repository **must include and maintain** the following:

### 1. `README.md`

A good `README.md` should contain:

* Project overview
* Architecture diagrams (if applicable)
* Setup and installation instructions
* Dependencies
* Video demos

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

* Use meaningful commit messages.
* Do not upload irrelevant or large binary files unless required.
* Keep branches and PRs small and focused.
* Squash commits before merging to `main`.
* Clean up stale branches after merging.

---

## 🔐 Responsibility and Maturity

Branch protection is **not enforced by default**. We trust contributors to:

* Never commit directly to `main`/`master`
* Get the PR reviewed from any of the leads or even your peers to ensure that it’s double checked before the merge.
* Always add team leads as reviewers and all contributors as assignees on PRs.
* Work on branches and create clean PRs
* Avoid unnecessary or irrelevant commits

---

## 🆘 Need Help?

If anything is unclear or you’re stuck:

* Ask your domain lead
* Discuss in your team’s communication channel or in your task on Notion
* Or raise a GitHub Discussion in the Q\&A category

---

### 💬 GitHub Discussions & Idea Sharing

We highly encourage all contributors and team members to actively use the **GitHub Discussions** tab to:

* Ask questions (Q\&A)
* Share interesting ideas or project enhancements
* Vote and engage in polls
* Post results or updates in **Show and Tell**
* Contribute to domain-specific threads under **Technical Discussions** (Electrical, Mechanical, Software, Life Sciences, etc.)

> 💡 **Have an idea or a question? Don’t hesitate — start a discussion!**
> Whether you're brainstorming a new feature or seeking feedback on a challenge, this space is open to all members.

Engaging in Discussions ensures we:

* Promote open collaboration and opinions of others
* Build knowledge across teams
* Document context for future contributors
