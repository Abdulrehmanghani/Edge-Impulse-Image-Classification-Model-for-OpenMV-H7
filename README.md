# Edge Impulse Image Classification Model for OpenMV H7
This repository contains an image classification model for pedistrian detection trained using Edge Impulse for deployment on the OpenMV H7 board. The model allows the OpenMV H7 to classify persons or zebra crossing as no person captured by its camera.

# Requirements
* OpenMV H7 board
* OpenMV IDE or similar software for uploading the code
* Edge Impulse account

# Getting Started

Perpare dataset for this project by combine the given two datasets. Use the dataset one as person class and dataset two as no person class.

Sign up for an account on the Edge Impulse platform at https://www.edgeimpulse.com/ if you haven't already.

Create a new project in Edge Impulse and choose the "Image" data type.

Collect and prepare your dataset. You will need images for each class or category you want to classify. Ensure that the images are representative and cover a diverse range of examples. Preprocess your images as necessary (e.g., resize, crop, augment).

Upload your dataset to Edge Impulse, labeling each image with the appropriate class.

Configure and train the model in Edge Impulse. Choose the desired model architecture (e.g., MobileNetV1, MobileNetV2, ResNet-50) and set the hyperparameters accordingly.

Evaluate the trained model's performance using the testing dataset in Edge Impulse.

Export the trained model from Edge Impulse. Select the "OpenMV H7" deployment option.

Connect your OpenMV H7 board to your computer.

Open the OpenMV IDE (or a similar software) and upload the provided code or write your own code using the exported model.

Run the code on the OpenMV H7 board and observe the classification results.
