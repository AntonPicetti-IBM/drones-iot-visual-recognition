# Survey wildfire-damaged neighborhoods to identify burned homes and intact homes

 Use drone aerial images, Watson Studio, and Watson Visual Recognition to survey damage.

## Introduction

This hands on lab uses drone aerial images, Watson Studio and Watson Visual Recognition to survey wildfire damaged neighborhoods and identify burned homes and intact homes.

![Watson Studio screenshot](screenshots/WatsonStudio-VisualRecognitionModelTestResults.png)

## Learning objectives

After completing this tutorial you will be able to:

- Create a Visual Recognition model in Watson Studio running in IBM Cloud

- Capture images from a drone and zip them into a class

- Train a model to identify objects in the images

- Score and count the identified objects

## Prerequisites

This tutorial can be completed using an IBM Cloud Lite account.

- Create an [IBM Cloud account](https://console.bluemix.net/registration)

- Log into [IBM Cloud](https://console.bluemix.net/login)

## Estimated time

You can complete this task in no more than 15 minutes.

## Step 1 - Learn about Drones

There are many types of drones available that range from toys to industrial use cases. Many of the drones now include a camera that can store or stream aerial video to the ground. Using the livestream video frames, we can sample frames and send the images to Watson Visual Recognition for classification.

- Pocket toy drones

  - [Contixo F8](http://www.contixo.com/products/Contixo-F8-Foldable-Pocket-Size-Selfie-Drone-Voice-Controls-720P-HD-Wifi-Live-FPV-Video-Camera-360-Stunts-8-10min-Fly-Time-Gravity-Control-Red_308.html)

- Tello - Control a [Tello Drone using Node-RED](https://github.com/johnwalicki/Node-RED-Tello-Control)

- Hobbyist drones

- Commercial drones

## Step 2 - Capturing Images

One of the fun experiences of flying a drone is capturing video or pictures from a unique aerial perspective. You can use your drone to capture images of interesting objects that you want to train a visual recognition model to autonomously identify.

In this lab, we have created three zip files of pictures recorded by drones. The lab will use these images to identify neighborhoods affected by the devastating 2018 West Coast wildfires. These images will be used as our training set.

- Aerial drone images of burned homes - [BurnedHomes.zip](https://github.com/AntonPicetti-IBM/drones-iot-visual-recognition/raw/master/WildFires/classes/BurnedHomes.zip)

- Aerial drone images of intact homes - [AerialHomes.zip](https://github.com/AntonPicetti-IBM/drones-iot-visual-recognition/raw/master/WildFires/classes/AerialHomes.zip)

- Aerial drone images of forests, roads, rivers to be used for the negative class. [NotHomes.zip](https://github.com/AntonPicetti-IBM/drones-iot-visual-recognition/raw/master/WildFires/classes/NotHomes.zip)

*Source attribution: USA Today [article](https://www.usatoday.com/in-depth/news/nation-now/2018/08/02/drone-aerials-california-wildfire-devastation/889885002/), various internet sources*
