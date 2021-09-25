# Dog-Breed-Classification-Udacity-Capstone-Project

## Project Overview
This project makes use of transfer learning with Convolutional Neural Network(CNNs) to identify various dog breeds. Transfer learning is a machine learning method where a model developed for a task is reused as the starting point for a model on a second task. In this scenerio, transfer learning was used with the pretrained weights of resnet50 to achieve better classification result on the dataset. The model is such that, when a user gives the input as a dog it classifies the breed it belongs to, and if it is fed with the image of an human, it detects it is an human and predict the dog breed the human resembles most, while input that are neither dog or humans are not classified.

### Table of Contents
- Libraries
- Description of files
- Insights

#### Libraries
The following are the libraries that was used in building the model
- Keras
- OpenCV
- Numpy
- Pandas
- Matplotlib

#### Description of files
- dog_app.ipynb - This is the notebook that contains the various steps in building the classification model
- dog_app.html - This is the html version of the notebook
- Haarcascades folder - This is the folder that contains the opencv face detector model
- Images - These are the various images used to perform inference on the model

#### Insights
- Without the use of transfer learning the model achieved an accuracy of 6.1005%
- With the use of transfer learning with resnet50, the model achieve an accuracy of 81.6986% on the test set with an epoch of 20.
- The accuracy of the model can further be improved by increasing the number of epochs or by adding more layers to the top of the resnet50 model to enable it to extract more features from the images.
- The model effectively classified all the dog breeds currectly
