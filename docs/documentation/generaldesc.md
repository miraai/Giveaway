# 2. General Description

This section will give an overview of the whole system. The system will be explained in its context to show how the system interacts with other systems and introduce the basic functionality of it. It will also describe what type of stakeholders that will use the system and what functionality is avaliable for each type. At last, the constraints and assumptions for the system will be presented.

## 2.1 Product perspective

This system will consist of two parts: one mobile application and one web application. Both mobile and web application will share the same static and dynamic content as well as one shared SQL database. 

[![Architecture Block Diagram](../images/block1.png)](../images/block1.png)
###### Figure 1. Architecture Block Diagram

As stated, both mobile and web application will used shared static and dynamic content and all the information distributed through the application will be stored in the same database. As presented in the Figure 1 above. All the load will be shared between mobile and web application. Information will be provided through the front end of the application by users and administrators. Application is scalable and autoscaling is used as responsiveness of the application to be displayed on all device sizes. 

The information is stored in shared SQL database. After the changes are made in the database itself through execusion of the task queries.
Task Queues provide a mechanism to offload longer running tasks to backend servers, freeing the front end servers to service new user requests. The application should provide real time content as fast and accurate as possible through communication with the database.

Memcache is an in-memory cache shared across instances. This provides extremely high speed access to information cached by the web server (e.g. authentication or account information).

## 2.2 Product Functions

With the application, users will be able to create giveaways and receive ones. UUsers can create giveaways with the image of an item they want to gift to someone as well as a description of the chosen item. Users who want to receive a giveaway from someone leave a comment under the presented giveaway and a comment chosen by the gift owner will get the item.

Users can also search giveaways and users that are using the application. Users can see the News Feed that will provide all the content published by the users they are following and a Trending page where they will see all the trending giveaways currently ongoing.

The result of the search will be viewed either in a list view or in a profile view, depending on what criteria is included in the search. The list view will have one list item for each giveaway matching the search criteria and show a small part of the giveaway information so the user can identify the searched giveaway. 

## 2.3 User Characteristics

There are three types of users that interact with the system: users of the application, giveaway owners and administrators. Each of these three types of users have different uses of the system so each of them have their own requirements.

The application users can only use the application to find giveaways or users and create or edit their own profile. They can also create giveaways and become gift owners. This means that the users have to be able to search for giveaways, choose a giveaway from that search and then navigate to it. In order for the users to get a relevant search result there are multiple criteria the users can specify and all results matches all of those.

The giveaway owners will also be able to use both mobile and web application. From there they will manage the information about their giveaways, for example a description of the giveaway, contact information and their profile. They also can create new giveaways and search for one as well as search for the users of the application.

The administrators can also interact both with the mobile and web application.They are managing the overall system to ensure there is no incorrect information within it. The administrator can manage the information for each giveaway as well as the options for both the application users and the giveaway owners. 

## 2.4 Constraints

The application is constrained by the system interface to the navigation system within the application. Since there are multiple system manufacturers, the interface will likely not be the same for every one of them. Also, there may be a difference between what system features each of them provide.

The Internet connection is also a constraint for the application. Since the application fetches data from the database over the Internet, it is crucial that there is an Internet connection for the application to function. Both the web and the mobile application will be constrained by the capacity of the database. Since the database is shared between both application it may be forced to queue incoming requests and therefore increase the time it takes to fetch data.

## 2.5 Assumptions and Dependencies

One assumption about the product is that it will always be used on mobile phones that have enough performance. If the phone does not have enough hardware resources available for the application, for example the users might have allocated them with other applications, there may be scenarios where the application does not work as intended or even at all. 

Before the official release of the application there will be a list of minimal and recommended both hardware and software requirements.

## 2.6 Apportioning of Requirements

In the case that the project is delayed, there are some requirements that could be transferred to the next version of the application. 
