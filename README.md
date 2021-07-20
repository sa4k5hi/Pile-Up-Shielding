# Project Description
Driving a car is a complex task, and it requires complete attention. Distracted driving is any activity that takes away the driver’s attention from the road. Several studies have identified three main types of distraction: visual distractions (driver’s eyes off the road), manual distractions (driver’s hands off the wheel) and cognitive distractions (driver’s mind off the driving task). The National Highway Traffic Safety Administration (NHTSA) reported that 36,750 people died in motor vehicle crashes on an average, and 12% of it was due to distracted driving. Many states now have laws against texting, talking on a cell phone, and other distractions while driving. We believe that computer vision can augment the efforts of the governments to prevent accidents caused by distracted driving. Our algorithm automatically detects the distracted activity of the drivers and alerts them. We envision this type of product being embedded in cars to prevent accidents due to distracted driving.This project aims to recognize unsafe behaviour and send real time feedback to the driver using short sound alert etc.This system can be used to classify the behaviour of a driver via live video feed.The system uses various python libraries for extracting features in the training phase of the warning system

## Proposed Solution
To overcome the problem we came up with the solution implemented using OpenCV, DLib and other open source libraries . Python is used as a language to implement the idea. A web camera is used to continuously track the facial landmark and movement of eyes and lips of the driver. This project mainly targets the landmarks of lips and eyes of the driver. Fordetection of drowsiness, landmarks of eyes are tracked continuously. If the driver is found to be distracted then a voice (audio) alert is provided and a message is displayed on the screen. Following use cases are covered in this project

1. If the eyes of drivers are closed for a threshold period of time then it is considered that the driver is feeling sleepy and a corresponding audio alarm is used to make the driver aware.

2. If the mouth of the driver remains open for a certain period of time then it is considered that the driver is yawning and corresponding suggestions are provided to the driver to overcome drowsiness.

3. If the driver doesn't keep eyes on the road then it is observed using facial landmarks and the corresponding alarm is used to make the driver aware.

All this functionality is then implemented with the help of python libraries, an espeak compact open source software is used to produce alert sound.

Simple code in python to detect Drowsiness and Yawn and alert the user using Dlib.

## Dependencies

 1. Python 3
 2. opencv (tested with 3.4)
 3. dlib (tested with 19.18.0)
 4. imutils (tested with 0.5.3)
 5. scipy
 6. numpy
 7. argparse

## Run

    Python3 drowsiness_yawn.py -- webcam 0		//For external webcam, use the webcam number accordingly

## Setups

    EYE_AR_THRESH = 0.3
    EYE_AR_CONSEC_FRAMES = 30
    YAWN_THRESH = 10`	//change this according to the distance from the camera

