# 2. General Description

This section will give an overview of the whole system. The system will be explained in its context to show how the system interacts with other systems and introduce the basic functionality of it. It will also describe what type of stakeholders that will use the system and what functionality s avaliable for each type. At last, the constraints and assumptions for the system will be presented.

## 2.1 Product perspective

This system will consist of two parts: one mobile application and one web application. Both mobile and web application will share the same static and dynamic content as well as one shared SQL database. 

[![Architecture Block Diagram](../images/block1.png)](../images/block1.png)
###### Figure 1. Architecure Block Diagram

As stated, both mobile and web application will used shared static and dynamic content and all the information distributed through the application will be stored in the same database. As presented in the Figure 1 above. All the load will be shared between mobile and web application.
Information will be provided through the front end of the application by users and administrators. Application is scalable and autoscaling is used as responsiveness of the application to be displayed on all device sizes. 

The information is stored in shared SQL database. After the changes are made in the database itself through execusion of the task queries.
Task Queues provide a mechanism to offload longer running tasks to backend servers, freeing the front end servers to service new user requests. Application should provide real time content as fast as possible and as accurate as possible through communication with the database.

Memcache is an in-memory cache shared across the instances. This provides extremely high speed access to information cached by the web server (e.g. authentication or account information).

