![static](https://img.shields.io/badge/Build%20With-Python-brightgreen)![static](https://img.shields.io/badge/Using-NLP%20and%20Machine%20Learning-orange)
# __Duplicate-Questions-pair-Quora__
### Objective is to predict which of the provided pairs of questions contain two questions with the same meaning.
## __Dataset__ : [https://www.kaggle.com/competitions/quora-question-pairs/data]
### Quora is a general-purpose Q&A platform
### One of the many problems that quora face is the duplication of questions. Duplication of question ruins the experience for both the questioner and the answerer. Since the questioner is asking a duplicate question, we can just show him/her the answers to the previous question. And the answerer doesn’t have to repeat his/her answer for essentially the same questions.
![myimage](https://i0.wp.com/www.janagrc.com/wp-content/uploads/2017/02/Questions.jpg)

## Data Overview:
### Available Columns: id, qid1, qid2, question1, question2, is_duplicate
### Class labels: 0, 1
### Total training data / No. of rows: 404290
### No. of columns: 6
### is_duplicate is the dependent variable.
### No. of non-duplicate data points is 255027
### No. of duplicate data points is 149263

### We have 404290 training data points. And only 36.92% are positive. That means it is an imbalanced dataset.
### __NOTE:__ Sampled data to 30000 and 10000 rows beacuse of Hardware contraints, model would've been better if a bigger sample was used.

## Model:
- ### Initial EDA
- ### Basic text data preprocessing,  Bag of words embedding and constructing some basic new features.
- ### Adding more advanced features, including fuzzy features([ https://chairnerd.seatgeek.com/fuzzywuzzy-fuzzy-string-matching-in-python/]) to improve the performance of our model. 
