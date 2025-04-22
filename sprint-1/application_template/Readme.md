## Application Template
---

##  **Author Information**
| Created     | Version | Author        | Last Updated       |           |          |
|-------------|---------|---------------|--------------------|------------------|------------------|
| 17-04-2025  | V1      | Adil Nawaz    |                    |            |          |

---



##  Table of Contents

1. [ Purpose](#purpose)  
2. [ Pre-requisites](#pre-requisites)  
3. [ System Requirements](#system-requirements)  
4. [ Dependencies](#dependencies)  
   - [ Build Time Dependency](#build-time-dependency)  
   - [ Run Time Dependency](#run-time-dependency)  
   - [ Other Dependency](#other-dependency)  
   - [ Important Ports](#important-ports)  
   - [ Others](#others)  
5. [ Architecture](#architecture)  
6. [ Dataflow Diagram](#dataflow-diagram)  
7. [ Step-by-step Installation of [Application]](#step-by-step-installation-of-application)  
   - [ Step 1: Install Software Dependencies](#step1-installation-of-software-dependencies)  
   - [ Step 2: Build/Artifact Generation](#step2-buildartifact-generation)  
   - [ Step 3: Application Deployment](#step3-application-deployment)  
8. [ Monitoring](#monitoring)  
   - [ Metrics](#metrics)  
   - [ Health Check](#health-check)  
   - [ Explanation of Health Check Parameters](#explanation-of-parameters-used-in-above-table)  
9. [ Logging](#logging)  
   - [ Event Logs](#event-logs)  
   - [ Authentication & Authorization Logs](#authentication--authorization-logs)  
   - [ Server Logs](#server-logs)  
   - [ Threat Logs](#threat-logs)  
10. [ Disaster Recovery](#disaster-recovery)  
11. [ High Availability](#high-availability)  
12. [ Contact Information](#contact-information)  
13. [ References](#references)  

---


## Purpose
Explain the purpose of this application. Why there was a need for this application and what problems does it solve.

## Pre-requisites
Before diving into application deployment, let’s ensure the following Hardware, Software and Security requirements are met.

## System Requirements

| Hardware Specifications | Minimum Recommendation |
|-------------------------|------------------------|
| Processor                | Dual Core                        |
| Ram                      | 4GB                       |
| Disk                     | 20GB                       |
| OS                       | Ubuntu(22.04)     |

## Dependencies

### Build Time Dependency

| Name                    | Version                | Description |
|-------------------------|------------------------|-------------|
|  <application>          | <version>              |<Description>|
|  <application>          | <version>              |<Description>|
|  <application>          | <version>              |<Description>|
|  <application>          | <version>              |<Description>|

### Run Time Dependency

| Name                    | Version                | Description |
|-------------------------|------------------------|-------------|
|  <application>          | <version>              |<Description>|
|  <application>          | <version>              |<Description>|



### Other Dependency

| Name                    | Version                | Description |
|-------------------------|------------------------|-------------|
|  <application>          | <version>              |<Description>|
|  <application>          | <version>              |<Description>|

### Important Ports

| Inbound Traffic         | Description |
|-------------------------|------------------------|
| 8080          | used by Tomcat-server            |


| Outbon Traffic         | Description |
|-------------------------|------------------------|
| 9042          | used by ScyllaDB            |

### Others

| Others                  | Description            |
|-------------------------|------------------------|
| Additional Requirements | Description            |


### Architecture


### Dataflow Diagram

Explain the flow of the data in this diagram. How the data is traveling/flowing in this application.

## Step-by-step installation of [application]

### Step1: Installation of software Dependencies
**Build Dependency**
Add the command used to install the dependency in code snippet format. [command]

**Run time Dependency**
Add the command used to install the dependency in code snippet format. [command]

**Other Dependency**
These are the dependencies specific to integration of your application with 3rd party application.

### Step2: Build/Artifact Generation
  - Clone the git repository [commands]
  - Run the following command inside the directory to build your software artifact. [commands]
### Step3: Application Deployment
  - Perform the following steps to deploy the software artifact. [command]
  - Ensure the application deployed is in working state [command]

### Monitoring
Monitoring in DevOps refers to the practice of continuously observing and collecting data from various components of an application or system to ensure its health, performance, and availability. It involves tracking various metrics, events, and logs to identify issues, anomalies, and opportunities for improvement. Monitoring is a crucial aspect of the DevOps lifecycle as it helps teams proactively manage and maintain their applications, enabling faster response to problems and better overall system performance.

### Metrics

| Parameter  |             Description                       | Priority |    Threshold   |
|------------|-----------------------------------------------|----------|----------------|
| Disk Utilization | The percentage of disk space used by the application.    | High   | >90%          |
| Availablity      | The percentage of time the application is available.     | High   |               |
| Memory Utiliztion| The percentage of memory used by the application.        |        |               |
| CPU Utilization  | The percentage of CPU time used by the application.      |        |               |
| Network Traffic  | The amount of network traffic generated by the application.|      |               |
| Latency    | The time taken for the application to respond to a request.    |        |               |
| Errors     | The number of errors generated by the application.             |        |               |
| Throughput | The number of requests the application can handle per unit of time.|    |               |
| Security	 | The security of the application (authentication, authorization, encryption).|    |       |

### Health Check

| Name       |   Type   | InitialDelaySeconds |    PeriodSeconds   | TimeoutSeconds | SuccessThreshold | FailureThreshold |
|------------|----------|---------------------| -------------------|----------------|------------------|------------------|
| App Name   | Readiness Probe| 10            | 10                 | 5              | 1                |  3                |
| App Name   | Liveness Probe | 10            | 10                 | -              | 5                | 1                 |

### Explanation of parameters used in above table

| Parameter           | Description           |
|---------------------|------------------------|
| ReadinessProbe      | This probe checks if the application is ready to receive traffic.                |
| LivenessProbe       | This probe checks if the application is still running and responding to requests.| 
| InitialDelaySeconds | The number of seconds to wait before the first health check is performed.        | 
| PeriodSeconds       | The frequency at which the health check should be performed.                     | 
| TimeoutSeconds      |The maximum amount of time that the health check should wait for a response before it considers the application unhealthy                         | 
| SuccessThreshold    | The number of consecutive successful health checks before the application is considered healthy.| 
| FailureThreshold    | The number of consecutive unhealthy health checks before the application is considered unhealthy.| 


### Logging

This offers all types of logs related to the application like: Event Logs, Server Logs, System Logs, Authorization and Access Logs, Change Logs, Availability Logs, Resource Logs, Threat Logs

| Event Logs               |                                Description                                                   |
|--------------------------|----------------------------------------------------------------------------------------------|
| location/to/event.log    | An event log is a high-level log that records network traffic and usage data such as incorrect password attempts, login attempts, and application events.|

| Authentication & Authorization Logs             |                                Description                            |
|--------------------------|----------------------------------------------------------------------------------------------|
| `location/to/access.log`  |Authorization and access logs contain a list of persons or bots who have accessed specific programs or files.|


| Server Logs             |                                Description                            |
|--------------------------|----------------------------------------------------------------------------------------------|
| `location/to/server.log`  |A server log is a text document that keeps track of actions on a certain server over some time.|

| Threat Logs             |                                Description                            |
|--------------------------|----------------------------------------------------------------------------------------------|
| `location/to/threat.log`  |Threat logs are logs that contain information on the system, file, or application traffic that matches a firewall's security profile.|


### Disaster Recovery

In the event of a disaster affecting the application's functionality, it's important to have a robust disaster recovery plan in place. It typically ensures that critical systems and data can be restored after a disaster.

Disaster could be caused by a natural disaster, a cyberattack, or other event that takes down your IT infrastructure.

### High Availability

Ensuring high availability of the application is crucial to minimize downtime and provide seamless service to users. High Availability is a design approach that minimizes downtime for critical systems and services. This is achieved by deploying redundant components and systems, so that if one component fails, another can take over.

Note: In other words, DR is focused on recovering from a disaster, while HA is focused on preventing downtime.

### Contact Information

| Name         | Email Address                                 |
|--------------|-----------------------------------------------|
| Adil Nawaz | adil.nawaz.snaatak@mygurukulam.co           |


## References

| **Title**                        | **Link**                                                                                      |
|----------------------------------|-------------------------------------|
| Ubuntu Official Documentation  | (https://help.ubuntu.com)          |
| Ubuntu Releases List           | (https://wiki.ubuntu.com/Releases) |





















