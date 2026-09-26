# DSCI 552 - Homework 2

**Name:** Chengfeng Tang  
**GitHub username:** tcf2021  
**USC ID:** 5488902262

This repository contains my solutions to Homework 2: regression analysis of the Combined Cycle Power Plant dataset and ISLR exercises 2.4.1 and 2.4.7. The notebook includes my answers, code, plots, and executed outputs.

## Files

- `notebook/Tang_Chengfeng_HW2.ipynb`: complete assignment with saved outputs.
- `data/CCPP/Folds5x2_pp.xlsx`: original dataset; I used Sheet1 only.
- `data/CCPP/Readme.txt`: original dataset documentation and citations.
- `requirements.txt`: Python dependencies.
- `reports/Tang_Chengfeng_HW2.pdf`: PDF version of the assignment.
- `latex/`: LaTeX source and figures for the PDF.

## Running the notebook

From the repository root:

```bash
python -m pip install -r requirements.txt
cd notebook
jupyter notebook Tang_Chengfeng_HW2.ipynb
```

The cells can be run sequentially from a fresh kernel. The notebook loads the data using the relative path `../data/CCPP/Folds5x2_pp.xlsx`.

## Methods

I used all observations for parts (b)-(g). For parts (h)-(j), I used the same 70% training and 30% test split with `random_state=42`. Scaling parameters and variable selection were fitted using the training set only.

I used a significance level of 0.05 and preserved model hierarchy during variable selection. KNN regression uses Euclidean distance and uniform weights; the normalized version uses min-max scaling. I retained all observations, including repeated records. I selected k by test MSE, so the reported minimum KNN test error is a model-selection result rather than an independent final evaluation.

References are listed at the end of the notebook.
