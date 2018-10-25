.. _intro:

------------
Introduction
------------

From the Xi IoT product page ...

**Part of the Nutanix Xi family, Xi IoT is an internet of things and edge computing platform that simplifies edge computing and cloud infrastructure management, enabling users to quickly build and deploy intelligent applications across a public or private cloud infrastructure. Xi IoT consists of Xi Edge, an application infrastructure, project and administrator users, and cloud and data pipelines to help converge edge and cloud data.**

-------------------------------
Simplify IoT and Edge Computing
-------------------------------

And now consider this statement:

**In 2017, 3 billion enterprise IoT edge devices generated over 30 times more data (256 ZB) than the 30+ million nodes across cloud and private data centers. The classic IoT model of ingesting massive amounts of data on edge devices and processing data in the cloud, leads to several IT challenges such as bandwidth congestion, lack of scalability, processing delays, compliance and privacy issues.**

With that in mind, Nutanix has introduced a new product - Xi IoT_.  The Xi IoT platform delivers local compute, machine learning and intelligence for your IoT edge devices.

Of course, Nutanix Xi IoT has been developed to deliver the experience you've come to expect from Nutanix: a delightful application development platform.

By eliminating complexity we can accelerate deployments and elevate developers to focus on the business logic so critical for the success of IoT applications and services.

--------
This lab
--------

Today's lab is broken into two parts.

Part 1 will focus on following a tutorial-style set of steps that will end with a functioning Xi IoT application.  The application that you'll be deploying makes use of a live video stream published via RTSP.  This RTSP stream is processed by the various parts of the Xi IoT platform and allows a custom application to "do stuff" with the results.  We'll get to the "do stuff" part shortly!

Estimated time to complete: **120 minutes**

During part 1, you will configure the following Xi IoT components.

- The edge device itself has been pre-staged but you will add it to your Xi IoT profile.
- Configure a data source based on an RTSP-capable IP camera.
- Add the Data Type category that will logically group your edges (just 1, for this lab)
- Create a connection to the container registry that holds our sample/demo application
- Add Functions (analogous to Scripts, for the purposes of this lab).  Functions act as "steps" in the Data Pipeline.
- Create the Data Pipeline that will process the data from our camera data source.
- Add an application that acts as the front-end for the processed data.
- Finally, test the deployed application to make sure it does what it is supposed.

In part 2 of the lab, you will use a physical edge device to create an application of your own.

A selection of pre-tested runtime environments (models) have been provided for the lab.  This will ensure the best chance of success while creating your own application.

With those high-level steps outlined, let's start part 1.

.. _IoT: https://www.nutanix.com/products/iot/