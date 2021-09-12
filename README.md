# Unauthorized-person-detection-model

## Overview
This is an opensource library for CNN-based face detection in images. SIMD instructions are used to speed up the detection. You can enable AVX2 if you use Intel CPU or NEON for ARM. 
The authorized person’s name and details are stored in CSV format and then into the database.
In case of any unauthorized person's face is detected the image of the intruder along with time is stored in the database and warning signal is also given to alert the surrounding members in case of intrusion detection.

## Motivation
Assisted my undergraduate professor for his research work developing face detection model while working as IT professional. My passion to learn Machine learning was inherited in my college days and have presented a paper in an international conference. Due to high cost involved in implementing, the corrosion detection in pipelines using overhead drones the idea ended up as a theoretical concept.
Working in the project helped me to learn the basic algorithms of Machine learning and Neural network.

## Introduction
Face recognition without using CNN is done by using encoding method. Here we will find all of the faces in the given image and label them and then we will compare the input image with the encoded file. The face distance is calculated to find the image that matches with the input image. The best match is found using the image with the smallest face distance. The label of the original image is displayed to detect the face of the given input image. Face recognition using CNN and transfer learning method is done by using the concept of transfer learning and using the pre-trained weights of VGG16 architecture, we can save both our time and resources.

## Technical Aspect
In this technique the image is broken down into pixels of arrays. First the path directory of the image is given. Then the function looks through all the faces in the folder and returns the encoded faces. Only images stored in file format of .jpg and .png is acceptable. Thus, the figure 1 shows the keys and the values of the encoded image.
 
![image](https://user-images.githubusercontent.com/86893978/133006385-13a57f7c-8058-46a1-b7c7-1887590ee007.png)

Figure 1: Encoded values
 
 
![image](https://user-images.githubusercontent.com/86893978/133006428-c1ba65ff-b652-48b3-a5bf-3aaf3dbb54bd.png)

Figure 2: Accuracy plot


![image](https://user-images.githubusercontent.com/86893978/133006433-361b6ca1-b15c-42ad-9540-5b7d1dd6832e.png)

Figure 3: Loss plot


![image](https://user-images.githubusercontent.com/86893978/133006441-35436047-9fc8-46e8-8957-7e776556c911.png)

Figure 4: Model prediction of an authorized person


![image](https://user-images.githubusercontent.com/86893978/133006446-be42f4b4-f8ec-4f78-b86b-424789b5b7b1.png)

Figure 5: Model prediction of an authorized person


![image](https://user-images.githubusercontent.com/86893978/133006451-af113477-40e5-4175-96f4-f4907f1946c5.png)

Figure 6: MYSQL Database


## Experimental Result
The final result of face recognition is shown in above figure from Figure 1 to Figure 6. 

Figure 1 shows the keys and the values of the encoded image

Figure 2 shows the accuracy plot we got accuracy percentage of 98.76

Figure 3 shows the loss plot we got a loss percentage of 9.79

Figure 4 and 5 represents the face recognition of person, that is If the person is authorized then it will display the face of an authorized person under the green colour rectangle, else it will display unknown person in red rectangle, 

Figure 6 shows how details are stored in the database.

## Installation
The Code is written in Python 3.7. If you don't have Python installed, you can find it [here](https://www.python.org/downloads/). If you are using a lower version of Python, you can upgrade using the pip package, ensuring you have the latest version of pip. To install the required packages and libraries, run this command in the project directory after [cloning](https://www.howtogeek.com/451360/how-to-clone-a-github-repository/) the repository:
> pip install -r requirements.txt

## Technologies used
•	Python
•	Tensorflow
•	SQL

## Team
Joseph – Assistant Professor, Anna University

## Credits
Google images- This project wouldn't have been possible without this tool. It saved enormous amount of time while collecting the data.

