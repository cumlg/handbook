# Weekly rhythm

A light cadence around the [daily loop](how-we-work.md).

## Monday — plan in the open
- Post a 3-line update on your **weekly-log** issue: *did last week / doing this week / blocked on.* Link the issues you mention (`#12`).
- Close anything you finished last week.

That update is your progress record — three minutes, and your supervisor always knows where you are.

## What you get back
- Your supervisor reads every weekly log and **replies on it every week**, even if briefly. The reply lists the issues he commented on that week, so it doubles as an index.
- **Substantive comments live on the issue they concern** — a technical objection, a decision, a change to an experiment — not on the weekly log. That keeps the discussion next to the work, where you and anyone reading the issue later will find it.
- No reply on your log by Tuesday means it was missed, not ignored — say so at your 1:1.

## During the week
- Work on branches; discuss in issue comments.
- Log experiments to W&B as you go.
- Flag anything stuck with the `blocked` label so it surfaces.

## Meetings
The cadence changes from time to time; this is the current one.

- **Paper reading** (weekly, one hour): we take turns presenting a paper — or something else worth the hour, such as a proposal talk or a mock candidacy.
- **Progress meeting** (fortnightly): about ten minutes each on your own work — did / doing / stuck, and the result or decision that matters.
- **1:1 with supervisor** (weekly, 30–60 minutes): driven off your weekly log and open issues; bring your agenda.
- **After your 1:1, add an entry to your `1:1 notes — <Name>` issue** — same day, or the next
  working day. One comment per meeting, in this shape:

  ```markdown
  ### 1:1 2026-10-22
  - **Discussed:** intro framing (#23); timing of the M1 proposal
  - **Decided:** rewrite the intro around the distilled contributions (#23)
  - **Qilin will:** read the contribution list
  - **I will:** post the contribution list on #23 before the rewrite
  - **Next 1:1:** first draft of the research questions
  ```

  Link every issue you discussed (`#23`); GitHub then shows the entry on that issue's timeline.
  This is the record of what we agreed, in your words. Your supervisor reads every entry and
  replies on it only when something reads differently from what he understood — **no reply by
  your next 1:1 means agreed.** No 1:1 this week means no entry. Comments on that issue are your
  entries and his corrections only; everything else goes on the issue it concerns.
- **And write each decision back on its issue** — one comment per issue discussed, starting with
  this line so it can be found later:

  ```
  Decided at 1:1 (2026-10-22): <what was decided, and what you will do next>
  ```

  If your supervisor said "let's decide #30 at the 1:1", #30 counts as open until that comment is
  on #30 — he checks for it each week, and will ask in his weekly-log reply if it is missing (also
  when the decision is in your 1:1 notes but not yet on #30). Decided something that has no issue
  yet? Open one (Task) and write the decision there.
  Writing it yourself is the point: if it reads differently from what he understood, it gets
  corrected now rather than a month later.

## Milestones
Your candidature stages (**M1–M3**), each **`Paper: <venue>`**, and any contract **`Deliverable — <name>`** are milestones in your repo ([how milestones work](how-we-work.md)). Keep a milestone's due date honest: when it passes, close it with what was delivered or move the date — a milestone that is months overdue tells nobody anything.
