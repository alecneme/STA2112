# STA 2112 — Statistical Learning I (UofT, Fall 2026)

Code and writeups for STA 2112 homework.

## Layout
```
hw1/                         Homework 1 v2 (due Thu Oct 15, 11:59 p.m. Toronto)
├── hw1_student.ipynb        Q6-Q7 code, outputs and explanations (submitted, executed)
├── ridge_design.csv         supplied data, kept beside the notebook
├── hitters_hw1.csv          (Quercus instruction), loaded with DATA = Path(".")
├── scans/                   photos of handwritten Q1-Q5 derivations
├── code/                    .py files exported from the notebook, if needed
└── assignment/              handout PDFs + instructor README (read-only reference)
```

## Submission (two files on Quercus)
1. `hw1_student.ipynb`, executed (Restart -> Run All first).
2. PDF writeup = handwritten Q1-Q5 scans + PDF export of the notebook for Q6-Q7.

## Setup
- Python with `numpy`, `pandas`, `matplotlib`, `scikit-learn`, `ipykernel`
- Open **this folder** in VS Code (File -> Open Folder), not individual files.
- Notebook runs with `hw1/` as its working directory.

## Reproducibility rules
- Seed 2112 (`SEED`); one seeded generator per notebook: `rng = np.random.default_rng(SEED)`, passed into functions.
  Use separate fresh generators (`default_rng(0)`) for tests.
- Data are the supplied CSVs beside the notebook; always load from there.
- Every figure is produced by code in the notebook.
- Small functions, each tested against a known answer before use.
- Before taking final numbers: Restart -> Run All, so everything comes from one clean run.
- Keep the notebook tidy (it is submitted); ASCII-only code comments.
- Q7: record CV-selected models before touching the test set.

## Daily routine
1. Start: `git pull`
2. Work, then **save** (Ctrl+S) — git only sees saved files
3. `git status` — check what changed (nothing listed = not saved)
4. `git add <files>` (or `git add .` once status looks right)
5. `git commit -m "Short present-tense description of one change"`
6. `git push` — at least at the end of every session
