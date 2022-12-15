# Rock, Paper, Scissors Identifier 
The following program is designed to train a machine learning model for it to be able to identify the hand positions corresponding to rock, paper or scissors. Premade [Mediapipe Hand Landmark](https://google.github.io/mediapipe/solutions/hands) pipeline is used to obtain the lankmark points of the hand. Then data is normalized and fed into a Support Vector Machine (SVM) model. The model is then saved and used to predict the hand gesture in real-time.

## Recommended resources
- [Google Mediapipes](https://google.github.io/mediapipe)
- [Support Vector Machine](https://scikit-learn.org/stable/modules/svm.html)
- [Learn SVM with Programming Knowledge](https://www.youtube.com/watch?v=zEabrO9l1vg&ab_channel=ProgrammingKnowledge)

## Support Vector Machine
A Support Vector Machine (SVM) is a supervised ML model that can be used for classification or regression problems. It is a powerful model that can be used for both linear and non-linear problems. It is a binary classifier, which means it can only classify two classes. To classify more than two classes, we can use the One-vs-Rest method, which is a technique that trains multiple binary classifiers and then uses a voting system to classify the data.

## How it works
As the model gets fed data about the determined hand landmarks at a certain position, it normalizes the distances between each landmark to determine its gesture. For instance, if the fingertips are the furthest from the wrist, it means the hand is making a Paper gesture. 