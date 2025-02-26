# PatternRecognition-SVM-Model-for-Weather-Classification-Project

Project Overview:
This project involves several key steps and image processing, specifically focusing on image classification, feature extraction, dimensionality reduction, and model evaluation. The code makes use of several popular Python libraries such as numpy, scikit-learn, opencv, and matplotlib to process the data and apply various machine learning algorithms.

Data Preparation:

The dataset is first loaded from a .zip file. A check is performed to ensure that the file has been extracted successfully. If the file has already been extracted, the program informs the user. This process is handled by the zipfile and os libraries.
The dataset is split into training and testing sets, where each class of images is placed into separate folders.
Image Preprocessing:

The images are resized and converted to grayscale using the opencv (OpenCV) and skimage libraries. The preprocessing also includes the application of CLAHE (Contrast Limited Adaptive Histogram Equalization) to enhance the contrast of the images.
Feature extraction is performed using SIFT (Scale-Invariant Feature Transform), which identifies key points and extracts descriptors. These features are later used in the classification model.
Dimensionality Reduction using PCA:

Principal Component Analysis (PCA) is applied to reduce the dimensionality of the image data. This helps in capturing the most important features while reducing the complexity of the data.
The covariance matrix is computed, and eigenvectors and eigenvalues are derived. The top eigenvectors are then used to transform the data into a lower-dimensional space.
Feature Selection:

Sequential Feature Selection (SFS) is used to select the most relevant features for classification. This helps in improving the model's efficiency by reducing the number of features without losing important information.
Model Training and Evaluation:

The final model is trained using a Support Vector Machine (SVM) classifier. The training process uses the selected features to build the model.
After training, the model is tested using the test set, and the results are evaluated. The performance is measured using a confusion matrix and accuracy metrics.
Visualization:

The confusion matrix is visualized using matplotlib, providing an intuitive way to understand the classification performance. The matrix shows which classes were predicted correctly and which were misclassified.
