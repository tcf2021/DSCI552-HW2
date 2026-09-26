# DSCI 552 - Homework 2

Name: Chengfeng Tang  
GitHub username: tcf2021  
USC ID: 5488902262

The executed assignment is `notebook/Tang_Chengfeng_HW2.ipynb`.
The PDF follows the same question-by-question order, including code and outputs.

## Files

- `notebook/Tang_Chengfeng_HW2.ipynb`: answers, code, plots, and saved outputs.
- `data/CCPP/Folds5x2_pp.xlsx`: original dataset workbook; only Sheet1 is used.
- `data/CCPP/Readme.txt`: original dataset documentation and citations.
- `requirements.txt`: Python dependencies.
- `reports/Tang_Chengfeng_HW2.pdf`: PDF copy.
- `latex/`: LaTeX source and figure files.

## Run locally

From the repository root:

```bash
python -m pip install -r requirements.txt
cd notebook
jupyter notebook Tang_Chengfeng_HW2.ipynb
```

Restart the kernel, run all cells in order, and save the notebook with its outputs.
The data path is relative to `notebook/`: `../data/CCPP/Folds5x2_pp.xlsx`.
The notebook needs no network connection after dependencies are installed.

Parts (b)-(g) use all observations. Parts (h)-(j) share a 70%/30% split with
`random_state=42`. Normalization and variable selection use training data only.
KNN uses uniform weights and Euclidean distance. The normalized version uses
min-max scaling. All observations, including repeated records, are retained.
The reported minimum KNN test error uses the test set to choose k, as in the
assignment comparison; it is not an independent final evaluation.

## GitHub submission

Create your own repository under `tcf2021`, using the visibility and TA access
required by the course. Place the contents of this project directly in the
repository root; do not upload only the ZIP file. Check that the notebook,
data, and requirements file appear on GitHub and that notebook outputs display.

If using Git locally, replace `YOUR_REPOSITORY` with the repository name:

```bash
git init
git add .
git commit -m "Complete DSCI 552 Homework 2"
git branch -M main
git remote add origin https://github.com/tcf2021/YOUR_REPOSITORY.git
git push -u origin main
```

No GitHub repository has been created or submitted by this file package itself.
