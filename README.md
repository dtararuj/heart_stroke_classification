# heart_stroke_classification
Attempt to predict heart stroke by using models from sklearn and using keras

In this case we have dataset with 5110 patient records, but only 5% of them diagnosed as a heart attack.

The best results we achived using sofisticated method to replicate data (SMOTE) for minority class and neural network, built with:

- 2 dense layers with 1024 and 256 units,
- dropout layer (rate 0.1) and batchnormalization after each dense layer,
- dense layer with 2 units and softmax activation layer as an output,
- binary_crossentropy loss function,
- Adam Optimizer with learning rate = 0.0001

Our model results is:

88% accuracy in general,
93% precision for class 0 (No heart attack) and 83% for class 1,
81% recall for class 0 and 94% of class 1

Our results tell us that final model can detect 83% of heart attacks, classifing correctly each patient with symphtoms as a potential heart attack with 94% probability (recall).
Kaggle competition worksheet (link)[https://www.kaggle.com/tararuj4/heart-stroke-classific-87-acc-with-keras-pl]
