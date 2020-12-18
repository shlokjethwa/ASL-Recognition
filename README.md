# ASL Based Hand Gesture Recognition using Convolution Neural Network(CNN)
For the ASL Gesture recognition we have 44 gesture samples and for each gesture sample we have 1200 images. Each of the images is of 50*50 pixels and is stored in the gestures
folder. Each of these images is in grayscale and we have also flipped them in the python file so that we can increase the accuracy of detection and so now for each gesture we 
have 2400 images.

## Start running the ASL-Detection.ipynb file for recognizing the characters that you make gestures of using ASL 

### Step 1 - Setting up the histogram 
For the first step we are setting our hand histogram and so we need to fit our hand within the green boxes appearing on the screen. For this once we see that our hand is covering
all the green boxes then we can press the button 'c' for capturing our hand color and so after that we would be able to see the skin color in white and the rest in black in a new
window. Once we see that our hand is properly detected then we can press 's' for stopping the detection and saving the hand color.

### Step 2 - Flipping the images
Here we flip the images on the vertical axis for better accuracy of the prediction of the alphabet. 

### Step 3 - Loading the images
Now comes the turn of loading the images and so we are loading all the gestures that we have in the dataset and using pickle for searching. The pickle module is used for serializing
and deserializing the python object structures. And this is the process that converts all the images into binary. This process is known as pickling, serialization, or flattening. 

### Step 4 - Shuffle
Here we shuffle all the images and since the images are in a multiple of 12 so we have the training dataset as the 10/12 of the whole dataset, testing dataset as the 1/12 and 
validation dataset as the 1/12 of the dataset. 

### Step 5 - Display gestures
We display all the gestures here. And for each gesture we choose randomly one image for display.

### Step 6 - Training
In this step we are implementing 10 epochs and for each we have a patch size of 500. The training is done using Keras.

### Step 7 - Model report
Here we are displaying the confusion matrix of the model. Along with that we also get the f scores, precision, recall for the predictions by the model. 

### Step 8 - Testing
This is the step where we recognize the gesture that we are making in the ASL in the form of alphabet and we achieved an accuracy of 99%. 
