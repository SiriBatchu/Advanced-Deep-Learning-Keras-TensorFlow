# Advanced-Deep-Learning-Keras-TensorFlow - Neural Networks

This repository contains a series of Colaboratory notebooks demonstrating a comprehensive range of advanced deep learning concepts using TensorFlow and Keras.

# Part 1 : Data Augmentation and Generalization Techniques

This part explores various methods to improve the generalization of deep learning models by augmenting training data and applying regularization techniques.

1-a) L1 and L2 Regularization 

Description: Demonstrates how to apply L1 and L2 regularization to the kernel weights of dense layers in Keras.

Colab : https://colab.research.google.com/drive/1JnlGXTziquIps84i4Z5ms1b1JaPdpqFq

Execution in Colab: Train these models and compare their performance (loss, accuracy) on a validation set to a baseline model without regularization. Observe how L1 tends to drive weights to zero (sparsity), while L2 penalizes large weights.

1-b) Dropout 

Description: Illustrates the use of dropout layers to prevent overfitting.

Colab : https://colab.research.google.com/drive/1DdH8i_egV9DCiDAPVvV4wbAVLXhGXIty

Execution in Colab: Train this model and compare its validation performance to a model without dropout. Dropout should help reduce overfitting.

1-c) Early Stopping 

Description: Shows how to use the EarlyStopping callback to halt training when validation loss stops improving.

Colab : https://colab.research.google.com/drive/1aGBYzOsLCUCh74pg71cyfJvgjBD8BD4D

Execution in Colab: Run the training and observe when the EarlyStopping callback triggers. The restore_best_weights=True argument will ensure that the model with the best validation performance is used.

1-d) Monte Carlo Dropout 

Description: Demonstrates how to use dropout at inference time to get a distribution of predictions, which can be useful for uncertainty estimation.

Colab : https://colab.research.google.com/drive/1UxQ-iLrIqH2fFZQPhoN4991dZfZN5nHh

Execution in Colab: Run the code and observe the mean and standard deviation of the predictions. Higher standard deviation indicates higher uncertainty.

1-e) Various Initializations 

Description: Shows how to use different weight initialization strategies in Keras layers and when to use them (e.g., glorot_normal, he_normal, lecun_normal).

Colab : https://colab.research.google.com/drive/1WY-S46FR_0NWR6b1a66M2qjjg6WtGZrt

Execution in Colab: Train these models and compare their training curves (loss and accuracy) to see how different initializations affect learning.

1-f) Batch Normalization 

Description: Demonstrates the use of batch normalization layers to stabilize training and potentially improve generalization.

Colab : https://colab.research.google.com/drive/15_aNlpnSS_3ZrqFHsmPxHu9cP6r-iNjy

Execution in Colab: Train this model and compare its training speed and validation performance to a model without batch normalization. Batch normalization often allows for higher learning rates and faster convergence.

1-g) Custom Dropout, Custom Regularization 

Description: Shows how to create custom dropout layers (e.g., based on activation) and custom regularization techniques by implementing custom layer classes.

Colab : https://colab.research.google.com/drive/18hlZLFXgow5q3pHTCd4PY86GU4lZnI10

Execution in Colab: Implement and train these models. Observe how the custom dropout behaves based on activation values and how the custom activity regularizer penalizes large activations.

1-h) Using Callbacks and TensorBoard 

Description: Demonstrates how to use Keras callbacks like ModelCheckpoint, EarlyStopping, and TensorBoard for monitoring and controlling the training process. (Reference: Hands-On ML3 - Chapter 10)

Colab : https://colab.research.google.com/drive/1p-D1dHDVhVi6KcDKZyof3wJWse65DgX3

Execution in Colab: Run the training with TensorBoard callbacks and then use the %tensorboard magic command to view the logs.

1-i) Using Keras Tuner 

Description: Shows how to use Keras Tuner to perform hyperparameter optimization. (Hint: Hands-On ML3 - Chapter 11, TensorFlow.org)

Colab : https://colab.research.google.com/drive/1SPvzlXFHwOWmojMYgYWdgikg7wBaswOY

Execution in Colab: Run the Keras Tuner search. Observe the different hyperparameter combinations tried and the resulting validation accuracies. The best hyperparameters and the corresponding model will be printed.

1-j) Using KerasCV Data Augmentation 

Description: Demonstrates how to use the data augmentation layers provided by KerasCV. (Reference: KerasCV Documentation)

Colab : https://colab.research.google.com/drive/1d3jdIwNvn3N4NMiFCeyy0vexECckngc_

Execution in Colab: Explore and apply various KerasCV augmentation layers to image data and observe the results. Train a model with and without KerasCV augmentation to see the impact on performance.

1-k) Data Augmentation for Multiple Data Types 

Description: This notebook explores data augmentation techniques for different data modalities, including image, video, text (using libraries like nlpaug), and potentially time series or tabular data (using libraries like tsaug or custom methods). (References: Data Augmentation Review, AugLy, TensorFlow Image Augmentation)

Colab : https://colab.research.google.com/drive/1xFumJPvNPQi6kPJwXIZeB1oHLPxQQDvg

Execution in Colab: Run the code to apply augmentation techniques to sample data from different modalities and observe the transformed data. Train separate models with and without augmentation for each data type to compare performance.

1-l) Demonstrating Fastai Data Augmentation 

Description: This notebook demonstrates the data augmentation capabilities of the Fastai library. (Hint: Fastbook - Chapter 7)

Colab : https://colab.research.google.com/drive/1EBxncB6OSp4dqFya6gkPRwi3IDBFxDP-

Execution in Colab: Load image data and use Fastai's ImageDataLoaders and aug_transforms to visualize augmented images. Train a model using Fastai's data augmentation pipeline and observe its performance.


# Part 2 : Advanced Keras Deep Learning Constructs

Dive deep into internal Keras customization using your own layers, training loops, metrics, losses, and more.This covers OneCycle LR scheduler, custom dropout (MC Alpha), normalization layers, TensorBoard logging, custom loss/activation/initializer, metrics/layers, residual models, and custom training loop.

Colab : https://colab.research.google.com/drive/1zOMMF90Qy1_vu9r0gOgzp_7ezsd2W211

Youtube : https://youtu.be/bxP4N4WVofQ
