# FacialMapping

### Setup
In order to run this program and animate a rigged object, you will need an installation of blender as well as a couple of modules that we
will outline how to install in this section. In order to install these modules, you must first locate the python installation for blender. You
can do this by running the folling commands in the terminal of the scripting tab in blender:
<br />
<br />
*import sys
<br />
sys.path*
<br />
<br />
This gives the path to the installation of python for your blender enviroment. Naviate to the lib directory in the python folder and make sure
pip is installed. You can do this by running the following commands:
<br />
<br />
*python3.10 -m ensurepip
<br />
python3.10 -m pip install --upgrade pip --user* 
<br />
<br />
Once pip is installed you will need a the opencv, numpy, and dlib packages. Fun the following command to install these packages:
<br />
<br />
*python3 -m pip install opencv-python opencv-contrib-python imutils numpy dlib --user*
<br />
<br />
Once you import the python scripts using the open scripbutton on the top of the text editor window (icon of the file folder next to the name of the text file) and facial mapping predictor from the repo (you can save this file anywhere on the computer, just make sure you know its location), make sure the path for variable p in line 14 of 
*OpenCVAnimOperator.py* points to the *file shape_predictor_68_face_landmarks.dat* wherever you have it saved on your system. Then make sure the 
rig_name variable matches the name of your object in the scene graph.
<br />
**You are now ready to start animation using your webcam capture**
