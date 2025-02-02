# Tiktok Server Backend Assignment 2023

![Tests](https://github.com/weixingp/tiktok-tech-immersion-2023/actions/workflows/test.yml/badge.svg)

## Overview
Designing and implementing a backend Instant Messaging system.
For this assignment, the focus will be on the backend only,
focusing on core message features without the front-end part and the account/authentication part.

## Requirements
1. Architecture: HTTP server and RPC server.
2. Data Storage: To store the the messages data.
3. Messages Delivery: deliver messages to the intended recipients in timely and consistent manner.
4. Performance and Scalability: Able to handle a relatively large number of users and messages. (more than 20 concurrent users)

## System Artitecture Design
![UML diagram](https://github.com/Iciclemeltz/tiktok-tech-immersion-2023/assets/71871315/0aa7b01f-8e1b-4917-ad3d-3fc4ea45f869)


## Implementation
1. For the database, Redis will be used. It is an open source in memory data and for this project advanced queries are not needed too.
2. Golang is required to be installed on the computer. For this project, Golang IDE will be used 
3. Docker will be used to run this project.Hence, Docker will be required to be installed as well.
4. Postman will be used to test out the API as well.

## Running The Program
1. right clock on docker-compose.yml and click on run. Wait for it to initialise and run.
2. Atfter the setup is done, use Postman to test the APIs. 
3. Afterwards, use the cURL format to import the request and try sending the message.
4. Note that the demo code logic has a 50% chance of getting a 200 Success Message or an 500 Internal Error.

## Testing
1. For Unit Testing, this project is unable to do as the database used in this case is Redis. It will not work as it cannot connect to the Redis server.
2. For the handling of more than 20 concurrent users JMeter is used to test for this scenario. Use the JMeter file in the repo and the QPS can be changed in the thread group.

## Scaling
1. Not yet implemented but if it is used Kubernetes cluster will be the way to go.

## Installation Links
1. Golang IDE (jetbrains): https://www.jetbrains.com/go/
2. Redis: https://aws.amazon.com/redis/
3. Docker: https://docs.docker.com/desktop/install/windows-install/
4. Postman: https://www.postman.com/downloads/
5. JMeter: https://jmeter.apache.org/download_jmeter.cgi
6. Kubernetes Cluster: https://kubernetes.io/releases/download/


