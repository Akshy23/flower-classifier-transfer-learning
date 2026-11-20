# Flower Classification with Transfer Learning

An image classification project that recognizes five types of flowers using TensorFlow/Keras and transfer learning.

## Project overview

This project uses MobileNetV2, a CNN pretrained on ImageNet. The pretrained layers are frozen, and a new classification head is trained to identify the flower categories.

The notebook covers:

- Loading and splitting image data into training and validation sets
- Resizing images and applying random horizontal flips
- Building and training the transfer learning model
- Plotting training and validation accuracy and loss
- Viewing sample predictions

## Dataset

The project uses TensorFlow’s flower photos dataset, which contains 3,670 images across five classes:

- Daisy
- Dandelion
- Roses
- Sunflowers
- Tulips

The notebook downloads and extracts the dataset automatically. You don’t need to upload the images separately. See the [TensorFlow dataset guide](https://www.tensorflow.org/tutorials/load_data/images) for the dataset source and image attribution information.

## Model and tools

- **Model:** MobileNetV2 pretrained on ImageNet, with a new five-class output layer
- **Training:** 5 epochs; pretrained base layers frozen
- **Tools:** Python, TensorFlow/Keras, NumPy, Matplotlib, Google Colab

## Results

| Metric | Result |
| --- | ---: |
| Training accuracy after epoch 5 | 91.59% |
| Validation accuracy after epoch 5 | 89.78% |
| Validation loss after epoch 5 | 0.3025 |

These are results on the validation split, not a separate test set.

## Run the notebook

Open `cnn_flower_transfer_learning.ipynb` in Google Colab, connect to a runtime, and run the cells in order. The notebook downloads the dataset when needed.

## Learning note

This is a learning project built to practice CNNs and transfer learning. The model is a demonstration and has not been evaluated for real-world use.
