![Assignments](assigments.jpg)

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

### Expected Deliverables
We'd like to see:

1-The API server implementing the multi-protocol endpoints

2-An API consumer that actually does something with the API endpoints, composing and showing information retrieved from the API.

3-Any IaC needed to see everything working (optional). It can run on your machine as the default option.



## 2-Extract, Transform, Load!

### Description
Probably you've guessed the main topic of this assignment from the header. Yes, it's about the infamous ETL processes world. The assignment consists of the making of an ETL applications that esentally:

Firstly, gets the data from a source data storage.

Secondly, applies one or several transformations of the content or the formats.

Finally, loads the result of the transformation to a one or several destination data storages.


### Special Rules
The application will run in a nightly basis with a limit of 15 minutes of running time (this is the time window provided by the evil people in charge of the infrastructure).

The maximum amount of memory to be consumed by the application is 3 GB.

Our system is 24/7. So, the source data storage can not suffer any latency or issue derived of the query related to the Extraction phase.


### Requirements
The ETL process must be able to handle at least 2 million of records for all involved phases.

We expect notifications from any unexpected error.

The ETL process should log all actions at different levels of importance and priority.

Administrators should be able to compose graphical dashboards from the operation logs of the ETL process in time. 


### Expected Deliverables
We'd like to see:

1-The ETL application including the mentioned phases as well as mock data storages to test the component.

2-Any related component handling the traces and logs from executions

3-Any IaC needed to see everything working (optional). It can run on your machine as the default option.



## 3-Microservice in Kubernetes

### Description
The goal of this assigment gathers a software component with IaC. Our mission is to develop an application as a microservice, following the main guidelines of the Micro Services Architecture. There is not any requirement about the implemented protocols but we'd like to see here is a good, solid, robust and efficient microservice, completely autonomous and containing all the features we could find in the best examples of microservices around the world.

Besides, we should release our microservice in a Kubernetes cluster and find out what is its behavior in a Kubernetes pod with several containers containing the app.


### Special Rules
You can choose your favourite protocol or protocols for the microservice but you always should follow an architectural pattern (for instance, REST architecture for HTTP1). 


### Requirements
High Availability, responsiveness and robustness are the core terms here. It is expected a really high concurrency (+500 users) and workload (heavy payloads in some occasions). You should implement some kind of heavy payload in the usage of the microservice to emulate this workload.


### Expected Deliverables
1-The microservice application applying all the special rules and standard quality features.

2-This time is mandatory: You have to provide the IaC needed to stand up a Kubernetes cluster with a pod of several instances of the microservice. The target of the IaC can be a Cloud Provider or anything you consider. Factors as exchangeability, agnosticism and versatility of the IaC code will be really appreciated.



**Good Luck!**
Well, that's all folks. Again, if you have any question send an email to jdediego@fexco.com, fmuno@fexco.com or tmacsweeney@fexco.com
