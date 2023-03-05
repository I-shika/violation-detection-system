

## Problem Statement

#### To create a deep-learning based system to detect and store information of traffic violators in a database hosted on a website to collect proof and number plates of the criminals simultaneously.

## Mentors

### [Pranjal Mangal]
### [Maanas Verma]

## Contributors 

## [Ishika]
## [Rishika]
## [Divyanshu]
<br/>

## Technolegy used

<img align="left" width="26px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/django/django-plain.svg" style="padding-right:10px;" />
<img align="left"  width="26px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/opencv/opencv-original-wordmark.svg" style="padding-right:10px;" />
<img align="left"  width="35px" src="https://cdn.analyticsvidhya.com/wp-content/uploads/2018/12/yologo_2-850x451.png"  />
<br/>
<br/>

###

# Approach

#### 1) Learn Differnt Deep Learning and Computer Vision models

#### 2) As yolo was chosen for the project, do an in depth study of it's working and custom training 

#### 3)  Using Google and Kaggle images were collected

#### 4) Labeling of images was implemented using [labelImg](https://github.com/tzutalin/labelImg)

#### 5) Model was trained according to collected Data set 

#### 6) Made a Django based web interface to host the model

<br/>

# Solution

#### 1)Initial dataset consisted of 100 images which were expanded using image processing tecniques using OpenCV

#### 2) We used  [labelImg](https://github.com/tzutalin/labelImg) to gentrate labeled .txt file

#### 3) Seraching for proper training parameters was toughest part, after multiple experiments and advice for mentors we were able to fix parameters like learning rate,no of steps for training and much more

#### 4) Model training was done using google collab and data was acessed via google drive 

#### 5) Intial problems in the model were resoloved using better data sets, changing parameters

#### 6) After training of model with sufficent accurecy it had to host it on a website

#### 7) it was deployed on Django because it is written in python,OpenCv can used with Django and it has many inbuilt fetures to aid the process of integration and built the website




# Working

## Get API acess

#### Go to https://platerecognizer.com/ and get your credentials

#### Put them in webcam\views.py and add creditals in line 23
## Run the following commands


```
pip install -r requirements.txt

python manage.py createsuperuser (create a super user to acess admin page)   

python manage.py runserver
```
## After starting the server

#### Go to localhost:8000/admin 
#### in two wheeler upload image to be tested 

#### Go to localhost:8000/index/camera2 to run the test and see the object detection output

#### Go to localhost:8000/admin/webcam/crime2/ to view the crime result

<br/>



# Result

### A platform was successfully made to detect people on a two-wheeler and not wearing helmets , storing proof of the violation and the number plate of the vehicle.