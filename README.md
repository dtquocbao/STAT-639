# STAT 639 Homework

Solutions for STAT 639 (Spring 2026), written in R Markdown against *An Introduction to Statistical Learning*, 2nd edition (ISLR). Each homework has a source `.Rmd` and a knitted PDF. Question sheets are included for Homework 3 and Homework 4.

| Homework | Source | PDF | Status |
| --- | --- | --- | --- |
| 1 | [STAT639_HW1.Rmd](STAT639_HW1.Rmd) | [STAT639_HW1.pdf](STAT639_HW1.pdf) | Complete |
| 2 | [STAT639_HW2_Updated.Rmd](STAT639_HW2_Updated.Rmd) | [STAT639_HW2_Updated.pdf](STAT639_HW2_Updated.pdf) | Revised writeup |
| 3 | [STAT639_HW3.Rmd](STAT639_HW3.Rmd) | [STAT639_HW3.pdf](STAT639_HW3.pdf) | Draft |
| 4 | — | [stat639_hw4_questions.pdf](stat639_hw4_questions.pdf) | Questions only |

[STAT639_HW2.Rmd](STAT639_HW2.Rmd) and [STAT639_HW2.pdf](STAT639_HW2.pdf) are the earlier Homework 2 writeup. [STAT639_HW2_Updated.Rmd](STAT639_HW2_Updated.Rmd) covers the same exercises with a fuller solution.

## Assignments

**Homework 1** — ISLR Chapter 2, Exercises 1, 2, 8, and 10. Exercise 8 uses the local [College.csv](College.csv). Exercise 10 uses the `Boston` data from `ISLR2`.

**Homework 2** — ISLR Chapter 4, Exercises 1, 4, 8, and 14, and Chapter 9, Exercise 3(a)–(f). The applied parts use `Auto` from `ISLR2`, plus `MASS`, `e1071`, and `class` (LDA, QDA, naive Bayes, and KNN).

**Homework 3** — ISLR Chapter 5, Exercises 3 and 6; Chapter 6, Exercises 2, 3, and 9(a)–(d); Chapter 8, Exercises 4 and 5. Applied parts use `Default` and `College` from `ISLR2`, with `boot` for the bootstrap and `glmnet` for ridge and lasso. The assignment sheet is [stat639_hw3_questions.pdf](stat639_hw3_questions.pdf). Due March 31, 11:59pm Central Time.

**Homework 4** — questions only, in [stat639_hw4_questions.pdf](stat639_hw4_questions.pdf). Due April 21, 11:59pm Central Time.

1. ISLR Chapter 8, Exercise 9
2. ISLR Chapter 8, Exercise 10(a)–(e)
3. ISLR Chapter 10, Exercise 1
4. ISLR Chapter 10, Exercise 4(a)–(b)
5. Prove the within-cluster sum-of-squares identity from slide set 7
6. ISLR Chapter 12, Exercise 3

## Knit a homework

From this directory, with [R](https://www.r-project.org/) and `rmarkdown` installed:

```r
rmarkdown::render("STAT639_HW3.Rmd")
```

Install packages the first time a file needs them:

```r
install.packages(c("ISLR2", "MASS", "e1071", "class", "boot", "glmnet"))
```

Homework 1 reads `College.csv` from the working directory, so render it from the repository root.
