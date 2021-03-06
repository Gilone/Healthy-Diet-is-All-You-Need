# Healthy Diet is All You Need

Hao Feng, Kaiqi Jin, Mingqing Xu and Pai Tong

## Abstract

Analyzing calories based on recipes is a critical and meaningful task for many platforms.

In this paper, we aim to predict the calories of recipes from Food.com dataset into three categories based on their ingredients, making techniques and analysing recipe’s preparation steps.  

We made a detailed study on datasets, using Logistic Regression, Support Vector Machine, Random Forest Classifier, Multi-layer Perceptron Classifier, XGBoost, LSTM and LSTM with GloVe word embedding models, and optimized them by tuning and adjusting various hyperparameters and model structures. 

We also compared the performance between different models and different features. In conclusion, the Logistic Regression model has the best performance on techniques and ingredients features with 0.5145 F1 score, and the LSTM with GloVe word embedding model performs best on steps features with 0.50118 F1 score.  

Our result is very helpful for the platforms to use recipes information provided by users to create value.

## Doc.

[Article](https://github.com/Gilone/Healthy-Diet-is-All-You-Need/blob/main/Healthy%20Diet%20is%20All%20You%20Need.pdf)  
[Overleaf](https://www.overleaf.com/project/61a6d99bab117381be5813ae)  

## F1 Score Result

| features                           | LR     | RF     | MLP     | XGB    | GradientBoostingClassifier | LSTM| LSTM + GloVe | LSTM + trainable GloVe |
| ---------------------------------- | ------ | ------ | ------ | ------ | -------------------------- |---|---|---|
| Techniques                         | 0.3781 |0.3636 | 0.4081 |0.4079| 0.3849                     | |||
| Ingredients_ids(500)               | 0.4796 |0.3512 |0.4305 |0.4156 |0.4312                    ||||
| Ingredients_ids(1000)              | 0.5073 |0.3474 |0.4477 |0.4178 |0.4336                     ||||
| Techniques + Ingredients_ids(1000) |  0.5145| 0.3583 |0.4538 |0.4308 |0.4491                  ||||
| Glove Ingredients                  | 0.4661 |0.3842 |0.4997 |0.4301 |0.5023                     ||||
| Steps                  |  |   |  |  |                     | 0.47708 | 0.50118 | 0.50048 |


## Ref.

- [Original paper of Prof.](https://github.com/majumderb/recipe-personalization)
