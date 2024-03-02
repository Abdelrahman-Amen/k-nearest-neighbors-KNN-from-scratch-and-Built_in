# k-nearest-neighbor 🚀

# Introduction to k-Nearest Neighbors (KNN)

k-Nearest Neighbors (KNN) is a simple yet powerful supervised machine learning algorithm used for both classification and regression tasks. It is a non-parametric and instance-based method, meaning it doesn't make assumptions about the underlying data distribution and learns directly from the training instances.


![Screenshot 2024-03-02 150910imagw](https://github.com/Abdelrahman-Amen/k-nearest-neighbors-KNN-from-scratch-and-Built_in/assets/103226865/63efa6ef-e765-4345-820e-ffdb5c6dbb8c)
# Principle
KNN operates based on the principle that similar instances are likely to belong to the same class or have similar properties. It classifies a new data point by identifying the majority class among its k nearest neighbors in the feature space.

![Screenshot 2024-03-02 150925image](https://github.com/Abdelrahman-Amen/k-nearest-neighbors-KNN-from-scratch-and-Built_in/assets/103226865/b1ab4ca3-5d79-4404-ab47-4f1181bf165d)

# steps to make KNN:


1. Choose the Value of K: Determine the value of K, which represents the number of nearest neighbors to consider. Typically, you can use techniques such as cross-validation to select the optimal K value.

2. Calculate Distance: For each data point in the test set, calculate its distance to all data points in the training set. Common distance metrics include Euclidean distance, Manhattan distance, Minkowski distance, or cosine similarity.

Euclidean distance:


![Screenshot 2024-03-02 150854euc](https://github.com/Abdelrahman-Amen/k-nearest-neighbors-KNN-from-scratch-and-Built_in/assets/103226865/b810f505-99fb-4b44-b519-2f840d8dc34a)

Manhattan distance:


![Screenshot 2024-03-02 150814MD](https://github.com/Abdelrahman-Amen/k-nearest-neighbors-KNN-from-scratch-and-Built_in/assets/103226865/2b1d1fd6-08bd-4af7-a8fa-223fd35748e0)

Minkowski distance:


![Screenshot 2024-03-02 151022minc](https://github.com/Abdelrahman-Amen/k-nearest-neighbors-KNN-from-scratch-and-Built_in/assets/103226865/d6e25b88-d771-4577-927f-fe48293c13b8)

cosine similarity:


![Screenshot 2024-03-02 150839cosi](https://github.com/Abdelrahman-Amen/k-nearest-neighbors-KNN-from-scratch-and-Built_in/assets/103226865/f1c9602a-ea5b-457a-b82e-195924c562e6)

3. Find K Nearest Neighbors: Select the K data points from the training set that are closest to the test data point based on the calculated distances.

4. Majority Vote (Classification) or Weighted Average (Regression): For classification problems, assign the class label that is most frequent among the K nearest neighbors. For regression problems, compute the weighted average of the target values of the K nearest neighbors, where the weights are inversely proportional to the distance.

5. Make Predictions: Use the majority class or the computed average to make predictions for the test data points.

6. Evaluate the Model: Assess the performance of the KNN model using evaluation metrics such as accuracy, precision, recall, F1-score (for classification), or Mean Squared Error, Mean Absolute Error, R-squared (for regression).

7. Tune Hyperparameters: Fine-tune hyperparameters such as the value of K or the choice of distance metric based on the model's performance on the validation set.
