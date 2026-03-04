what is kubernets:
==================

“Kubernetes is a container orchestration platform. It helps us deploy, scale, and manage containerized applications. It provides auto-scaling, self-healing, load balancing, rolling updates, and rollback. So instead of managing containers manually, Kubernetes manages everything automatically in production.”

why we use kubernets:
=====================

“We use Kubernetes to manage containerized applications in a scalable and automated way. In real projects, we have multiple microservices running as containers. Managing them manually is very difficult. Kubernetes helps us with auto-scaling, self-healing, load balancing, rolling updates, and rollback. So it ensures high availability and stability in production environments.”

If they ask for a simple explanation:


“Suppose my application is running in 3 containers. If one container crashes, Kubernetes automatically restarts it. If traffic increases, Kubernetes automatically creates more containers. That’s why we use Kubernetes — to automate and manage containers efficiently.”

what is different between docker and kubernets
===============================================

“Docker and Kubernetes serve different purposes. Docker is used to create and run containers. Kubernetes is used to manage and orchestrate those containers at scale.”
Let me explain clearly 👇

Docker
======

Used to build container images
Run application inside a container
Works well for single-container or small setups
Example: docker run myapp


Kubernetes
===========


Used to manage multiple containers
Handles scaling, load balancing, self-healing
Used in production for microservices
Example: automatically restart container if it crashes


what is advantage of kubernetes
================================

“The main advantage of Kubernetes is that it automates the deployment, scaling, and management of containerized applications. It makes applications highly available, scalable, and stable in production.”


1️⃣ Auto Scaling

If traffic increases, Kubernetes automatically increases the number of pods.
If traffic decreases, it reduces them.
So we don’t need manual intervention.

2️⃣ Self-Healing

If a container crashes, Kubernetes automatically restarts it.
If a node fails, it reschedules the pods to another node.

3️⃣ High Availability

It distributes application instances across multiple nodes.
So even if one server goes down, the application stays up.

4️⃣ Rolling Updates & Rollback

We can deploy a new version without downtime.
If something goes wrong, we can easily roll back to the previous version

5️⃣ Load Balancing

Kubernetes automatically distributes traffic across multiple pods.

6️⃣ Environment Consistency

Same deployment works in Dev, QA, and Prod — no environment issues.