+++
title = '8th Fall Meeting - Docker & Microservices'
date = 2023-10-19T11:00:00-12:00
draft = false
summary = 'club meeting, presentation, docker'
tags = ['technologies', 'docker', 'web', 'full-stack']
+++

# Attendance

- Karl
- Luke B
- David
- Christian
- Luke
- Paul
- Matthew
- Moe
- Brandon
- Zach

# Announcements

No announcements were given this meeting.

# Overview

Guest speaker Paul MacLean, former president of the Software Development Club, held a presentation on Docker and microservices. He discussed the basics of Docker, and provided a live demo using his own implementation of a basic server.

## Docker

Docker is used to install and run applications on a containerized file system. These containers usually run a Linux distribution. Some people compare containers to virtual machines. However, containers are much more lightweight than a VM, and is usually interfaced by a terminal.

Paul proposed a full-stack application for users to create an account, sign in, and modify settings. Users may also view, upload, and delete posts. This server will be managed using Docker. Each of these actions will be associated with an API endpoint.

## Issues

Paul discussed the downsides of using a single container to manage all API endpoints. He mentioned the following complications:
- New features may break existing ones
- Hard to monitor resources
- Thousands of APIs in one codebase is difficult to manage.
- Vulnerable to DDoS attacks.
- If one API is "abused", it may affect all other APIs.

## Group Related APIs

Paul's solution is to use multiple Docker containers. Related APIs will be grouped in one container. He decided to separate our APIs into the following groups.
- Image features
- Authentication features
- User-settings features

This implementation solves a few issues with the first approach.
- Feature updates won't break other features
- Easier to monitor resources for related APIs
- Databases may determine the type of API endpoint it receives.
- The codebase is easier to understand.

## How are Containers Made?

A Docker File is a text file of instructions to generate a docker image.
- Specify the programs to install
- Specify commands to run
A Docker Image is the "blueprint" for creating multiple containers. Once a container is created, you can launch and use it.

## Docker File Syntax

Here is an example of Docker File syntax.
```dockerfile
FROM python:3.11
ADD  requirements.txt .
RUN  pip install -r requirements.txt
ADD  src/* /home/app
```
`FROM` specifies a dependency.
`ADD` copies a file from your project to the container.
`RUN` executes a terminal command in the container.

## Live Demo

Paul showcased a live demo of Docker. He provided a back-end and database as microservices. He shown us the server logs and terminal output from the Docker GUI.

## Docker Compose

Docker Compose is a composition of multiple related Docker Containers. These details are stored as one `YML` file. Here are some details you may provide for each container.
- Image
- Container name
- Build command
- Ports
- Environment
- Dependencies.

# Votes

No votes were held this meeting.
