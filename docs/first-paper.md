# Your first paper

How your first paper runs in this group. Each paper is a `Paper: <venue or working title>` milestone with a Plan issue behind it ([how milestones work](how-we-work.md#milestones-the-arc-of-the-work)).

!!! note "Who this is for"
    Students writing their first paper in the group, and their supervisor. *You deliver* is what the student produces; *I provide* and *I hold back from* are what the supervisor gives and refrains from. Treat the supervisor lines as a contract — if I am not keeping to them, say so.

## What the first paper is for

A publication, and the one paper where you learn how a paper is made — with me, closely: three to five rounds of comments, and the submission done together. The real deliverable is a student who can state the paper's contribution in one sentence, build the story that leads a reader to it, and run a paper from plan to submission with every number reproducible.

**The bar:** a journal in JCR Q1 for its category — civil/structural engineering or machine learning. The venue itself may be known from the start or decided when the paper is done; either is fine.

## The contribution

A **contribution** is what a reader can do or know after your paper that they could not before — not what you did, but what changed. One to three per paper. Each must pass three tests:

- **new** — the closest prior work is named and the difference stated;
- **checkable** — the figure or table that demonstrates it is named;
- **matters** — what the result makes possible, cheaper, safer, or settles, that a reader of this journal would care about.

The contribution statement is the one thing I ask for before the full draft, because everything else is judged against it: the introduction tells the story that leads to it, in five moves — *problem → existing methods → where they stop and why → what we propose → our contributions*; related work is organised around it; every experiment supports it; the conclusion says whether it held.

How you get there is yours. Some people know the contribution from the plan. I usually don't — I write the method and experiments first and let the contribution emerge from the results. Either is fine. One suggestion from the papers that went wrong: until the statement passes, keep the method and experiments as notes, and leave the introduction, related work and conclusion for last. Those are the sections that get rewritten when the contribution moves, and rewriting a finished introduction is the most common first-paper setback.

## Exit criteria — what "ready to submit" means

All of these. Copy this list into the plan issue as a checklist, and tick the items off there, not on this page.

- Contribution statement passes all three tests; you can defend it without notes.
- The introduction tells the story in five moves; a reader could predict the contributions before reaching them.
- Every section serves the contributions, as above.
- Every figure and table regenerates from the repo at a tagged commit, from the README alone, checked from a fresh clone — `Reproduced:` comment on the plan issue.
- Authorship recorded on the plan issue before the first draft.
- Every co-author has read it and every comment has an answer.
- AI log current; the venue's AI declaration written from it.
- My sign-off against this list, on the plan issue.

## Kill criteria

- **Contribution statement fails the tests after two revisions** → back to experiments or re-scope. Wording is never the fix.
- **Key result does not reproduce** → no submission until it does; if it cannot, the claim changes to what does.
- **A baseline is unfair or a stronger prior method turns up** → fix the comparison first, even if the result weakens.
- **Flag — after round 3 I am still commenting on the story, not the sentences.** That is an ownership problem, and we talk about it directly.

## Stages

Planned backwards from the submission target. Durations are first-paper defaults.

### 0 — Plan (one week)

**You deliver** — the `Paper: <venue or working title>` milestone with the submission target as its due date, and the `[plan] Paper: …` issue from the template: backwards timeline, proposed authorship, exit criteria, and the venue if already known.

**I provide** — authorship recorded before anything is written; the first-draft date I will hold you to.

### 1 — Contribution (two to six weeks)

**You deliver** — the contribution statement as a comment on the plan issue, revised weekly, every version posted; the story in five moves, one paragraph each; a **figure plan** — the three to six figures and tables that will demonstrate the contributions, each labelled with the one it supports; a ten-minute **contribution talk** at a progress meeting.

**I provide** — reviewer mode on every version: which test it failed, and an explicit "this passes" before the stage ends; help finding the contribution when it is hiding in your results — I say what I think it is, you write the statement; the comparisons reviewers will demand.

**I hold back from** — writing the statement for you; letting a version sit more than two weeks without a verdict; adding contributions — three is the maximum.

### 2 — First draft (four to six weeks)

**You deliver** — a complete manuscript in Overleaf, shared with me from day one. If you want an order to write in, mine is: figures and tables with captions → method → experiments → related work → introduction → conclusion → abstract → title. References from your reference manager, for papers you have read; no placeholders. Before hand-over, check that every paragraph serves a contribution — cut or move the rest. Then a `Ready for round 1` comment on the plan issue.

**I provide** — a weekly checkpoint at the 1:1 and answers to specific questions. The round-1 read within a week of `Ready for round 1`.

**I hold back from** — reading half a draft; "you could also…".

### 3 — Rounds (three to five, one week each way)

**Rounds 1–2** are structure and argument, inline in Overleaf. **Rounds 3–5** are the text, on a PDF. When I have no structural comments left, I decide the venue if it is still open — recorded on the plan issue, milestone renamed — and say "ready for co-authors"; you send it to all co-authors at once with a date two weeks out, and answer every comment. Disagreements come to me.

**You deliver** — each round back within a week; every comment resolved or answered, never silently — if you disagree, say so and why; a `Round N:` comment on the plan issue each time.

**I provide** — each round back within a week, or a date; comprehensive comments — what a paragraph fails to do, not just that it fails; the venue, if not decided at the start.

**I hold back from** — rewriting your sentences, so that you can write the next paper; grammar comments in round 1; letting the draft reach co-authors before the rounds are done.

### 4 — Check and submit (the same two weeks as the co-author read)

**You deliver** — a `paper/` directory in your repo: one command regenerates every figure and table from stored results, with a README; tag `submission-v1`. Then the check from a fresh clone: an AI coding agent reproduces everything from the README alone, without you steering it; if it cannot, the README is incomplete — fix, retag, repeat. Post `Reproduced:` on the plan issue. The manuscript in the venue's template; the AI declaration from the AI log; a one-page cover letter; the exit criteria ticked; submission with me in the room.

**I provide** — sign-off against the exit criteria, not the deadline; the submission session.

**I hold back from** — submitting without the check to hit a deadline. We move the deadline.

### 5 — After submission

Rejection is normal; most first papers get one. Within a week of a decision, post the reviews on the plan issue with a triage table — one line per reviewer point: *fix / argue / decline*, with a reason. Within two weeks, `Decided at 1:1`: resubmit here or go to the next venue, new target on the milestone. The response letter answers every point, saying what changed and where; I read it before it goes. Resubmit within four to six weeks unless new experiments are needed.

**On acceptance:** tag `accepted`, citation in the repo README, close the milestone, tell any partner whose data it used, present it at a paper-reading hour.

## Authorship — decided before the first draft

- **First author:** the person who led the work and wrote the first draft — on a paper from your thesis, you.
- **Corresponding author:** me, as principal supervisor.
- **Co-authors:** co-supervisors, and anyone whose intellectual contribution the paper depends on — a method idea in the paper, code the results depend on, data collected for it, substantial writing or revision. Reading once, running an experiment to a recipe, or supervision alone is an acknowledgement.
- **Order:** first author, then by contribution. Roles in [CRediT](https://credit.niso.org/) terms, on the plan issue. Changes need a comment everyone named agrees to.
- **Who reads the first draft:** me, alone, until I say "ready for co-authors". Nothing goes to co-authors or outside the group before that.

## Using AI

The group rules on [Using AI](ai-claude-code.md) apply, plus two: **citations are read, not generated** — every `.bib` entry is a paper you have opened; and **keep an AI log** — one comment on the plan issue (tool, what for, which sections), from which you write the venue's AI declaration. AI is never an author.

!!! warning "Not written yet"
    A consistent group way of using AI in the writing itself is not established yet. Until it is, the rules above and your judgement apply, and the AI log records what you did.

## Templates

**Paper plan** — the body of the `[plan] Paper: …` issue. *T* is the submission target.

```
Submission target (T): YYYY-MM-DD   ← milestone due date
Venue: <journal, JCR Q1> — or "open", decided when the paper is done; milestone renamed then

- T−22w  Plan agreed; authorship recorded
- T−16w  Contribution statement passes; story and figure plan agreed
- T−15w  Contribution talk
- T−10w  First draft → "Ready for round 1"
- T−10w … T−2w  Rounds 1–4
- T−2w   Venue decided if open; co-authors; reproducibility check; venue template; AI declaration; cover letter
- T       Submit together

Authorship (agreed YYYY-MM-DD): 1. <student>, first — CRediT: …  2. Qilin Li, corresponding — CRediT: …  3. …
AI log: <one comment below, kept current>
Exit criteria: <paste from the handbook>
```

**Contribution statement** — a new comment for every version.

> This paper shows that [claim] by [approach] on [data / setting].
>
> **C1.** [One sentence.] *Demonstrated by:* Fig./Table X. *New because:* the closest prior work is [ref], which [does not …]. *Matters because:* [what it makes possible, cheaper, safer, or settles].
>
> *It would not hold if:* [the result a reviewer could point to].

**Round comment**

```
Round N (YYYY-MM-DD) — Changed: …  Pushed back on: … because …  Still open: …
```

**Reproduced comment**

```
Reproduced: tag submission-v1 (<sha>), fresh clone on <machine>, run by <agent> from the README alone. Figures N/N, tables M/M. Exceptions: …
```

## Where things live

- **Milestone** `Paper: <venue or working title>`, renamed to the venue once decided, due date = submission target. **Plan issue** `[plan] Paper: …` attached to it — body: the template; comments: statement versions, AI log, `Ready for round 1`, `Round N:`, `Reproduced:`, reviews and triage, `Decided at 1:1`.
- **Experiments** feeding the paper: Experiment issues on the milestone, closed with `Result:`.
- **Manuscript:** Overleaf, shared with me from day one, linked from the plan issue. If a venue or senior co-author requires Word: one owner, everyone else tracked changes.
- **References:** your reference manager (Zotero recommended) → `.bib`. Nothing by hand, nothing from a model.
- **Code, results, figures:** your repo, `paper/` directory; tags `submission-v1`, `revision-v1`, `accepted`.
