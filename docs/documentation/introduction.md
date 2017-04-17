# 1. Introduction

This section gives a scope description and overview of everything included in this SRS document. Also, the purpose for this document is described and a list of abbreviations and definitions is provided.

## 1.1 Purpose 

The purpose of this document is to give a detailed description of the requirements for the "Giveaway" software. It will illustrate the purpose and complete declaration for the development of the system. It will also explain system constraints, interface and interactions with other external applications. 
This document is primarily intended to be proposed to a customer for its approval and a reference for developing the first version of the system for the development team.

## 1.2 Scope

The "Giveaway" is a web-based mobile application which creates a way for people to gift the things (clothes, shoes, coupons, gift cards, games...) they don't need or use anymore. All those things would go to people in need which are choosen based on the comment poll under each gift. Gifts are presented in the form of an image and a descroption. Anyone who would like to receive a certain gift leaves a comment with a reason why should they get it. The owner then pics the favorite comment and gift goes to that person. The application should be free to download from either a mobile phone application store or similar services. The application will also be avaliable as a web application.

The gift owners can provide their gift information using either the web or mobile application. This information will act as the bases for the search results displayed to the user. An administrator also uses the web application in order to administer the system and keep the information accurate. The administrator can, for instance, verify gift owners and manage user information.

Furthermore, the software needs both Internet, to fetch and display results, and access to your camera in case you want to publish a new giveaway. All system information is maintained in a database, which is located on a web-server. The application also has the capability of representing both summary and detailed information about the users. Security system is custom made as it uses the custom made tokens.

## 1.3 Definitions, acronyms, and abbreviations
###### Table 1. Definitions

| Term                | Description                                                                                                                                                   |
|---------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------|
| User                | A person who interacts with mobile/web application.                                                                                                           |
| Admin/Administrator | System administrator who is given specific permission for managing and controlling the system.                                                                |
| Giveaway            | Gift post created by users.                                                                                                                                   |
| Gift owner          | Someone who wants to create a giveaway and gift something to other users.                                                                                     |
| DB                  | Database - storage of all the system information.                                                                                                             |
| Application Store   | An installed application on mobile phone which helps user to find new compatible applications with mobile phone platform and download them from the Internet. |
| Stakeholder         | Any person who has interaction with the system who is not a developer.                                                                                        |
| DESC                | Description                                                                                                                                                   |
| FR                  | Functional Requirements                                                                                                                                       |
| NFR                 | Non-functional Requirements                                                                                                                                   |
| SD                  | Sequence Diagram                                                                                                                                              |
| SSD                 | System Sequence Diagram                                                                                                                                       |
| AVG                 | Average                                                                                                                                                       |
| EST                 | Estimate                                                                                                                                                      |

## 1.4 References

- [1] IEEE Software Engineering Standards Committee, "IEEE Std 830 - 1998, IEEE Recommended Practice for Software Requirements Specifications", October 20, 1998.
- [2] Software engineering - A Practitioner's Approach (Roger S. Pressman) 
- [3] Software engineering - Tenth Edition, Pearson Education, Ian Sommerville
- [4] Davis M. A., "Just Enough Requirements Management: Where Software Development Meets Marketing", New York, Dorset House Publishing, 2005. 
- [5] Karlsson J, "A Cost - Value Approach for Prioritizing Requirements", Norges Teknisk - Naturvitenskapelige Uni. 1997

## 1.5 Overview

The remainder of this document includes nine chapters. The second one provides an overview of the system functionality and system interaction with other systems. This chapter also introduces different types of stakeholders and their interaction with the system. Further, the chapter also mentions the system constraints and
assumptions about the product. The third chapter provides the requirements specification in detailed terms and a description of
the different system interfaces. Different specification techniques are used in order to specify the requirements more precisely for different audiences.
The fourth chapter deals with the prioritization of the requirements. It includes a motivation for the chosen prioritization methods and discusses why other alternatives were not chosen. The fifth and the sixth ones represent the deployment and architecture of the system itself, while the rest of the chapters are focused on the implementation and system design. This document also includes a master test plan.