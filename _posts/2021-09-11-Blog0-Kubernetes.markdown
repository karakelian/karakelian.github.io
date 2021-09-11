---
layout: post
title:  "Blog 0 - Kubernetes"
date:   2021-09-11 03:52:29 -0700
categories: Tech
---
## Introduction to Kubernetes
Kubernetes is a portable, extensible, and open-source platform which allows management of containerized workloads and
services. These services facilitiate both declarative configuration and automation, as Kubernetes has a rapidly growing
ecosystem. Kubernetes was open-soruced by Google in 2014, and is now maintained by the Cloud Native Computing Foundation.

## What can you do with Kubernetes
In order to make sure there is no downtime for containers that run applications, Kubernetes provides users 
with a framework to run distributed systems resiliently. This means it takes care of failover and scaling, and 
provides deployment patterns for your applications.

### A few examples of what Kubernetes provides you with:
- Service discovery and load balancing
- Storage Orchestration
- Automated rollouts and rollbacks

## What Kubernetes is not
It is important to note that Kubernetes is not a traditional Platform as a Service System `Paas`, because it operates at 
the container level rather than the hardware level. This also means Kubernetes `does not deploy source code` or build your application.
It also does not dictate logging, monitoring or alerting solutions, and does not provide nor mandate a configuration language/system.

### Learn more about Kubernetes
There is quite a bit of info regarding Kubernetes and deployment strategies, which can be found on [Kubernetes.io][kubernetes-io].
They also have a [Documentation][documentation-io] page which includes training, setting up a K8s cluster, and looking up reference information. Stay tuned for more posts on Kubernetes!



[kubernetes-io]: https://kubernetes.io/
[documentation-io]: https://kubernetes.io/docs/home/ 