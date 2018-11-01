.. _terminology:

*******************************
Xi IoT Concepts and Terminology
*******************************

Before getting started with the lab itself, it's a good idea to get familiar with Xi IoT concepts & terminology.

Category
--------

A category is a logical grouping of edges, data sources & other items.

Cloud Connector
---------------

Built-in Xi IoT platform feature to publish data to a public cloud like Amazon Web Services or Google Cloud Platform.

Requires a customer-owned secured public cloud account and configuration in the Xi IoT management console.

Cloud Profile
-------------

Cloud provider service account (Amazon Web Services, Google Cloud Platform, and so on) where acquired data is transmitted for further processing.

Container Registry Profile
--------------------------

Credentials and location of the Docker container registry hosted on a cloud provider service account. Can also be an existing cloud profile.

Data Service
------------

Cloud hosted data infrastructure such as AWS Simple Queue Service, Azure, or Google Pub/Sub.

Data Source
-----------

A collection of sensors, gateways, or other input devices to associate with an edge. Enables you to manage and monitor sensor integration and connectivity.

Data Pipeline
-------------

Path for data that includes input, processing, and output blocks. Enables you to process and transform captured data for further consumption or processing.

- Input - An existing data stream or data source, identified according to a Category
- Processing | Transformation - Code block such as a script to process or transform input data. Scripts are available in the Scripts library or can be uploaded to the library.
- Output - Publish data to the cloud or cloud data service (such as AWS Simple Queue Service) at the edge.

Edge or Edge Device
-------------------

1. Any location (hospital, parking lot, retail store, oil rig, factory floor, and so on) where sensors or other input devices are installed and collecting data. Typical sensors measure (temperature, pressure, audio, and so on) or stream (for example, an IP-connected video camera). An edge minimally consists of an edge device and a data source.
2. Cluster or device providing the Xi IoT infrastructure (consisting of a full software stack combined with a hardware device). It enables customers to deploy intelligent applications (powered by AI/artificial intelligence) to process and transform data ingested by sensors. This data can be published selectively to public clouds. Also known as an Edge Device.

Infrastructure Administrator
----------------------------

User who creates and administers most aspects of Xi IoT. The infrastructure administrator provisions physical resources, edges, data sources and public cloud profiles. This administrator allocates these resources by creating projects and assigning project users to them.

Project
-------

A collection of infrastructure (edge, data source, project users) plus code and data (applications, data streams, scripts, runtime environments), created by the infrastructure administrator for use by project users.

Project User
------------

User who views and uses projects created by the infrastructure administrator. This user can view everything that an infrastructure administrator assigns to a project. Project users can utilize physical resources, as well as deploy and monitor data streams and applications. This user has project-specific CRUD permissions: the project user can create, read, update, and delete assigned applications, scripts, data streams, and other project users.

Functions
---------

Code used to perform one or more tasks. Script languages include Python, Golang, and Node.js. A script can be as simple as text processing code or it could be advanced code implement AI using popular machine learning frameworks like Tensorflow or Caffe.

Runtime Environments
--------------------

Command execution environment such as Kubernetes Service to run Docker applications.

Xi IoT
------

Nutanix Software as a Service (SaaS) based management platform and cloud IoT services. Includes the Xi IoT management console.

Xi Edge
-------

Intelligent edge Platform as a Service (PaaS).

Xi IoT Management Console
-------------------------

Browser-based console where you can manage the Edge infrastructure, depending on your role (infrastructure administrator or project user).