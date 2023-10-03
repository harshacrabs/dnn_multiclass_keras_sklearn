# dnn_multiclass_keras_sklearn


<h3>Overview</h3>
In this project, I aimed to predict whether the Apple Watch can correctly predict physical activity. I used a dataset that contained information on the physical activity of 16 participants.

I used several machine learning models to build a predictive model, and  evaluated them based on their F1-macro score. I selected this score because we assumed that both false positives and false negatives were equally expensive in this problem. Therefore, I needed a performance metric that would consider both precision and recall.

<h3>Data Preprocessing</h3>
I performed the following data preprocessing steps before building the models:

I resampled the data using the RandomOverSampler to balance the class distribution.
I split the data into training and testing sets using a 70-30 ratio.

<h3>Models</h3>
We built the following models:

<ul>
<li>Keras Neural Network without hyperparameter tuning</li>
<li>Keras Neural Network with hyperparameter tuning</li>
<li>Scikit-learn MLP Classifier with Random Search</li>
<li>Scikit-learn MLP Classifier with Grid Search</li>

</ul>


<h3>Results</h3>
The table below shows the F1-macro score of each model on the test data:

Model	F1-macro
| **Model** | **F1-Macro** |
| :---: | :---: |
| Keras NN | 12% |
| Keras NN with Hyperparameter Tuning | 52% |
| Scikit learn MLP Classifier with Random Search | 75%  |
| Scikit learn MLP Classifier with Grid Search | 78% |

Based on the results, we can conclude that the Scikit-learn MLP Classifier with Grid Search is the best model for this problem, as it has the highest F1-macro score on the test data.

Conclusion
In this project, we aimed to predict whether the Apple Watch can correctly predict physical activity. We built four models and evaluated them based on their F1-macro score. We selected the Scikit-learn MLP Classifier with Grid Search as the best model for this problem. The model had an F1-macro score of 53% on the test data.
