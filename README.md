# Realtime chat app


![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)

>[!NOTE]
>About the project

This is a simple study project to learn more about websocket protocol. In this project is created a realtime chat using basic websocket configuration with Java + SpringBoot and an index html file to see every functionality working. In html file was implemented a simple logic to distinct received and sent messages using javascript with stomp and pure css, with no frameworks. Basicly the project has two methods, add an user to enter in global chat and sending messages. 

>[!NOTE]
> How to run

1 - To run this project i created a dockerfile, so you can build the image and running this one without needing to have Java installed on your machine. But fisrt you need to clone this repository using: 
```bash
  git clone https://github.com/gabrielferreira02/Realtime-chat-app.git
```

2 - Then you need to generate jar application file
```bash
  mvn clean install
```

3 - Now you can build docker image and run the project
```bash
  docker build -t chatapp/v1 .
```

4 - Verify if docker image was created
```bash
  docker images
```

5 - Start the project
```bash
  docker run -p 8080:8080 chatapp/v1
```

6 - Access the application in 
```bash
http://localhost:8080
```
