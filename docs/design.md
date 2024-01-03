
---
geometry: margin=1in
---

# Moodsic Documentation

## Team Information

- Team members
  - Alfonso Blas-Pinto

## Executive Summary

Moodsic is a mindfullness app with the main goal of helping artists reach their artistry
by integrating ai with song selection depending on the user's prompt to 

### Purpose


### Glossary and Acronyms


| Term |          Definition           |
| ---- | ------------------------------|
| DAO  | Data Access Object            |
| MVP  | Minimal Viable Product        |
| MVVM | Model View View-Model         |
| OO   | Object Oriented               |
| REST | Representational Stat Transfer|
| SPA  | Single Page Application       |
| UML  | Unified Modeling Language     |
| Admin| A person who is in charge of administrative actions in the organization |


## Requirements

This section describes the features of the application.

. Cupboard / Need management
. All users can see upcoming and past events
. All users can see the needs 
. Admins can create, edit and delete the needs in an organization
. Admins can create, edit and delete events
. Volunteers and Admins can create, edit and purchase funding baskets of goods
. Minimal user authentication
. Users can create an account, login to their account and logout.
. Users can purchase the contents of a funding basket
. Admins can see a list of the needs that people want more of.
. Users can edit their account information.

### Definition of MVP



### MVP Features


### Enhancements


## Application Domain

This section describes the application domain.

![Domain Model Team 3](domain-model-team-3.png)

The domain model depicts a user that can add funds into the basket that holds donations.
The dashboard shows the events and volunteers, and users can login to view these events.
The dashboard also has graphs that show the data from the events. Our donations, baskets,
and events information is stored and can be changed and accessed by admins.


## Architecture and Design

This section describes the application architecture.

### Summary



### Overview of User Interface

> _Provide a summary of the application's user interface. Describe, from the user's perspective, the flow of the pages in the web application._

### View Tier

> _**[Sprint 4]** Provide a summary of the View Tier UI of your architecture.
> Describe the types of components in the tier and describe their
> responsibilities. This should be a narrative description, i.e. it has
> a flow or "story line" that the reader can follow._

  The View Tier UI in our architecture is a crucial layer that directly interacts with users, providing an interface for accessing and managing their needs. The Home Screen is the user's point of entry into our application.  The Navigation Bar acts as a guide through the application, ensuring users can effortlessly explore different sections, including their funding basket and needs. The Needs Dashboard takes center stage, presenting users with a visually appealing display of available needs. As users curate their selections, the Funding Basket component dynamically updates, providing a real-time summary of their chosen needs. Users can easily review, modify, or proceed to checkout directly from the Funding Basket. The User Profile component is clear and simple, ensuring users can easily update information or explore additional features.

> _**[Sprint 4]** You must provide at least **2 sequence diagrams** as is relevant to a particular aspects
> of the design that you are describing. (**For example**, in a shopping experience application you might create a
> sequence diagram of a customer searching for an item and adding to their cart.)
> As these can span multiple tiers, be sure to include an relevant HTTP requests from the client-side to the server-side
> to help illustrate the end-to-end flow._













> _**[Sprint 4]** To adequately show your system, you will need to present the **class diagrams** where relevant in your design. Some additional tips:_
>
> - _Class diagrams only apply to the **ViewModel** and **Model** Tier_
> - _A single class diagram of the entire system will not be effective. You may start with one, but will be need to break it down into smaller sections to account for requirements of each of the Tier static models below._
> - _Correct labeling of relationships with proper notation for the relationship type, multiplicities, and navigation information will be important._
> - _Include other details such as attributes and method signatures that you think are needed to support the level of detail in your discussion._

### ViewModel Tier

> _**[Sprint 4]** Provide a summary of this tier of your architecture. This
> section will follow the same instructions that are given for the View
> Tier above._

> _At appropriate places as part of this narrative provide **one** or more updated and **properly labeled**
> static models (UML class diagrams) with some details such as critical attributes and methods._
>
> ![Replace with your ViewModel Tier class diagram 1, etc.]()

### Model Tier

> _**[Sprint 2, 3 & 4]** Provide a summary of this tier of your architecture. This
> section will follow the same instructions that are given for the View
> Tier above._

The Model Tier is where all of the object classes are so we can create these objects to use in our controller and persistence classes. For example, these objects include our Events, Donations, User, Admin, etc. We can use the methods in these classes to get information, change information, and such.


> _At appropriate places as part of this narrative provide **one** or more updated and **properly labeled**
> static models (UML class diagrams) with some details such as critical attributes and methods._
>

![UML Diagram Model Tier]()

## OO Design Principles

> _**[Sprint 2, 3 & 4]** Will eventually address upto **4 key OO Principles** in your final design. Follow guidance in augmenting those completed in previous Sprints as indicated to you by instructor. Be sure to include any diagrams (or clearly refer to ones elsewhere in your Tier sections above) to support your claims._
 
> _**[Sprint 3 & 4]** OO Design Principles should span across **all tiers.**_

## Static Code Analysis/Future Design Improvements

> _**[Sprint 4]** With the results from the Static Code Analysis exercise,
> **Identify 3-4** areas within your code that have been flagged by the Static Code
> Analysis Tool (SonarQube) and provide your analysis and recommendations.  
> Include any relevant screenshot(s) with each area._

![Static Code Analysis]()

![Future Design Improvements]()

> _**[Sprint 4]** Discuss **future** refactoring and other design improvements your team would explore if the team had additional time._


## Testing

### Acceptance Testing

> _**[Sprint 2 & 4]** Report on the number of user stories that have passed all their
> acceptance criteria tests, the number that have some acceptance
> criteria tests failing, and the number of user stories that
> have not had any testing yet. Highlight the issues found during
> acceptance testing and if there are any concerns._
![Acceptance Testing Sprint 2 Dashboard Passed]()

![Acceptance Testing for Sprint 2 basic functions for Dashboard Passed]()

![Acceptance Criteria issues / Resolved Now]()


### Unit Testing and Code Coverage

- Our testing strategy throughout our project's lifetime has been straight forward. There should be tests written for any code
you implement. In our Java code we were aiming to stay well above 90% code coverage. We selected this target for a secure application.

[SPRINT 2] Code Coverage: 
 ![Sprint 2 Code_Coverage]()

In our recent review of the code coverage for the ufund-api, we've made noteworthy strides in certain areas that underscore the efficacy of our testing strategy:

    Controller Layer : We've achieved a commendable 83% instruction coverage in the com.ufund.api.ufundapi.controller package. This high percentage showcases our commitment to testing the routes and interactions that our users will experience, ensuring a reliable user interface.

    Model Layer Precision: The com.ufund.api.ufundapi.model package demonstrates near-perfect instruction coverage at 99%. This precision indicates our dedication to validating the integrity of the data structures which are fundamental to the robustness of our application.

    Application Layer: The com.ufund.api.ufundapi package boasts an outstanding 100% coverage, reflecting our thoroughness in testing the application's configuration and foundational components.

    Overall Coverage Strategy: Our approach has been to prioritize depth over breadth, focusing our testing efforts where they have the most significant impact. 