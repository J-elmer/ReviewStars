# ReviewStars
![cover](https://user-images.githubusercontent.com/75163176/167580311-31988630-0a87-47d3-b098-22de4b9442f2.png)

Welcome to ReviewStars where you can see upcoming concerts and leave your reviews for concerts you have visited. 

This is an application build in order to experiment with how to set up several back end applications in Java [Spring Boot](https://spring.io/projects/spring-boot) and how to make sure data remains consistent between them. This application helped me to understand the concept of microservices a bit better. It is also my first application in which I built a [Angular](https://angular.io/) frontend. 

Here is a schematic overview of the application and how it is all connected:

![image](https://user-images.githubusercontent.com/75163176/167581524-06ab10cd-00bf-4ccb-8c32-6bc07dc75ded.png)

In building the Angular frontend, I used [Materialize](https://materializecss.com/) in order to get acquinted with that framework. In choosing the design of my page, I choose elements which I haven't used before. Not everything is perfectly implemented and the frontend could use some finetuning, but my main focus was learning for example how to add a search functionality, or how to effectively add modals. 

## Installation

*Prerequisites*

To run this application, an installation of [Docker](https://docker.io/) is required.

*Steps*

Clone this repository to your local machine by running:

```
git clone https://github.com/J-elmer/ReviewStars.git
```

Navigate to the directory in which you cloned this repository and run:

```
docker-compose up -d
```

Once the containers are running, navigate to http://localhost:4200 and you should see the app.


**Running on Linux? Extra steps**

When runnning on Linux, Docker resolves internal URL's through localhost instead of host.docker.internal. If you want to run the application on linux follow these extra steps:

- go the application folder
- open docker-compose.yml in an editor
- comment out line 20; comment in line 22
- comment out lines 47 and 48; comment in lines 50 and 51
- comment out line 85; comment in line 87

After you've updated the file, you can run docker-compose up -d


## Reviewing the code

If you are interested in the code of one of the microservices or the backend, please visit the individual repositories:

[Angular frontend](https://github.com/J-elmer/review-stars-frontend)

[Performer microservice](https://github.com/J-elmer/Performer-Microservice)

[Concert microservice](https://github.com/J-elmer/Concert-microservice)

[Review microservice](https://github.com/J-elmer/Review-microservice)
