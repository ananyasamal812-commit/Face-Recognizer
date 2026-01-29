# Face-Recognizer
Face Recognition System developed using Python, OpenCV with MySQL used for storing user details.
The system can:
Capture face images using a webcam

Train a face recognition model using LBPH (Local Binary Pattern Histogram)

Recognize known faces in real-time

Provide a GUI for user interaction

Store user details (name, age, address, etc.) in a MySQL database

---------------------------------------------------------------------------------------------------

# Features

 Real-time face detection using Haar Cascade

 Face recognition using LBPH algorithm

 Automatic dataset generation

 Model training and saving (classifier.xml)

 MySQL database integration for storing user information

 Recognition of known users and labeling as UNKNOWN if not matched
 
 --------------------------------------------------------------------------------------------------

 # Technologies Used

 Python

 OpenCV

 MySQL

 Libraries:

opencv-python

opencv-contrib-python

numpy

Pillow

mysql-connector-python

---------------------------------------------------------------------------------------------------------


# How It Works

1.Dataset Generation

Webcam captures face images

Faces are detected using Haar Cascade

Cropped grayscale images are saved in the data/ folder

2️. Training the Model

Images are loaded from the dataset

LBPH Face Recognizer is trained

Trained model is saved as classifier.xml

3️. Face Recognition

Live webcam feed is processed

Faces are detected and predicted

If confidence > 75%, the person’s name is displayed

Otherwise, the face is labeled UNKNOWN

4️. GUI Interface

Enter user details (Name, Age, Address, etc.)

Buttons provided for:

Generate Dataset

Train Model

Detect Face

Data is stored in MySQL when submitted

------------------------------------------------------------------------------------------

# How to Run the Project

1.Install Dependencies

pip install opencv-python opencv-contrib-python numpy pillow mysql-connector-python


2.Start MySQL Server

Create database python_database

Create table my_table

3.Generate Dataset

Click Generate Dataset button

Capture face images via webcam

4.Train Model

Click Training button

Model is saved as classifier.xml

5.Recognize Face

Click Detect the face

Webcam starts recognizing known faces

------------------------------------------------------------------------------------------
# Output

Recognized faces are labeled with stored names

Unknown faces are marked as UNKNOWN

User details are saved in MySQL database

Real-time face detection window opens via webcam

