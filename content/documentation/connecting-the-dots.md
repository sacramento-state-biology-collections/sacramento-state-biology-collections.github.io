---
title: "What is the CSC 190/191 Project?"
date: 2022-10-19T00:21:03-07:00
draft: false
toc: false
---

The CSC 190/191 Project is a project-based course that teach's students how to work in a team to develop a software product. Software development process are practiced to create a software product that solves a real-world problem. The purpose of the course is to provide usefulness to the client and to provide a learning experience for the students.

## Understanding the Problem

At CSU, Sacramento there exists multiple collections ranging from mammals to herps. Each of these collections have existed for quite a long time at CSU, Sacramento but the information on every specimen was only available to some faculty and hardly any students. The problem is that the information stored on the collections differs between each collection and are stored in different places and some in even different formats.

## Understanding the requirements

- The system must be able to store information on the collections.
- The system must be low to no cost.
- The system must be able to be accessed by anyone with out a login.
- The system must be usable for CRUD operations on the collections data.
- The system CRUD functionality must be secure and only accessible to the correct users.
- The system must be stable and reliable for at least 5+ years.

## Understanding the constraints

### Low to no cost

lorem ipsum

### Accessible to anyone

lorem ipsum

### CRUD functionality

lorem ipsum

### Secure

lorem ipsum

## Understanding the risks

- The system may not be extensible to other organizations unless they have the same requirements.
- The system may not be integrable with a university's database login systems.

## Understanding the assumptions

- The system will be able to be used by anyone with out a login.
- The system will be able to be used by anyone with a login and a role.
- The system will be hosted on a university server with at least static site hosting.
- The system will be hosted on a university server with at least a database server.
- The system will be hosted on a server with accessability to setup self-healing and self-repairing systems.

## Reasoning the solutions and the tradeoffs

lorem ipsum

## Connecting the dots

### MVP

```goat
 Milestone 1 - MVP
-------------------
.-----------. .-----------------. .--------------. .---------.
|Static Site| |Search Engine PWA| |Service Worker| |Resources|
'-----------' '-----------------' '--------------' '---------'
      |               |                  |             |
      | Serve's Site  |                  |             |
      |-------------->|                  |             |
      |               |                  |             |
      |               |  GET DB Entries  |             |
      |               |----------------->|             |
      |               |                  |             |
      |               |                  |  SQL Query  |
      |               |                  |------------>|
      |               |                  |             |
      |               |                  |   Entries   |
      |               |                  |<------------|
      |               |                  |             |
      |               |     Entries      |             |
      |               |<-----------------|             |
      |               |                  |             |
.-----------. .-----------------. .--------------. .---------.
|Static Site| |Search Engine PWA| |Service Worker| |Resources|
'-----------' '-----------------' '--------------' '---------'
```

### Migration/Deployment of the system

```goat
 Milestone 2 - On-Prem Server
------------------------------
.-------------. .-----------------. .--------------. .---------.
|School Server| |Search Engine PWA| |Service Worker| |Resources|
'-------------' '-----------------' '--------------' '---------'
       |                |                  |             |
       |  Serve's Site  |                  |             |
       |--------------->|                  |             |
       |                |                  |             |
       |                | GET DB Entries   |             |
       |                |----------------->|             |
       |                |                  |             |
       |     REST Query for Resources      |             |
       |<----------------------------------|             |
       |                |                  |             |
       |            Resources              |             |
       |---------------------------------->|             |
       |                |                  |             |
       |                |                  |    POST     |
       |                |                  |------------>|
       |                |                  |             |
       |                |                  |  SQL Query  |
       |                |                  |------------>|
       |                |                  |             |
       |                |                  |   Entries   |
       |                |                  |<------------|
       |                |                  |             |
       |                |    Entries       |             |
       |                |<-----------------|             |
       |                |                  |             |
.-------------. .-----------------. .--------------. .---------.
|School Server| |Search Engine PWA| |Service Worker| |Resources|
'-------------' '-----------------' '--------------' '---------'
```

### Integration of "Login" for CRUD operations

```goat
 Milestone 3 - On-Prem Server with Login
-----------------------------------------
.-------------. .-----------------. .--------------. .---------.
|School Server| |Search Engine PWA| |Service Worker| |Resources|
'-------------' '-----------------' '--------------' '---------'
       |                |                  |             |     
       |  Serve's Site  |                  |             |     
       |--------------->|                  |             |     
       |                |                  |             |     
       |                | GET DB Entries   |             |     
       |                |----------------->|             |     
       |                |                  |             |     
       |     REST Query for Resources      |             |     
       |<----------------------------------|             |     
       |                |                  |             |     
       |            Resources              |             |     
       |---------------------------------->|             |     
       |                |                  |             |     
       |                |                  |    POST     |     
       |                |                  |------------>|     
       |                |                  |             |     
       |                |                  |  SQL Query  |     
       |                |                  |------------>|     
       |                |                  |             |     
       |                |                  |   Entries   |     
       |                |                  |<------------|     
       |                |                  |             |     
       |                |    Entries       |             |     
       |                |<-----------------|             |     
       |                |                  |             |     
       |                |   User Site      |             |     
       |                |----------------->|             |     
       |                |                  |             |     
       |   Request Encrypted User Site     |             |     
       |<----------------------------------|             |     
       |                |                  |             |     
       |            User Site              |             |     
       |---------------------------------->|             |     
       |                |                  |             |     
       |                |   User Site      |             |     
       |                |<-----------------|             |     
       |                |                  |             |     
       |                |      CRUD        |             |     
       |                |----------------->|             |     
       |                |                  |             |     
       |                |                  |    CRUD     |     
       |                |                  |------------>|     
       |                |                  |             |     
       |                |    Publish       |             |     
       |                |----------------->|             |     
       |                |                  |             |     
       |                |                  |   GET DB    |     
       |                |                  |------------>|     
       |                |                  |             |     
       |                |                  |     DB      |     
       |                |                  |<------------|     
       |                |                  |             |     
       |   REST CRUD with Credentials      |             |     
       |<----------------------------------|             |  
       |                |                  |             |   
.-------------. .-----------------. .--------------. .---------.
|School Server| |Search Engine PWA| |Service Worker| |Resources|
'-------------' '-----------------' '--------------' '---------'
```

## Getting to know the solutions