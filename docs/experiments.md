# Experiments & reproducibility

The goal: **any result can be reproduced** — by you in six months, or by a collaborator. This is the heart of how we work.

## One issue per experiment
Open an issue with the **Experiment** template. It captures:

- **Hypothesis / question** — what you're testing.
- **Dataset version** — the Roboflow version or DVC hash.
- **Setup** — model, key hyperparameters, branch/commit.
- **W&B run link** — the metrics.
- **Result / conclusion** — filled in after, with the next step.

Now the experiment documents itself, and your supervisor can review it without a meeting.

## Track every run in Weights & Biases
```python
import wandb
wandb.init(project="<your-repo>", config=hyperparams)
# ... training ...
wandb.log({"val_rmse": rmse})
```
Paste the run URL into the experiment issue. W&B keeps the metrics, the config, and — via Artifacts — datasets and checkpoints.

## Version the inputs
Code is in git (note the commit). Data and models are in [DVC or W&B](data.md). Together these mean a result = **code commit + data version + config**, all recoverable.

## Reproducible environments
Keep `requirements.txt` (or `environment.yml`) current so anyone can rebuild your environment. Pin versions for anything that affects results.

!!! tip "The reproducibility test"
    Could someone else reproduce your latest number from the issue alone — the commit, the dataset version, the config, the W&B run? If not, something's missing.
