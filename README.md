![Assignments](assignments.jpg)

# Introduction
Congratulations! You have been selected for the next phase of the selection process. 

This phase consists of the making of a software project. The true objective of this task is more to create an opportunity for the discussion of your technical skills as well as your apporach to the problem.

All assigments should be on boarded following the same criteria:

## Requirements
You formulate the requirements. Use functional (FR) and not functional requirements (NFRs). For instance performance, responsiveness, concurrency, etc. although some times you'll see some not functional requirements in the description of the assignment.
We recommend you using the Gherkin syntax to write the requirements (FRs and NFRs).

## Methodology
Write the code following the procedure, methodology and quality approach you consider is the best one for the project. Please include comments to illustrate decisions, solutions and approaches. 
We recommend you to pay special attention to the structure of the project, segregation of tasks and clarity of the code.



**Honesty**
Remember the goal is to give us an idea of your personal and special way of understanding software development. Please be honest and write your own code. It is thousands of times better to read YOUR code with mistakes and errors rather than reading some copied code from the web.

**Think of the whole process**
Try not thinking as a pure developer. We prefer the term * *Development Engineer* * . The Engineer is aware of the whole Software Development & Delivery Life Cycle to provide the maximum quality of the software as well as the tools to bring the component to Live considering all the circumstances in a regular delivery pipeline.

**Read everything!**
Have a look on the presented proposals for assignments and choose your favourite one. Please read carefully all the sections in the assignment to avoid confusions. 

**Any doubt?**
For any question send an email to jdediego@fexco.com, fmuno@fexco.com or tmacsweeney@fexco.com



# Assignments

## 1-The API and the Consumer

### Description
In this assignment our mission is to produce an API server that will expose 2 or more endpoints. These endpoints will implement some regular CRUD functions to be consumed by public API consumers (e. g. a public web site). The endpoints 

### Special Rules
Well, usually API endpoints are based exclusively on a single protocol, HTTP1. However, our API is intended to support at least two protocols. We suggest to publish a subscription to a topic for notifications or creating some streaming channel based on HTTP2. 
Examples of protocols: HTTP1, HTTP2, AMQP, MQTT, etc.
In any case the client (we prefer the term * *API Consumer* * ) should consume somehow all the endpoints available in the API regardless the implemented protocol.
It is not needed that all endpoints in the API server implement several protocols. 1 protocol per each endpoint is OK always you use at least 2 different protocols.

### Requirements
We expect a concurrency of 200 users (business time) with an average operation duration of 10 minutes.

### Expected Deliverable
We'd like to see:
1-The API server implementing the multi-protocol endpoints
2-An API consumer that actually does something with the API endpoints, composing and showing information retrieved from the API.
3-Any IaC needed to see everything working.

