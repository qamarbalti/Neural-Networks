Iran University of Science and Technology
Faculty of Computer Engineering 
Artificial intelligence and robotics group 
Pattern Recognition project
Student Name: Qamar Abbas
Student ID: 402722135
First semester of 1402 - 1403
Comprehensive Report on RBF Network-Based Wine Classification 
Project
The project began with the loading of the Wine dataset from scikitlearn's library, containing various features related to wine properties. 
The dataset was split into training and test sets (80% and 20%, 
respectively) to facilitate model training and evaluation.
2. Data Preprocessing:
2.1 Standardization:
The feature data underwent standardization using the StandardScaler 
from scikit-learn. This process ensures that the data has a mean of 0 
and a standard deviation of 1, making it suitable for processing by the 
RBF network.
3.2 RBF Feature Calculation:
The RBF features were computed for both the training and test sets. 
The number of RBF centers and the scale parameter.
4. Logistic Regression:
4.1 Model Training:
A logistic regression classifier was employed, taking RBF features as 
input. The model was trained on the RBF features extracted from the 
training data.
4.2 Model Evaluation:
The trained classifier was used to make predictions on the test data. 
The accuracy of the model was calculated using the accuracy_score 
function from scikit-learn.
5. Results:
The accuracy of the implemented RBF network for wine classification 
was found to be 
38.89
%
38.89%. This accuracy represents the percentage of correctly classified 
instances in the test set.
6. Conclusion:
In conclusion, the project successfully implemented an RBF network for 
wine classification using logistic regression. The accuracy achieved 
provides insights into the model's predictive capabilities. Further 
enhancements and optimizations can be explored to improve the 
model's performance
Problem#3 
Self-Organizing Map (SOM) for Face Image Data

Libraries Used:
NumPy: For numerical operations.
Scikit-learn: Specifically, fetch_olivetti_faces for loading face image data.
Matplotlib: For data visualization.
MinMaxScaler: From Scikit-learn for data normalization.
Dataset:
The code uses the Olivetti Faces dataset, which is loaded using 
fetch_olivetti_faces() from Scikit-learn.
The face image data is then shuffled to introduce randomness.
Data Visualization:
Displays 25 randomly selected face images from the dataset in a 5x5 
grid using Matplotlib.
Data Normalization:
Uses MinMaxScaler from Scikit-learn to normalize the face image data 
to the range [0, 1]. This ensures that all features have the same scale.
Self-Organizing Map (SOM) Parameters:
Epochs: 500
Number of Neurons: 100
Learning Rate: 0.1
Input Dimension: The number of features in the normalized face image 
data.
SOM Initialization:
Initializes SOM weights randomly.
find_best_matching_unit Function:
Calculates the Euclidean distances between SOM weights and input 
data.
Returns the Best Matching Unit (BMU) coordinates.
Training the SOM:
The SOM is trained by iterating through the data points and updating 
weights.
Utilizes batch processing for efficiency.
For each epoch, the BMU is found for each data point, and the weights 
of the neighborhood are updated.
The learning rate is decayed in each epoch.
Visualizing the Learned SOM:
Finally, the code visualizes the learned SOM.
Creates a 10x10 grid of subplots and displays the SOM neurons as 
images.
Notes:
The code uses vectorized operations and batch processing to improve 
training efficiency.
Adjustments to parameters, such as batch size and SOM dimensions, 
can be made based on specific requirements.
LVQ3 Model Report
1. Dataset Information
The model was trained and evaluated on the Car Evaluation dataset. 
The dataset contains categorical features related to car attributes such 
as buying price, maintenance cost, number of doors, number of persons 
that can fit in the car, luggage boot size, and safety.
2. Data Preprocessing
Categorical features were encoded using Label Encoding.
The dataset was split into training and testing sets with a test size of 
20%.
3. LVQ3 Model Implementation
The Learning Vector Quantization 3 (LVQ3) model was implemented 
with the following key components:
Prototype Initialization: Prototypes were randomly selected from each 
class in the training set.
Finding Closest Prototype: The model finds the closest prototype for a 
given input using Euclidean distance.
Prototype Update: The prototype of the predicted class is updated 
based on the learning rate and the difference between the input and 
the prototype.
4. Model Training
The LVQ3 model was trained on the training set for a specified number 
of epochs (default: 100). During training, prototypes were updated 
based on the input samples, aiming to correctly classify them.
5. Model Evaluation
The model was evaluated on the test set, and the following metrics 
were computed:
Accuracy: The ratio of correctly predicted instances to the total 
instances.
6. Results
The LVQ3 model achieved an accuracy of [0.41040462427745666]% on the 
test set.
7. Confusion Matrix
A confusion matrix was generated to analyze the model's performance 
in detail. Each cell in the matrix represents the number of instances for 
each class
