# DATA 37711 — Homework 3

All solutions are in **[`homework3.ipynb`](homework3.ipynb)**, which is committed with its outputs.

| Problem | Content |
|---|---|
| 1 | Poisson boosting: link function, loss, gradient, how each tree is chosen |
| 2 | Generalization bound for hyperparameter selection on a held-out set (Hoeffding + union bound), the winner's-curse simulation, and a train/validation/test grid search on white wine (RandomForest and k-NN) |
| 3 | Gradient boosting with 1–1000 trees on `dset0` and `dset1`, and why the two behave differently |

## Run it

```bash
pip install -r requirements.txt
jupyter nbconvert --to notebook --execute homework3.ipynb --output executed.ipynb
```

Or open the notebook and choose *Restart & Run All*. A full run takes about 3–4 minutes, mostly the random-forest grid search.

## Data
- `dset0-1.csv`, `dset1-1.csv`: course datasets. The first column is the binary label.
- `winequality-white.csv`: the UCI Wine Quality (white) dataset. If the file is missing, the notebook downloads it.
