# CS3244 Project workflow

# Proposal to-do list


***

[Example 1](https://www.kaggle.com/code/abdallaellaithy/fashion-mnist-cnn-classifier)
## Preparation
1. Load clean dataset
2. Map integer labels to respective category EG 0: "T-shirt/top"
3. Visualise greyscale image by reshaping into 28x28 image
4. Normalise from 0-255 to 0-1 for better training performance - too big a range from  0 - 255 for different columns
5. Reshape data to fit CNN model

## Initial implementation
1. Encode labels using sk's LabelEncoder
2. Import test train split to split data

## Actual CNN model (example uses tensorflow and not pytorch)
1. Using keras package, define CNN model parameters (double check it is ReLU)
2. Compile model
3. Train model
4. Evaluate on test set
5. Plot training and validationa accuracy

## Notice mistakes were made despite high accuracy, address the generalisation
1. Data augmentation to help model learn more general patterns instead of memorising data sheet (overfitting)
2. Reduce learning rate to improve data generalisation
3. L2 Regularisation to reduce overfitting by penalising large weights
4. I'm not sure about using F1 score because the data might not be unbalanced? eg one class much more prevalent
5. Now we compile and train model with augmented data, plot accuracy etc

![Confusion Matrix looks like this](https://github.com/user-attachments/assets/8089d26a-cc76-4033-a017-0a1bae9a315c)

***

[Another decent example if we can read the format](https://www.kaggle.com/code/sunnyhoya/study05-fashion-mnist)
Many types of evaluation methods like Accuracy&Loss graphs, Confusion matrix, Confidence, and even Precision Recall F1 score below
