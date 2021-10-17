---
layout: post
title:  "Blog 5 - Ansible"
date:   2021-10-16 8:15:29 -0700
categories: Tech
---
## Ansible: An Introduction
Developed by Michael DeHaan, who also provisioned and developed the server application Cobbler and the Fedora Unified Network Controller, the Ansible tool was founded in 2013. To put it briefly, Ansible is an open-source IT automation engine. IT Automation refers to automatic provisioning, orchestration, application development and many more IT applications. Ansible runs on many Unix-like systems, and it can describe system configuration through its own declarative language. Ansible is linked to many historic IT applications as it is included with the Fedora distribution of Linux. It is also owned by Red Hat, and many other software companies such as CentOS, Debian, Scientific Linux, and etc. The inspiration for this blog regarding Ansible stems from Lab 3 of this course, where we learned how to deploy Ansible playbooks and create automated scripts within. To get a better idea of Ansible and its features, we will be going over its Architecture, Design Goals, and Cloud Integration. 
<br/><br/>
<img src="https://askops.in/wp-content/uploads/2020/05/ansible1.png" alt="MSC" width="460" height="345">

## Architecture
Ansible Architecture is interesting as it has a Python-dependent configuration. This means that Ansible is essentially a configuration-management software within Python where the controlling node and target machine require Python dependent packages. Since Ansible doesn't require a single controlling machine, it can work against multiple systems by choosing elements within Ansible's inventory. This includes version-able ASCII text files and other stored as edit-able files as well. 
<br/><br/>
Since Ansible does not have a central-server requirement, this drastically simplifies the planning for any disaster-recovery which may take place within its architecture. SSH also manages the Nodes on this controlling machine, and it can describe the location of them through its own inventory. Ansible Vault is also an important piece of its Architecture which stores Sensitive Data. Most importantly, Ansible's Architecture is described as "agentless", which means its software is not normally installed or running on the controlled node. Furthermore, nodes can be orchestrated through running and installing modules available on SSH temporarily. 
<br/><br/>
<img src="https://media-exp1.licdn.com/dms/image/C5612AQFxUgiPFoRJ9g/article-inline_image-shrink_1000_1488/0/1606844037609?e=1636588800&v=beta&t=_33qdbbuVBZ4oWcj1Nii5v6vzboKM9X1IylrOzlwrQ8" alt="MSC" width="460" height="345">


### Design Goals
Ansible has many design goals, which were set in mind back in 2013 during its initial development. This goals focus on keeping Ansible simple, logical and dependable. Through its various updates and patches, these design goals are reverberated to its users, and they take feedback into account for every possible development scenario.
<br/><br/>
- `Keep It Minimal`: To keep a minimalistic environment, management systems should not impose additional dependencies in the controlling machine.
- `Reliability`: Creating idempotent playbooks that can prevent unexpected occurences on managed systems.
- `Consistency`: Environments should be able to be created consistenly with Ansible
- `Security`: Only Python and OpenSSH are required on managed nodes, and agents are not deployed to nodes in Ansible
- `Easy Learning Curve`: Descriptive languaged such as YAML and Jinja templates are based for Ansible Playbooks.
- `Twitch`: The user streaming service applies Go for their IRC-based chat system.


## Cloud Integration
Integration on the cloud is possible in Ansible through bare metal hosts, cloud environments and virtual machines. Some examples of these cloud integration services are Amazon Web Services (AWS), Docker, Google Cloud Platform, Microsoft Azure, Oracle Cloud, and etc. Since Ansible allows for cloud integration on the various well-known cloud services, this IT automation engine is a powerful tool for many developers and programmers. Writing automated scripts is important in local environments, but applying them to a wide-variety of applications and projects through cloud services proves how important IT Automation software like Ansible can be. For this reason, there is no doubt new cloud installations and applications of future developments within IT fields see an increase in automation through Ansible. Developers interested in learning how to apply Ansible in cloud services such as AWS should visit the [Ansible Docs][Ansibledocs-io] to learn more on how to create an AWS Cloudformation stack using Ansible.
<br/><br/>
<img src="https://programmaticponderings.files.wordpress.com/2019/07/codepipeline.png" alt="MSC" width="460" height="345">

### Learn More About Ansible
You can visit [Ansible][golang-io] to learn about the Ansible Platform and how it works to automate cases and fast track development journeys. Much like other software-companies, Ansible offers a variety of ways to get in touch with similar-minded users that deploy Ansible in their working applications. [Ansible Fest][Ansiblefest-io] is an event where users can sign up to join developers, administrators, and IT decision makers at Ansible. There is also a large forum-based [Community][Community-io] that allows for collaboration to help users experience the power of automation possible through Ansible. 

[ansible-io]: https://www.ansible.com/
[Ansiblefest-io]: https://www.ansible.com/ansiblefest 
[Community-io]: https://www.ansible.com/community 
[Ansibledocs-io]: https://docs.ansible.com/ansible/latest/collections/amazon/aws/cloudformation_module.html 