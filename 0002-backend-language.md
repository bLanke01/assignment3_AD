# 2 - Backend Language

* Status: accepted 
* Deciders: everyone 
* Template used: [MADR 3.0.0](https://adr.github.io/madr/) 


## Context and Problem Statement

* Determining which backend language is most suitable for music player functionalities. Attributes to consider include user authentication, library / playlist management, and song recommendations based on user preferences. 

## Considered Options

* Node.js 
* Python (Django) 
* Java (Spring Boot)  

## Decision Outcome

* The decision is made to develop a backend via Node.js and a NoSQL database (MongoDB).

## Rationale

* Node.js provides high performance and is the best fit for developing real-time applications like a music player application. 
* Node.js works well with NoSQL databases like MongoDB, allowing for flexible management of playlists. 
* JavaScript can be used for both front and back-end development, which can streamline the coding process and learning curve for developers.  

### Consequences 

* The single-threaded event loop of Node.js is less suited for complex / intensive data processing. 
* Rapid prototyping and production speed, as a large selection of libraries and frameworks are available for use. 
* I/O-bound task scalability – able to handle multiple requests simultaneously. 
* Less suitable for large-scale data transactions compared to Java. 

## Follow-Up Actions

* Identify the options of offloading CPU-intensive tasks to a third party. 
* Ensure frameworks / libraries / packages are all up to date and are free of any security or data vulnerabilities. 
* Regularly test and optimize organization of database for streamlined storage and retrieval of data. 