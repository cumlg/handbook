# Getting started

Your first day, step by step. It should take under an hour.

## 1. Accounts & access
1. Accept the email invite to the **`cumlg`** GitHub organisation and your project team (`decra`, `linkage`, or `dot`).
2. **Enable two-factor authentication** on your GitHub account — it's required for the org.
3. Install [Git](https://git-scm.com/) and the [GitHub CLI](https://cli.github.com/) (`gh`), then run `gh auth login`.

## 2. Your repository
Your work lives in one repo named `<project>-<workstream>` (e.g. `linkage-damage-detection`). It was created from our [`project-template`](https://github.com/cumlg/project-template), so it already has the folder structure, conventions, and a `CLAUDE.md`.

```bash
gh repo clone cumlg/<your-repo>
cd <your-repo>
python -m venv .venv && source .venv/bin/activate   # or conda
pip install -r requirements.txt
```

## 3. Read these two files
- **`README.md`** — what your repo is and where its data lives.
- **`CLAUDE.md`** — the conventions your code (and Claude Code) should follow.

## 4. Open your first issue
Every piece of work starts as a GitHub issue. Open one describing your first task or experiment (use the **Experiment** template for a run). See [How we work](how-we-work.md).

## 5. Put it on the board
Your issues appear on the group board, **Workstreams — Qilin Li**. Set the **Project** field and drag your issue into **This week**.

!!! tip "New to Git or GitHub?"
    Read [Git & pull requests](git-and-prs.md) — it starts from zero and only assumes you can edit a file.
