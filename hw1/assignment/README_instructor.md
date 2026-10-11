# STA2112 Homework 1 v2 — revised student starter

This package corresponds to the revised v2 assignment. The extended deadline
is October 15, 2026, at 11:59 p.m. Toronto time. Check Quercus for submission details.

This assignment covers Lectures 1–4. Read `Homework 1.pdf` for the questions
and submission requirements, and Quercus for the deadline and submission location.

1. Extract the entire folder. Open `hw1_student.ipynb` with this folder as its
   working directory. In Colab, upload both CSV files into the runtime.
2. Required packages: NumPy, pandas, matplotlib, scikit-learn, and Jupyter
   (or a Colab notebook). XGBoost is **not** required.
3. Q6 implements ridge and estimates bias and variance at one fixed input. The fixed
   simulated design has 60 rows and 5 centered features. Keep the intercept zero.
4. Q7 uses `hitters_hw1.csv`, a subset of the Hitters dataset used in class:
   263 players with observed salary, fixed development/test assignment, and
   five development folds. Only the eight named performance variables are
   predictors. Do not use salary, log salary, row ID, split, or fold as inputs.
5. Complete the marked exercises. Implement `ridge_fit` before calling it;
   its initial `NotImplementedError` marks the function you need to write.
   Submit an executed notebook and the PDF writeup described in the assignment.

The October 1 revision removes extra tasks and shows the marks for each request.
The data, effective model settings, overall 100-point total, and submission
format are unchanged; the PDF gives the revised per-question allocations.
Q2 and Q6 now use the Lecture 2 objective: residual sum of squares
plus lambda times the squared coefficient norm. The ridge equation therefore
contains lambda I. Q6 uses lambda values 0, 2, 20, 200; these give exactly the
same fits as 0, 1, 10, 100 under the earlier half-sum-of-squares convention.
Keep consistently completed work under that earlier convention; no rerun is
required merely to change the labels. Q6 requires the mean-function experiment only:
ignore the existing Y0 variable. Q7(d) is a residual plot and a short commentary
(at most 150 words), not a model-comparison essay. Read the PDF's note if you
completed the earlier SVM option D. Do not redo completed work merely to match
the revised wording.

Do not use test outcomes to choose models or revise the analysis. Record the
CV-selected model before evaluating the test set. The optional supplement is
practice only and requires no submission. Follow the syllabus collaboration
and AI rules.

The PDF explains the geometric and statistical ideas before the relevant
calculations, including the SVM options and the Q5–Q7 workflow. Follow the
numbered requests for assessed work. In the revised SVM option A, (i) asks
for the normal-vector and closest-point reasoning (2 points), and (ii) asks
for the coefficient c and distance (3 points); the Pythagorean identity is
supplied. A still totals 5 points. Already completed work under the earlier
A is accepted without a rewrite. Code, datasets and candidate settings are unchanged.
