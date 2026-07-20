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
The group board **[Workstreams](https://github.com/orgs/cumlg/projects/1)** pulls every issue from every repo into one place, so the whole group's work is visible at a glance. Every issue you open is added automatically within half an hour, in **Backlog**, with its **Project** already set — you keep the rest current:

- Drag issues across **Backlog → This week → In progress → Blocked → In review → Done**.
- Set the **Priority** field.

## Milestones — the arc of the work
The three things above carry the day-to-day. **Milestones** give it a spine: they bundle issues toward a checkpoint and show progress as those issues close.

- **Candidature stages** are milestones in your repo — **M1 — Candidacy**, **M2 — Mid-candidacy review**, **M3 — Final review & submission**. Attach each task or experiment to the stage it belongs to; your supervisor sets the due dates for your timeline.
- **A paper** is its own milestone named `Paper: <venue>` (e.g. `Paper: ICES2026`), with the submission deadline as its due date. Its work-package issues attach to it.
- **A contract/partner deliverable** is its own milestone named `Deliverable — <name>` (e.g. `Deliverable — ML surrogate model`), with the deliverable's due date. Its tasks attach to it.

Every milestone surfaces on the board's **Milestone** field, so the whole group's checkpoints sit in one view.

## The loop
1. Open an issue for what you're about to do.
2. Work on it (see [Git & pull requests](git-and-prs.md)).
3. Log experiments to [Weights & Biases](experiments.md).
4. Close the issue when done; it moves to Done on the board.

The [weekly rhythm](weekly-rhythm.md) wraps a light cadence around this loop.
