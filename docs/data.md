# Where data lives

**Nothing large goes in git.** Git is for code and text. Big files live in the right specialist tool, with a pointer from your repo.

| What | Where it lives | How you reference it |
|---|---|---|
| Code, notebooks, configs | Your **GitHub repo** | — |
| Image datasets + labelling | **Roboflow** | Record the dataset version in the issue |
| Experiment runs & metrics | **Weights & Biases** | Paste the run URL in the issue/PR |
| Large data, 3D, sim output, checkpoints | **DVC** → institutional storage | Commit the small `.dvc` pointer |

## Why
A 2 GB dataset or a `.blend` file in git bloats the repo and can't be meaningfully diffed. Keeping bytes out of git keeps clones fast and history clean — while DVC and W&B still give you full versioning and provenance.

## DVC in practice
```bash
pip install dvc
dvc init
dvc remote add -d storage <institutional-remote>   # e.g. Pawsey / research drive
dvc add data/raw/bigfile.h5        # tracks the file, writes a small .dvc pointer
git add data/raw/bigfile.h5.dvc data/raw/.gitignore
git commit -m "Track dataset with DVC"
dvc push                           # uploads the bytes to the remote
```
Anyone can then `git pull && dvc pull` to get the exact code **and** data for a result.

## Your repo's data folder
`data/raw/` (never edit in place), `data/interim/`, `data/processed/` — all DVC-tracked and git-ignored. See `data/README.md` in your repo.
