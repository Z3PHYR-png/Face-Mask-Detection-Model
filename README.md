# Face-Mask-Detection

<h2>Brief Desciption of the project:</h2>

This project is made with the help of a dataset
downloaded from Kaggle.com.
The project detects and shows if a person is
wearing a face mask or not.
The dataset contains two types of images namely:
with_mask and without_mask.
The python program “train_mask_detector.py”
trains the model with the given dataset and
predicts the accuracy and loss of the model.
A plot is obtained showcasing the same. When the
“detect_mask_video.py” is executed, the web
camera app is launched and detects if the user is
wearing a mask or not. 

[ Code: https://github.com/balajisrinivas/Face-Mask-Detection/blob/master/train_mask_detector.py ]

Understanding the Face Mask Detection Algorithm:

There are given a dataset which is further divided into two
parts : one being a folder with approximately 1,910
images of people without mask and another folder
consisting people only with masks.

<strong><h2>Phases of training and applying the
algorithm to the model:</h2></strong>
In order to train a custom face mask detector, we need to
break our project into two distinct phases, each with its
own respective sub-steps


<br><strong>Training:</strong></br> Here we’ll focus on loading our face mask
detection dataset from disk, training a model (using
Keras/TensorFlow) on this dataset, and then serializing
the face mask detector to disk.


<br><strong>Deployment:</strong></br> Once the face mask detector is trained,
we can then move on to loading the mask detector,
performing face detection, and then classifying each face
as with_mask or without_mask


The dataset/ directory contains the data described in the
“Our face mask detection dataset” section.<br>
Three image examples/ are provided so that you can test
<br>Open terminal. <br>Go into the cloned project directory and
type the following command:<br>
<code>$ python3 train_mask_detector.py --dataset dataset</code>

<br>To detect face masks in an image type the following
command:
<br><code>$ python3 detect_mask_image.py --image
images/pic1.jpeg</code>

To detect face masks in real-time video streams type the
following command:

<code>$ python3 detect_mask_video.py </code>

the static image face mask detector.

Three Python scripts in this project are being used :

train_mask_detector.py: Accepts our input dataset
and fine-tunes MobileNetV2 upon it to create our
mask_detector.model.

A training history plot.png containing accuracy/loss
curves is also produced.

detect_mask_image.py: Performs face mask detection in static images

detect_mask_video.py: Using your webcam, this script
applies face mask detection to every frame in the stream

<h2>Installation</h2>

<p>We will be using VS Code and Windows Terminal for importing,
training and testing the data.</p>

1.Clone the repo:
<code>
$ git clone
https://github.com/balajisrinivas/FaceMask-Detection.git
</code>

2.Change your directory to the cloned repo:
<code>
$ cd Face-Mask-Detection
</code>

3.Create a Python virtual environment named 'test'
and activate it:
<code>$ virtualenv test</code><br>
<code>$ source test/bin/activate</code>

4.Now, run the following command in your
Terminal/Command Prompt to install the libraries
required:
<code>
$ pip3 install -r requirements.txt</code>
