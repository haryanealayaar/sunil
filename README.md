Face Recognition Project:-

This project demonstrates a face recognition system using Python and several popular machine learning libraries.

How it Works:

The system follows these steps:

1. Loads Face Images: It loads face images from a specified directory on your Google Drive.

2. Preprocesses Images: Each image is converted to grayscale and resized to a standard size (300x300 pixels). The image data is then flattened into a vector.

3. Applies PCA (Principal Component Analysis): This technique reduces the dimensionality of the image data while retaining the most important features (often called "eigenfaces").

4. Applies LDA (Linear Discriminant Analysis): This method further transforms the data to maximize the separation between different classes (individuals).

5. Trains an MLP Classifier: A Multi-Layer Perceptron (a type of neural network) is trained on the processed image data to learn to classify faces.

6. Evaluates the Model: The trained model is used to predict the identity of faces in a test set, and the accuracy of the predictions is calculated.

7. Visualizes Results: The project displays some of the test images along with their predicted and true identities and the confidence of the prediction.


* Requirements:
  
1. Python Libraries: matplotlib, sklearn, numpy, opencv-python

2. Google Colab (or a similar environment with Google Drive access)

3.A dataset of face images organized in folders, where each folder represents a different person.


* Setup:
  
1.Mount Google Drive: Run the provided code cell to mount your Google Drive.

2. Specify Dataset Path: Update the path and dir_name variables in the code to point to the location of your face image dataset on Google Drive.

3.Run the Notebook: Execute the code cells in order.


* Code Overview:
  
plot_gallery: A helper function to display images in a grid.

Data Loading and Preprocessing: Code to load images from your specified directory, 
resize them, and prepare them for the models.

Data Splitting: Splits the data into training and testing sets.

PCA and LDA: Applies dimensionality reduction techniques.

MLP Classifier: Trains the face recognition model.

Prediction and Evaluation: Makes predictions on the test set and calculates accuracy.

Result Visualization: Displays test images with predictions.

* Output:
  
The notebook will output:

The shapes of the processed data arrays.
The number of samples, features, and classes.
A gallery of the top "eigenfaces".
The loss during the MLP training process.
The accuracy of the face recognition model on the test set.
A gallery of test images with prediction results and probabilities.
