# How we work

Three GitHub things carry all our work. Understand these and you understand the system.

## Repositories — where the work lives
Each student has one repo for their workstream: code, notebooks, and the record of every task and experiment. Yours is your home base.

## Issues — the unit of work
**Every task or experiment is a GitHub issue.** Not an email, not a note to self.

- Use the **Task** template for work, the **Experiment** template for a run (hypothesis and setup up front; the result as the closing comment), the **Plan** template for a paper or a milestone deliverable that other issues feed into.
- Discuss the work **in the issue comments** — that keeps the discussion attached to the task and searchable forever.
- Label with `experiment`, `task`, `plan`, `bug`, `paper`, `reading`, or `blocked`.

## The board — the shared view
The group board **[Workstreams](https://github.com/orgs/cumlg/projects/1)** pulls every issue from every repo into one place, so the whole group's work is visible at a glance. Every issue you open is added automatically within half an hour, with its **Project** already set. You don't have to maintain it: what your supervisor reads is your issues and your weekly log, not the board's columns. Move cards or set **Priority** if it helps you; the `blocked` label is the one thing that must be set on the issue itself.

## Milestones — the arc of the work
The three things above carry the day-to-day. **Milestones** give it a spine: they bundle issues toward a checkpoint and show progress as those issues close. Use them where there is a real checkpoint; don't attach issues to a milestone for its own sake.

- **Candidature stages** are milestones in your repo — **M1 — Candidacy**, **M2 — Mid-candidacy review**, **M3 — Final review & submission**. Attach each task or experiment to the stage it belongs to; your supervisor sets the due dates for your timeline. What each stage involves, for you and for your supervisor: [M1 — Thesis proposal](stages/m1-thesis-proposal.md).
- **A paper** is its own milestone named `Paper: <venue>` (e.g. `Paper: ICES2026`), with the submission deadline as its due date. Its work-package issues attach to it.
- **A contract/partner deliverable** is its own milestone named `Deliverable — <name>` (e.g. `Deliverable — ML surrogate model`), with the deliverable's due date. Its tasks attach to it.

Every milestone surfaces on the board's **Milestone** field, so the whole group's checkpoints sit in one view.

## The loop
1. Open an issue for what you're about to do.
2. Work on it (see [Git & pull requests](git-and-prs.md)).
3. Record the result on the issue (see [Experiments](experiments.md)).
4. Close the issue when done. An issue that is finished but still open looks like work in progress to everyone else.

The [weekly rhythm](weekly-rhythm.md) wraps a light cadence around this loop.
