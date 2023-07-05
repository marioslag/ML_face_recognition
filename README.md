# ML_face_recognition
ML for face recognition project
# Face Recognition using Eigenfaces and SVMs

This project implements the Eigenfaces method for face recognition, which combines Principal Component Analysis (PCA) for feature extraction and the nearest neighbor classifier for face identification. The goal is to evaluate the algorithm's ability to handle variations in lighting conditions between the training set and the test set of face images from the Yale B face database.

## Dataset
The face images used in this project are from the Yale B face database, which contains 10 subjects captured under 64 different lighting conditions. The dataset can be found in the "faces.zip" file in the Documents directory on eclass.

## Eigenfaces Method
The Eigenfaces method for face recognition involves three main steps:

1. **Step 1: Preprocessing and PCA**: Each face image in the training set, with dimensions 50 x 50 pixels, is converted into a column vector of 2500 elements and stored in the training data matrix X. Principal Component Analysis (PCA) is then applied to X to extract the d principal components (eigenvectors). These eigenvectors, when represented as images, are referred to as Eigenfaces.

2. **Step 2: Projection onto Eigenspace**: The images from the training and test sets are projected onto the d-dimensional eigenspace, resulting in low-dimensional features. The low-dimensional space with dimension d is called the eigenspace.

3. **Step 3: Face Identification**: Face recognition is performed in the eigenspace using the nearest neighbor classifier with the Euclidean distance as the metric.

## Project Tasks
The project consists of two main tasks:

### Task 1: Face Recognition using Eigenfaces
1. Implement the `loadImages(path, set_number)` function, which takes the path to the image folder and the set number as input and returns a data matrix, where each image is represented as a column vector. The function should also return the corresponding labels encoded as integers.
2. Train the Eigenfaces method using d = 9 and d = 30 on the Set_1 images (70 images) and evaluate the face recognition accuracy on Set_1 to Set_5. Report the classification accuracy for each set and each value of d. Discuss the generalization capability of the Eigenfaces method across different sets.
3. Visualize the 9 top eigenvectors (eigenfaces) obtained after training the Eigenfaces method on Set_1. Analyze the observations and discuss what the different eigenvectors might represent.
4. Reconstruct a random image from each of the 5 sets using d = 9 and d = 30 Eigenfaces obtained from Set_1. Display both the original images and their reconstructed versions for different values of d. Comment on the quality of image reconstruction for each image.

### Task 2: Image Classification using SVMs
In this task, you are required to explore the use of Support Vector Machines (SVMs) for image classification. The details and requirements for this task are not provided in the question prompt. Please refer to the assignment materials or additional instructions to complete this task.

## Implementation and Dependencies
You can choose to implement the project using your preferred programming language and libraries. It is recommended to use libraries or functions that provide PCA functionality or eigenanalysis (e.g., eigenvectors computation) to simplify the implementation.

The following dependencies are suggested:
- Programming language: Python
- Libraries: NumPy, OpenCV, scikit-learn

Please ensure that the required datasets and image files are available in the appropriate directories.

## Running the Code
To run the code, please follow these steps:
1. Set up the necessary dependencies, including Python, NumPy, OpenCV, and scikit-learn.
2. Download and extract the face dataset from the

.
