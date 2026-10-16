# Experiments & reproducibility

The goal: **any result can be reproduced** — by you in six months, or by a collaborator. This is the heart of how we work.

## One issue per experiment
Open an issue with the **Experiment** template. Up front it asks for what you know before the run:

- **Hypothesis / question** — what you're testing and what you expect.
- **Setup** — model, key hyperparameters, data (which set, which version), branch/commit.
- **Links** (optional) — W&B run, Roboflow version, DVC hash, whichever you use.

**The result is the closing comment.** When the run is done, post a comment that starts with `Result:` — what happened, the number, the next step — and close the issue. A table in the comment is fine; so is a sentence. An experiment closed without a Result comment counts as not done, and the weekly digest flags it.

Now the experiment documents itself, and your supervisor can review it without a meeting.

## Track runs in Weights & Biases (recommended)
```python
import wandb
wandb.init(project="<your-repo>", config=hyperparams)
# ... training ...
wandb.log({"val_rmse": rmse})
```
Paste the run URL into the issue's Links field or the Result comment. W&B keeps the metrics, the config, and — via Artifacts — datasets and checkpoints. If you track runs some other way, the Result comment still has to carry the number and enough setup to reproduce it.

## Version the inputs
Code is in git (note the commit). Data and models are in [DVC or W&B](data.md). Together these mean a result = **code commit + data version + config**, all recoverable.

## Reproducible environments
Keep `requirements.txt` (or `environment.yml`) current so anyone can rebuild your environment. Pin versions for anything that affects results.

!!! tip "The reproducibility test"
    Could someone else reproduce your latest number from the issue alone — the commit, the dataset version, the config, the W&B run? If not, something's missing.
