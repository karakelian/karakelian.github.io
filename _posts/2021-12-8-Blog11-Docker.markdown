---
layout: post
title:  "Blog 11 - Docker"
date:   2021-12-8 6:15:29 -0700
categories: Tech
---
## Docker Basics
Docker is a PAAS (platform as a service) that employs OS-level virtualization to deliver software in packages that are called "containers". These containers can be used in isolation from one another, which allows them to bundle their own software, configuration files, libraries and etc. Since they share the service on a single O.S. kernel, fewer resources are utilized when compared to a virtual machine. For this reason, Docker has become a very important aspect of virtualization technology in education and professional environments. To learn more about Docker, we will be reviewing its history and touching upon its operation including its components. 
<br/><br/>
<img src="https://developers.redhat.com/sites/default/files/styles/article_feature/public/blog/2014/05/homepage-docker-logo.png?itok=zx0e-vcP" alt="MSC" width="350" height="200">
<br/>

## Docker: History
Founded by Kamel Founadi and Sebastien Pahl, Docker Inc was launched in 2011 and its main stable release debuted in Satna Clara at PyCon in 2013. At the time of release, Docker used LXC for its default execution environment, but was later released with libcontainer, which was written in the Go Language. `Refer to Blog 3 and Blog 4 to recall on Golang.` Since then, docker has been a prominent set of PAAS products that have been adopted by Fedora, Red Hat Enterprise Linux, and etc. After its release in 2013, Microsoft announced the integration of the Docker Engine a year later in 2014, to serve as a native support for the Docker client role in Windows.
<br/><br/>
As of recently, Docker announced in August 2021 that Docker Desktop will no longer be free for enterprise users. This meant that larger business customers would have to switch out to a personal plan instead of Docker's Free plan. 

## Operation: Components and Tools
The Docker Software as service offers the following three components to its users:
- `Software`
- `Objects`
- `Registries`
<br/>
`Software` refers to the Docker daemon, also called "dockerd", which is a persistent process that manages Docker containers and objects. Requests are sent via the Docker Engine API, and responses are made through the command-line interface which interacts the Docker daemon with its users. 
<br/>
`Objects` refer to Docker objects that are various entities used to assemble applications in Docker. The main classes of objects are organized are images, containers, and services. 
<br/>
`Registries` refer to repositories for Docker images, which allows the Docker client to connect to registries to download `pull` images for use or upload `push` images. 
<br/>
<img src="https://wiki.aquasec.com/download/attachments/2854889/Docker_Architecture.png?version=1&modificationDate=1520172700553&api=v2" alt="MSC" width="350" height="250">
<br/><br/>
Tools in Docker refer to utilities such as `Docker Compose`, `Docker Swarm` and `Docker Volume` which help in defining and running multi-container applications. 
<br/>
`Docker Compose` uses YAML files to configure the application's services, and its CLI utility enables users to run commands all at once on multiple containers. 
<br/>
`Docker Swarm` is important as it provides native clustering for containers in Docker, and this allows Docker Engines to group into a virtual Docker Engine.
<br/>
`Docker Volume` allows a solution when files that have been copied or created in a container are deleted when the container is stopped. 
<br/>
<img src="https://static.site24x7.com/images/community/2015/06/docker-workflow-tools.png" alt="MSC" width="350" height="250">
<br/><br/>

## Noted Disadvantages
Some noted disadvantages with Docker is that Containers don't run at bare-metal speeds. Since containers consume resources more efficiently, users feel like they should run faster than virtual machines. This however is not always the case because containers are still subject to performance overhead due to overlay networking. 
<br/>
Data Storage can also become complicated since the data inside a container disappears forever when the container is shut down. For this reason, the Docker Tool we touched upon above, `Docker Volume`, offers ways to save data persistently. Its also important to note that not all applications will benefit from containers, unless they are designed to run as a set of discreet microservices.

### Learn More About Docker
Docker has become a prominent fixture in the IT Industry and Dockers [Homepage][web-io] has great resources available to users seeking to learn more about it. Docker also has important features that can be learned through its [Getting Started][start-io] page, which includes complete container solution for users. To stay in tune with news regarding Docker, make sure to keep an eye on their [Docker Blog][blog-io] and stay up to date with the newest articles.
<br/><br/>
Stay tuned for a new blog when we come back from our Winter Break! 

[web-io]: https://www.docker.com/
[start-io]: https://www.docker.com/get-started
[blog-io]: https://www.docker.com/blog/
