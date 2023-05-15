# new_rep
ResNet50 Neural Network Architecture
NN image

Dataset
We have used brain tumor dataset posted by Jun Cheng on figshare.com.

This brain tumor dataset containing 3064 T1-weighted contrast-inhanced images from 233 patients with three kinds of brain tumor: meningioma (708 slices), glioma (1426 slices), and pituitary tumor (930 slices).

Modules
brain_tumor_dataset_preparation.ipynb - An IPython notebook that contains preparation and preprocessing of dataset for training, validation and testing.

torch_brain_tumor_classifier.ipynb - An IPython notebook that contains all the steps, processes and results of training, validating and testing our brain tumor classifier.

test.py - A python script which accepts path to an image as input, which then classifies the image into one of the three classes.

deploy.py - A python script integrated with Flask server, that starts the Web Interface on local server where user can upload MRI image of brain and get classification results.

Note: We have included few images for testing under test_images directory.

Running the classifier
Download the classifier model '.pt' file from this drive link and place it under a folder named 'models' in the same directory where the files of this repository are present.

Before running the programs, kindly install the requirements as given in Requirements section of this README.

Use the test.py script for running the script in Terminal, Powershell or Command Prompt.

python test.py
Use deploy.py script to access the classifier as an interactive web interface.

python deploy.py
Screenshots (Results & Web Interface)
Web Interface
Home Page
index

Classification Results via Web Interface
class 1

class 2

class 3

Classifier Evaluation
Loss Graph
Loss Metrics

Accuracy Graph
Accuracy Metrics

Confusion Matrix on Test set
Confusion Matrix

Requirements
Python 3 is required.

Computational Specifications
Project done using Google Colab with follwing specifications:

Ubuntu 18.04 64-bit OS
12 GB DDR4 RAM
16 GB NVidia Tesla P100 GPU
40 GB of Non-Persistent Storage
Library Requirements
We'll be using the following libraries to complete our classification problem:

Numpy - For linear algebra operations
Torch - Pytorch Deep Learning Framework
OS - To use Operating System methods
Random - To set random seed at specific places where random operations take place just so it happens the same way everytime it is executed
Pandas - To create DataFrame, CSV files, etc
Time - To perform date time operations
Seaborn - For sophisticated visualization
Pickle - To save and load binary files of our training data
Scikit-Learn - Machine learning framework. We have used this for evaluating our Classifier and for cross-validation split
Matplotlib - To visualize images, losses and accuracy
Google Colab Drive - To mount Google Drive so we can perform storage and loading operations using it (Only available on Google Colab)
The above mentioned libraries comes pre-installed and pre-configured with Google Colab.

Install the required libraries on your computer using the pip package manager.

For pip version 19.1 or above:

pip install -r requirements.txt --user
or

pip3 install -r requirements.txt --user
Pytorch
Follow the steps for installation given in the official website of Pytorch.

About
This project was done by Akshay Kumaar M. Paper is in progress. All the references papers have been included at the end of this repository's README.

References
Thanks to Vinoth Arjun for giving ideas for custom dataset class with different real-time augmentations.

License
Copyright 2020 Akshay Kumaar M

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.

Research Papers
Multi-grade brain tumor classification using deep CNN with extensive data augmentation

A Deep Learning-Based Framework for Automatic Brain Tumors Classification Using Transfer Learning

Deep Residual Learning for Image Recognition (ResNet)

Documentations
Pytorch
Future Scopes
Brain Tumor segmentation using GANs.
Brain Tumor detection using Object Detection for localization of tumor in a given MRI image of the brain.
Improve existing classification model and web interface
