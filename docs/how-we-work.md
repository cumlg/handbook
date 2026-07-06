# How we work

Three GitHub things carry all our work. Understand these and you understand the system.

## Repositories — where the work lives
Each student has one repo for their workstream: code, notebooks, and the record of every task and experiment. Yours is your home base. Shared code that several people reuse lives in [`lab-toolkit`](https://github.com/cumlg/lab-toolkit) — import from there instead of copying.

## Issues — the unit of work
**Every task or experiment is a GitHub issue.** Not an email, not a note to self.

- Use the **Task** template for work, the **Experiment** template for a run (it captures hypothesis, dataset version, W&B link, result).
- Discuss the work **in the issue comments** — that keeps the discussion attached to the task and searchable forever.
- Label with `experiment`, `task`, `bug`, `paper`, `reading`, or `blocked`.

## The board — the shared view
The group board **Workstreams — Qilin Li** pulls every issue from every repo into one place, so your supervisor sees the whole group at a glance. You keep your part current:

- Drag issues across **Backlog → This week → In progress → Blocked → In review → Done**.
- Set the **Grant** and **Priority** fields.

## The loop
1. Open an issue for what you're about to do.
2. Work on it (see [Git & pull requests](git-and-prs.md)).
3. Log experiments to [Weights & Biases](experiments.md).
4. Close the issue when done; it moves to Done on the board.

The [weekly rhythm](weekly-rhythm.md) wraps a light cadence around this loop.
