# Edge Impulse Image Classification Model for OpenMV H7
This repository contains an image classification model for pedistrian detection trained using Edge Impulse for deployment on the OpenMV H7 board. The model allows the OpenMV H7 to classify persons or zebra crossing as no person captured by its camera.

# Requirements
* OpenMV H7 board
* OpenMV IDE or similar software for uploading the code
* Edge Impulse account

# Getting Started

* Perpare dataset for this project by combine the given two datasets. Use the dataset one as person class and dataset two as no person class.
** Gender classification dataset by combining as 1 class
** https://www.kaggle.com/datasets/dataclusterlabs/zebra-crossing

* Sign up for an account on the Edge Impulse platform at https://www.edgeimpulse.com/ if you haven't already.
* Create a new project in Edge Impulse and choose the "Image" data type.
* Upload The dataset to Edge Impulse, labeling each image with the appropriate class.
* Preprocess the image to genrate the features for training.
* Configure and train the model in Edge Impulse. Choose the desired model architecture (e.g., MobileNetV1, MobileNetV2, ResNet-50) and set the hyperparameters accordingly.
* Evaluate the trained model's performance using the testing dataset in Edge Impulse.
* Export the trained model from Edge Impulse. Select the "OpenMV H7" library deployment option.
* Connect The OpenMV H7 board to your computer.
* If you insert a micro-sd card into the micro-sd card slot on your OpenMV Cam the micro-sd card will replace the internal flash drive for all of the above. The OpenMV Cam supports micro-sd cards up to 2 TB in size that are formatted with a FAT12, FAT16, FAT32, and ex-FAT filesystem. In particular, we support SD, SDHC, and SDXC micro-sd cards. Last, feel free to save pictures/video on a micro-sd card. Just don’t do this on your OpenMV Cam’s internal flash drive.
* In case Openmv H7 not switching the memory to micro-sd card please use the disk burn software for formatting and do not use the quick format.
* Open the OpenMV IDE (or a similar software) and upload the provided code or write your own code using the exported model.
* Copy the exported model and the lable file to openmv flash memory.
* Run the code on the OpenMV H7 board and observe the classification results.
