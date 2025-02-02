# MNIST-Digits-Classification
This project demonstrates the implementation of a simple neural network using TensorFlow for classifying handwritten digits from the MNIST dataset. The model consists of a few key steps.

Data Loading and Preprocessing:

        The MNIST dataset is loaded and split into training and testing sets.
        The pixel values of the images are normalized by dividing by 255.0 to scale them between 0 and 1.

Model Architecture:

        A Sequential model is created with the following layers.
        Flatten: Converts the 28x28 pixel images into a 1D vector of size 784.
        Dense: A fully connected layer with 128 neurons and ReLU activation.
        Dropout: A dropout layer with a rate of 0.2 to prevent overfitting.
        Dense: A final fully connected layer with 10 neurons (for the 10 digit classes) and softmax activation for multi-class classification.

Loss Function and Compilation:

        The SparseCategoricalCrossentropy loss function is used for multi-class classification.
        The Adam optimizer is used to minimize the loss function.

Model Training:

        The model is trained on the training set for 5 epochs.

Model Evaluation:

        After training, the model is evaluated on the test set to assess its accuracy.

This project demonstrates how to build and train a basic neural network for image classification using TensorFlow and the MNIST dataset.
