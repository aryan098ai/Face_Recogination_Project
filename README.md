# Face Recognition Models: CNN, Siamese Network, and PCA with SVC

## Description
This repository demonstrates three different approaches for face recognition using the Labeled Faces in the Wild (LFW) dataset:
1) Convolutional Neural Network (CNN): A model for multi-class classification of faces.
2) Siamese Network: A deep learning model for verifying whether two images belong to the same person.
3) Principal Component Analysis (PCA) with Support Vector Classifier (SVC): A machine learning pipeline for dimensionality reduction and classification.



## Features
1. Dataset: The LFW dataset is used for training and evaluation.
2. CNN: Classifies faces into multiple categories based on identity.
3. Siamese Network: Predicts similarity between image pairs for verification tasks.
4. PCA + SVC: Reduces dimensionality of image data and performs classification with a support vector machine.

## Installation

Clone the repository:

git clone https://github.com/UGMR20230013/PROJECT_2.git

Install the required libraries:

pip install tensorflow scikit-learn numpy

## Models and Workflow
1. CNN: Face Classification
The CNN model is trained on grayscale face images to classify them into multiple identities.

i. Preprocessing: Images are normalized and resized.

ii. Architecture: Three convolutional layers followed by dense layers.

iii. Loss Function: Categorical Crossentropy.

iv. Evaluation Metric: Accuracy.


#### Usage:

python cnn_model.py

2. Siamese Network: Face Verification
The Siamese network uses a shared CNN base to compute similarity between image pairs.

i. Preprocessing: Pairs of images are created for training.

ii. Architecture: CNN with a contrastive loss function.

iii. Metric: Binary accuracy.


#### Usage:

python siamese_network.py


3. PCA + SVC: Dimensionality Reduction and Classification
Principal Component Analysis is used to reduce the dimensionality of flattened images, followed by training a Support Vector Classifier.

i. Dimensionality Reduction: PCA with 150 components.
  
ii. Classifier: SVM with an RBF kernel.

iii. Evaluation Metric: Accuracy.

#### Usage:

python pca_svc_pipeline.py

    
## Result

CNN	= ~45%

Siamese Network	= ~95% (Verification)

PCA + SVC = ~85%

## Dataset
The LFW dataset contains grayscale images of faces. Only identities with at least 70 images are included for training and testing.

i. Image Size: 50x37 pixels.

ii. Classes: Number of distinct people.
## Contributing

Contributions are welcome! Feel free to submit issues or pull requests to improve this repository.





## License

This project is licensed under the MIT License.
