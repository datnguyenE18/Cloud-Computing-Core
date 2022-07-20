# **Microservices**



- Microservices architecture is an approach in which a single application is composed of many loosely coupled and independently deployable, smaller components or services (These services typically have their own stack running on their own containers)

![image](https://user-images.githubusercontent.com/43572616/180046290-2a9b138b-072a-4881-99bb-75c3df3a5297.png)


- These services communicate with one another over a combination of 
  - APIs, 
  - Event streaming
  - Message brokers

![image](https://user-images.githubusercontent.com/43572616/180046314-85b476e0-f1b1-4a07-a7b6-3e1ca31548e1.png)



- **Meaning:**
  - Application components can be developed and updated more efficiently by multiple developers working independently
 
  - Teams can use different stacks and runtime environments for different components
 
  - Components facing too much load can be scaled independently, reducing the waste and cost associated with having to scale entire applications
 
- **Detail:**
  - In the past, software was built as large monolithic applications where a team of developers would take months to construct a large application built on a common code base (write every part of the application from start to finish)
 
  - after decades of software development, there are vast amounts of code already out there that developers can use as the base of an application (they no longer have to create every line of code from scratch)
 
  - Now, instead of building one huge application on one team, developers break into small independent teams where they write smaller amounts of code called **microservices**
 
- Microservices breakdown large applications into their core functions, for example, search, recommendations, customer ratings, or product catalogs. 

  Each is developed independently of one another, yet work together on the cloud development platform to create a functioning application
 
- A container is the distribution method for each microservice (it delivers the code where it needs to go)

![image](https://user-images.githubusercontent.com/43572616/180046343-1c5d3bd2-8365-4f3d-841d-3c69cb1901d4.png)



![image](https://user-images.githubusercontent.com/43572616/180046365-e03fa93b-4085-4f8a-aa6c-d6641808790b.png)



![image](https://user-images.githubusercontent.com/43572616/180046379-90b0fba3-7390-4dba-8db9-7f4df3979f54.png)



![image](https://user-images.githubusercontent.com/43572616/180046398-54b7b569-318e-4bd9-bd37-f46ccb58a129.png)



- Containers are plug-and-play, so if one microservice isn’t working for an application, developers can take it out and put in a different one without disrupting how the rest of the app functions
