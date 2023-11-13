# Docker Overview

## Why You Need Docker Container

- Handling various tools like databases, messaging systems.
- Ensuring compatibility with different operating systems.
- Managing different versions of tools ('Matrix from Hell').

## What Can Docker Do

- Isolates each component in a separate container.
- Simplifies deployment with a simple `docker run` command.

## Understanding Containers

- Containers are lightweight, standalone, executable packages.
- Include everything needed to run an application: code, runtime, system tools, libraries, settings.
- More efficient and compatible compared to traditional software setups.

## Docker vs Virtual Machines

- ![Containers vs Virtual Machines](https://github.com/farhanajaved/K8_Notes/assets/87488893/c2909365-1e3c-46c0-b2a1-9e1a170e3521)
- Containers are more resource-efficient, faster, and offer isolated environments for applications.

## Docker Hub and Usage

- Docker Hub serves as a repository for Docker images.
- Basic command: `docker run <image_name>`.

## Image vs Container

- **Image:** A package or template, like a VM, used to create containers.
- **Container:** A running instance of an image with its own environment.

# Kubernetes (K8s) Architecture

## Introduction to Kubernetes

- Kubernetes is an orchestration system for managing containerized applications.
- Facilitates easy communication and management of containers.

## High-Level Architecture

- ![Kubernetes Architecture](https://github.com/farhanajaved/K8_Notes/assets/87488893/b4dd4b95-8c8d-4b05-8d08-8bb0b407ced3)

## Kubernetes Components

### Worker Node

- Hosts applications as containers.

### Master Node

- Manages, plans, schedules, and monitors the nodes.

### Control Plane Components

- **ETCD:** Stores important cluster information.
- **Kube Scheduler:** Determines where to run containers.
- **Controllers:** Includes Node Controller, Controller Manager, Replication Controller.

## Kubernetes Management

- **Kube API Server (Cube API):** Orchestrates and manages the cluster.
- **Container Compatibility:** Supports Docker and other container runtimes.
- **Kubelet:** Manages containers on each node, akin to a captain on a ship.

## Additional Points

- **Docker Containers vs. K8s Pods:** Pods are the smallest deployable units in K8s, containing one or more containers.
- **Networking in K8s:** Manages networking between containers and pods.
- **Scalability and High Availability:** Provides scalability and high availability for applications.
- **K8s Services and Load Balancing:** Offers services for load balancing and stable network addresses.
