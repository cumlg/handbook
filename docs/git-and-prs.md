# Git & pull requests

This starts from zero. If you already use Git, skip to [Our workflow](#our-workflow).

## The basics
Git tracks changes to your files; GitHub stores them online and lets us collaborate.

```bash
gh repo clone cumlg/<your-repo>     # get the repo
cd <your-repo>
# ... edit files ...
git add -A                          # stage your changes
git commit -m "Describe what changed"
git push                            # send to GitHub
```

## Branches
Do work on a **branch**, not directly on `main`, so `main` always works:

```bash
git switch -c 12-train-baseline     # new branch, named for issue #12
# ... work, commit ...
git push -u origin 12-train-baseline
```

## Our workflow
We keep it light: **you own your repo and merge your own work.**

- For routine work, merge your branch into `main` yourself — locally, or via a pull request (below). No waiting on anyone.
- Reference the issue in commits or the PR: `Closes #12`.

## Pull requests — when to use one
A **pull request (PR)** is a checkpoint on GitHub that shows exactly what changed (the *diff*) and gives a place to review before merging. Open one when:

- You want **feedback** from your supervisor or a peer.
- It's the code behind a **paper's key result** (so it can be checked for reproducibility).
- You're changing **shared code** (`lab-toolkit`), which affects others.

```bash
git push -u origin <branch>
gh pr create --fill                 # opens the PR
# review the "Files changed" tab on GitHub, then click Merge
```

For everyday exploratory work in your own repo, a PR is optional — committing to `main` is fine.

!!! note "Claude Code can review first"
    Your supervisor can run a first-pass review on your PR automatically. Clear PR descriptions and a linked issue make that fast — which means quicker feedback for you.
