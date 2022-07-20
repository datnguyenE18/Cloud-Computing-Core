# **Cloud Native Applications**





- **a cloud native application** is 
  - an application developed from the outset to work only in the cloud environment, 
  - or an existing app that has been refactored and reconfigured with cloud native principles



- A cloud native application consists of microservices working together as a whole to comprise an application
![image](https://user-images.githubusercontent.com/43572616/180047850-6cd385ea-09d2-45cb-8c33-49cfc76734a8.png)



  Each can be independently scaled and iterated through automation and orchestration processes
![image](https://user-images.githubusercontent.com/43572616/180047903-accb5619-0b5e-4b62-b857-bd6620995239.png)



  These microservices are often packaged in containers, which are executable units of software in which the application code is packaged along with its libraries and dependencies so that it can be run anywhere. 
![image](https://user-images.githubusercontent.com/43572616/180047952-f81aa17d-c4ba-4afd-862d-3c698099a3dc.png)



![image](https://user-images.githubusercontent.com/43572616/180047984-ad496429-d8ab-4592-b85b-2e3f6c63b51c.png)



- **Development principles:**
  - Follow the microservices architectural approach by breaking applications down to single-function microservices
 
  - Rely on containers for maximum flexibility, scalability, and portability
 
  - Adopt Agile methods (speed the creation and improvement process through quick iterative updates based on user feedback)

***

**Diagrams**

|designed, built, and delivered|Application Code| |
| :- | :- | :- |
| |Application Runtime|middleware|
|all about backing services, and being able to integrate our application code with existing services that may be available on other clouds, or even on-premise. |Application + Data Services| |
| |Scheduling & Orchestration|[k8s] all about control planes, like kubernetes|
|private,  public and enterprise infrastructure|Cloud / Infrastructure| |


- A runtime environment encompasses a range of platforms, frameworks and technologies. In basic terms, the application runtime environment is a configuration of hardware and software necessary for that application code to execute -- any operation or behavior that is not directly attributable to the work of the application
 
- Container orchestration automates the scheduling, deployment, networking, scaling, health monitoring, and management of containers. Containers are complete applications; each one packaging the necessary application code, libraries, dependencies, and system tools to run on a variety of platforms and infrastructure

  Container Orchestration là tất cả việc quản lý vòng đời của container, đặc biệt là trong môi trường lớn, năng động
 
- Kubernetes (also known as k8s or “kube”) is an open source container orchestration platform that automates many of the manual processes involved in deploying, managing, and scaling containerized applications
