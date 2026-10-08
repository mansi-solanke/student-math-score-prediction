 # Student Math Score Prediction

Kaggle notebook: https://www.kaggle.com/code/mansiiiiiiiiiiiii/student-math-score-prediction

This is my first data science project. I wanted to see what affects how students score in math, and whether I could train a model to predict the scores. I used the "Students Performance in Exams" dataset from Kaggle (1,000 students, 8 columns).

## What I did
1. Loaded the data with pandas and checked it. Nothing was missing, so I didn't have to clean anything.
2. Plotted the math scores as a histogram. Most students got around 66, and the graph looked like a bell curve.
3. Compared groups to see what makes a difference in scores.
4. Trained a Linear Regression model (scikit-learn) to predict math scores, and checked how far off it was.

## What I found
- Students who finished the test prep course scored about 5.6 points higher in math on average (69.7 vs 64.1).
- Students whose parents have a master's degree scored higher than students whose parents only finished high school (69.7 vs 62.1).

## My two models
- **Model 1** (all columns, including reading and writing scores): off by about 4.2 points on average, R2 = 0.88.
- **Model 2** (only background info, without reading and writing scores): off by about 11.3 points on average, R2 = 0.18.

## What I learned
Reading and writing scores made the prediction much better, since students who are good at one subject are usually good at the others. Things like parents' education and test prep do show a pattern, but they don't explain most of the difference between students. I also learned that just because two things go together doesn't mean one causes the other.

## Tools
Python, pandas, matplotlib, scikit-learn
