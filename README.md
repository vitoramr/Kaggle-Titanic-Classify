# Kaggle - Titanic Challenge
## Machine Learning from Disaster

This project is inpired in the [Titanic - Machine Learning from Disaster](https://www.kaggle.com/c/titanic/overview) Kaggle Challenge to use data to predict whether a person that was in the Titanic survived or not to the disaster.

This is a well-known Kaggle challenge for begginners, and there is plenty of material available to learn and to improve your project. I worked in this project with the purpose of applying my new knowledge of Machine Learning and Neural Networks. With the material I found online I could learn new tools of the pandas, scipy and Scikit-Learn libraries.

The different programs try different approaches to the problem and achieve different accuracies.

## Data format
The challenge data can be found [here](https://www.kaggle.com/c/titanic/data) and it consists of the following features

* *survival* : 1 if the person survived, 0 otherwise. It is the variable to be predicted
* *pclass*: Descbribes the ticket class. It is a proxy for socio-economic status (SES)
  * 1st = Upper
  * 2nd = Middle
  * 3rd = Lower
* *age*: Age is fractional if less than 1. If the age is estimated, is it in the form of xx.5
* *sibsp*: The dataset defines the number of siblings/spouses aboard the Titanic family relations in this way:
  * Sibling = brother, sister, stepbrother, stepsister
  * Spouse = husband, wife (mistresses and fiancés were ignored)
* *parch*: The dataset defines the number of parents/children aboard the Titanic family relations in this way:
  * Parent = mother, father
  * Child = daughter, son, stepdaughter, stepson
  * Some children travelled only with a nanny, therefore parch=0 for them.
* *ticket* : Ticket number
* *fare* : Passenger fare
* *cabin* : Cabin number
* *embarked* : Port of Embarkation
  * C = Cherbourg, Q = Queenstown, S = Southampton

## Models

* Titanic 1
  * Model: RandomForestClassifier from Sckit-learn
  * Features: Sex and Age to predict the model
  * Accuracy of 0.71291
* Titanic 4
  * Model: Testing over 8 different prediction models
  * More deep data analysis and Features engineering
  * Hyperparameters tuning with sklearn.model_selection.SRandomizedSearchCV
  * The best model was RandomForestClassifier
  * Accuracy of 0.78947

## Acknowledgements

Special thanks to the article [Predicting the Survival of Titanic Passengers](https://towardsdatascience.com/predicting-the-survival-of-titanic-passengers-30870ccc7e8) by [Niklas Donges](https://towardsdatascience.com/@n.donges) for providing clear explanations and insights to the problem. Special thanks also to the YouTube channel [Mario Filho - Data Science](https://www.youtube.com/channel/UCIFd_i2iwYox1PPm9rD8wFA) for the challenge tutorial and introduction to Kaggle.
