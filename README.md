# Exercise Quality Prediction

**Student:** SOMAPURAM UDAY  
**Course:** Practical Machine Learning, Johns Hopkins University  
**Assignment:** Peer-graded Assignment – Prediction Assignment Writeup  

Machine learning project predicting **barbell exercise quality** using a Random Forest classifier.

---

## Problem Statement / Background

Using devices such as Jawbone Up, Nike FuelBand, and Fitbit, it is possible to collect a large amount of personal activity data inexpensively. These devices are part of the **quantified self movement**, where individuals measure themselves to improve health or find behavioral patterns.  

Most analyses focus on **how much** activity is done, but rarely on **how well** it is performed. In this project, accelerometer data was collected from the **belt, forearm, arm, and dumbbell** of 6 participants performing barbell lifts correctly and incorrectly in 5 ways. The goal is to **predict exercise quality** based on this data.  

**Dataset source:**  
[Weight Lifting Exercise Dataset](http://web.archive.org/web/20161224072740/http:/groupware.les.inf.puc-rio.br/har)

---

## Quick Results
- **Accuracy:** High performance on validation data  
- **Algorithm:** Random Forest (50 trees for speed)  
- **Validation:** Out-of-sample error estimated using **k-fold cross-validation**  
- **Data:** Accelerometer measurements from 6 participants  

---

## Files
- `prediction_analysis.Rmd` – R Markdown source with full analysis  
- `prediction_analysis.html` – Compiled HTML report for easy viewing  
- `final_predictions.csv` – Predictions for 20 test cases  
- `README.md` – This file  

> View the complete analysis and results [here](https://udaycodespace.github.io/exercise-quality-prediction/).

---

## Dataset
- **Training Observations:** 19,622  
- **Features:** Accelerometer data from belt, forearm, arm, and dumbbell  
- **Classes:**  
  - `A` – Correct form  
  - `B-E` – Common mistakes  

**Data links:**  
- [Training Data CSV](https://d396qusza40orc.cloudfront.net/predmachlearn/pml-training.csv)  
- [Test Data CSV](https://d396qusza40orc.cloudfront.net/predmachlearn/pml-testing.csv)  

---

## Tech Stack
- **Language:** R  
- **Libraries:** caret, randomForest, ggplot2, dplyr  
- **Tools:** RStudio, GitHub, HTML rendering via R Markdown  

---

## Model Building
- **Algorithm:** Random Forest classifier  
- **Implementation:** Built in R using training dataset  
- **Parameters:** 50 trees for speed and accuracy balance  
- **Feature Handling:** Preprocessed accelerometer data for model input  
- **Justification:** Random Forest is robust to noisy sensor data and performs well without extensive tuning  

---

## Model Evaluation
- Performance evaluated on validation data  
- **Cross-validation** used to estimate out-of-sample error  
- Metrics reported: Accuracy, confusion matrix, and expected error  

---

## Reproducibility / Peer Review
- Repository includes both `.Rmd` and compiled HTML → satisfies peer-review requirement  
- Write-up constrained to < 2000 words and fewer than 5 figures  
- Predictions for the 20 test cases are included in `final_predictions.csv`  
- HTML viewable online via GitHub Pages  

---

## Summary

- In this project, I built a machine learning workflow to predict barbell exercise quality using accelerometer data from multiple sensors.  
- I included both the R Markdown source and the compiled HTML report in my GitHub repository to make my analysis reproducible and easy to review.  
- I chose a Random Forest model and carefully documented how I built it, including feature handling and parameter selection.  
- I applied cross-validation to estimate out-of-sample error, ensuring that my model generalizes well to unseen data.  
- This submission represents my independent work and meets all the requirements outlined in the assignment rubric.
