---
layout: post
title:  "Blog 0 - Kubernetes"
date:   2021-09-15 03:52:29 -0700
categories: Tech
---
## Introduction to Kubernetes
Kubernetes is a portable, extensible, and open-source platform which allows management of containerized workloads and
services. These services facilitate both declarative configuration and automation, as Kubernetes has a rapidly growing
ecosystem. Kubernetes was open-sourced by Google in 2014, and is now maintained by the Cloud Native Computing Foundation.

## What can you do with Kubernetes
In order to make sure there is no downtime for containers that run applications, Kubernetes provides users 
with a framework to run distributed systems resiliently. This means it takes care of failover and scaling, and 
provides deployment patterns for your applications.

Useres expect applications to be available all day within modern web services, in order for developers to deploy updated versions 
regularly. Kubernetes helps containerization applications run and provides tools resources when they need to function. Containerization
is especially important in modern web services as applications need to be be released and updated without any downtime.

### A few examples of what Kubernetes provides you with:
- Service discovery and load balancing
- Storage Orchestration
- Automated rollouts and rollbacks

## What Kubernetes is not | Common Issues
It is important to note that Kubernetes is not a traditional Platform as a Service System `Paas`, because it operates at 
the container level rather than the hardware level. This also means Kubernetes `does not` deploy source code or build your application.
It also does not dictate logging, monitoring or alerting solutions, and does not provide nor mandate a configuration language/system.

What does this mean for smaller organizations? If an organization has just one data center and fewer than a dozen applications that will be 
deployed, Kubernetes is an overkill. Although Kubernetes is not currently recommended for smaller organizations, there are various updates
and versions that are being worked on to deploy Kubernetes for smaller applications in the future.

Another common issue with Kubernetes is that it is hard to control manually. There are ways for users and admins to modify containers properly,
but Kubernetes architecture is not designed to expect manual changes from admins. Most of the time, Kubernetes defaults are set for most
web-scale deployments where there are thousands of servers and workloads. But for smaller groups, Kubernetes will not make it easy to have
more control on workloads due to its high volume defaults.

## Solve Problems with Kubernetes | Debugging
Troubleshooting in Kubernetes is efficient due to `Debugging Pods` which are specifically made to debug workloads in Kubernetes containers.
The first step in troubleshooting is triage, where you have the options of `Debugging Pods`, `Debugging Replication Controllers`, and `Debugging Services`. 
This [Troubleshoot.io][troubleshoot-io-io] documentation from Kubernetes explains troubleshooting methods, and the most effective methods to solve problems 
with Kubernetes containers.

It's important to know that when the triage of troubleshooting defaults do not work, there is also a Debugging Service Document to make sure that
a `Service` is properly running. More troubleshooting documentation is available through the Kubernetes contact page.

### Learn more about Kubernetes
If I were to research Kubernetes again for a future blog, I would take a different approach by researching user preferences and overall
satisfaction with Kubernetes from customer reviews, rather than visiting their main site first. This would be a good way to view different
perspectives of services offered and provided, and see possible solutions/issues that Kubernetes might not be transparent with on their home site.

There is quite a bit of info regarding Kubernetes and deployment strategies, which can be found on [Kubernetes.io][kubernetes-io].
They also have a [Documentation][documentation-io] page which includes training, setting up a K8s cluster, and looking up reference information. Stay tuned for more posts on Kubernetes!



[kubernetes-io]: https://kubernetes.io/
[documentation-io]: https://kubernetes.io/docs/home/ 
[troubleshoot-io]: https://kubernetes.io/docs/tasks/debug-application-cluster/debug-application/#debugging-pods/ 