# TITANIC SURVIVAL CLASSIFICATION
## TASK:
To predict whether a person will survive the titanic crash given a set of features.

##DATASET:
* The training dataset can be downloaded [here](https://storage.googleapis.com/tf-datasets/titanic/train.csv).
* The testing dataset can be downloaded [here](https://storage.googleapis.com/tf-datasets/titanic/eval.csv)

## FEATURES:
|FEATURES                        |DESCRIPTION                                 |
|               ---              |               ---                          |
|* SEX                           |  Male or female                            |  
|* AGE                           |  Age of the person                         |
|* N_SIBLINGS_SPOUSES            |  Siblings and spouses on board             |
|* PARCH                         |  Parents on board                          |
|* FARE                          |  Price of the ticket to board the ship     |
|* CLASS                         |  First or Second or Third class            |
|* DECK                          |  The location of his/her cabin             |
|* EMBARK_TOWN                   |  The town from which they boarded the ship | 
|* ALONE                         |  Whether the person was alone or not.      |

## LABEL:
* Given the above features we have to predict whether a person survived or not.
* survived(1) and didnt survive(0)

## FEATURE SELECTION

* We have to remove the features that doesnt add value.
* We have to remove the features like EMBARK_TOWN as it is immaterial where a person boarded the ship
* We can add the features N_SIBLINGS_SPOUSES and PARCH since they are nearly the same.

## MODELS USED:
* Logistic Regression
* Decision Tree
* Support Vector Machine
* Random Forest
* Boosting(using decision tree)
* MLP Classfier

## MODEL SELECTION:
 
* Random Forest was selcted as the best model based on the F1_score.
* One drawback of Random Forest is that it is a bit slow
* If our aim is for faster training of the model, we can select the Decison Tree
* Decision Tree provides a good F1_score while the time taken to train is fastet than that of Random Forest.



