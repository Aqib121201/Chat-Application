
#  Chat-Application: Real-Time Messaging System using Spring Boot & WebSockets

An academic-grade real-time chat platform using **Spring Boot**, **WebSockets**, and **Thymeleaf**. This project demonstrates protocol-level messaging, concurrency handling, and full-stack integration through Java and front-end web technologies.

[![Java](https://img.shields.io/badge/Java-17-blue)](https://www.oracle.com/java/)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.0-green)](https://spring.io/projects/spring-boot)
[![WebSocket](https://img.shields.io/badge/WebSocket-Enabled-lightgrey)](https://developer.mozilla.org/en-US/docs/Web/API/WebSockets_API)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

##  Abstract

This project implements a full-stack chat application using Java Spring Boot with real-time messaging powered by WebSockets. It simulates the core infrastructure of a scalable chat backend, incorporating session-aware message routing and broadcast architecture. The UI is lightweight, built with HTML, CSS, and JavaScript via Thymeleaf. This system demonstrates backend engineering principles, real-time protocols, and concurrency mechanisms.

---

##  Academic Motivation

- Apply WebSocket protocol for bidirectional real-time communication  
- Explore event-driven design in a stateless HTTP world  
- Demonstrate backend fluency in Spring Boot and concurrent systems  
- Build full-stack production-grade applications for AI-era messaging platforms  

---

##  Features

-  Real-time WebSocket-based chat
-  Session-based user messaging
-  STOMP protocol over WebSockets
-  Front-end templated with Thymeleaf
-  Modular Spring Boot architecture

---

##  System Architecture

```text
[ Browser ]
     ⇅  JavaScript WebSocket
[ Spring Boot WebSocketConfig ]
     ⇅  STOMP Controller
[ Simple Message Broker ]
````

---

##  Project Structure

```text
ChatApplication/
├── src/
│   ├── main/
│   │   ├── java/com/example/chat/
│   │   │   ├── config/           # WebSocket config
│   │   │   ├── controller/       # STOMP message handler
│   │   │   └── model/            # Message DTO
│   │   └── resources/
│   │       ├── static/           # JS/CSS
│   │       ├── templates/        # Thymeleaf HTML
│   │       └── application.properties
├── pom.xml                       # Maven build file
├── mvnw / mvnw.cmd               # Maven wrapper
├── HELP.md
└── README.md
```

---

##  How to Run

###  Prerequisites

* Java 17+
* Maven 3.6+
* Chrome or Firefox browser

###  Setup

```bash
# Step 1: Clone the repository
git clone https://github.com/Aqib121201/Chat-Application.git
cd Chat-Application-main/ChatApplication

# Step 2: Build the project
./mvnw clean install

# Step 3: Run the application
./mvnw spring-boot:run
```

---

##  Access the App

Open your browser and go to:

```
http://localhost:8080
```

Use multiple browser windows or tabs to simulate live users chatting in real-time.

---

##  Testing & Usage

* Open in multiple tabs or browsers
* Enter a username when prompted
* Send a message — all other sessions receive it instantly

---

##  Tech Stack

| Layer    | Technologies                     |
| -------- | -------------------------------- |
| Frontend | HTML, CSS, JavaScript, Thymeleaf |
| Backend  | Spring Boot, WebSocket, STOMP    |
| Protocol | STOMP over WebSocket + SockJS    |
| Build    | Maven                            |

---

##  Future Improvements

*  Add Spring Security (JWT/session)
*  Persist messages in PostgreSQL
*  Implement 1:1 private chats
*  Responsive mobile layout
*  Docker support for deployment

---

## � License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).

---

##  Acknowledgements

* Spring Boot documentation
* Baeldung & Java Brains tutorials
* STOMP & SockJS community libraries

---

##  Citation

```bibtex
@software{chatapp2024,
  title     = {Chat-Application: Real-Time Messaging with Spring Boot & WebSockets},
  author    = {Aqib Siddiqui},
  year      = {2024},
  url       = {https://github.com/Aqib121201/Chat-Application},
  note      = {Independent systems-level project using real-time WebSocket communication.},
}
```

