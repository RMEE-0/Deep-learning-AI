Explanation:

* Installs PyTorch, TorchVision, and Torchaudio (optional in Colab since PyTorch is often pre-installed).
* Imports necessary libraries for model building, optimization, datasets, preprocessing, and data loading.
* Uses GPU if available, otherwise CPU, and prints the device being used.
* Downloads the MNIST dataset (handwritten digits) and applies preprocessing: converts images to tensors and normalizes them.
* Creates training and testing data loaders with batch size of 64.
* Defines a simple neural network (SimpleNN) with three fully connected layers: 784 → 128 → 64 → 10, using ReLU activation and flattening 28x28 images into 784-length vectors.
* Uses CrossEntropyLoss for classification and the Adam optimizer with a learning rate of 0.001.
* Trains the model for 5 epochs: moves data to the device, computes outputs, calculates loss, backpropagates, and updates weights. Prints average loss per epoch.
* Evaluates the model on the test set, computing predictions and overall accuracy.
* Optionally saves the trained model as mnist_model.pth for later use or further training.
