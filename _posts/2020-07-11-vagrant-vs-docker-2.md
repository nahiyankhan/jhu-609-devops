---
ID: 12
post_title: Vagrant vs Docker
author: Nahiyan Khan
post_excerpt: ""
layout: post
permalink: http://one.wordpress.test/?p=12
published: true
post_date: 2020-07-11 22:01:49
---
I have used Docker at work and personal projects. I have not come across Vagrant before. To set the stage better, here is my experience with Docker first. 
Docker has been an immense lifesaver in my team. Over and over again the same repositories would have unique dependency issues on each of our machines. At first, I was giving a lot of time to help everyone resolve them but it was soon unscalable. Starting to use docker containers took that pain point off. The containers helped create a neutral shell for all the dependencies and it was agnostic of the host system. 

Vagrant looks very interesting. It is different from Docker in that it is a virtualization automation tool. While a Docker container relies on the host operating system to run on top of, Vagrant boxes encapsulate and contain any operating system that it is configured with. From the module lectures, I get the sense that Vagrant requires a bit more understanding of how it is set up and explicitly needs to call out the OS and configuration of the boxes via the vagrant files. Another additional step was the need to have Virtualbox installed and used as the box in which Vagrant runs. Hence, a virtualization box is a dependency albeit a simple one.

Another observation that I think is a benefit of Vagrant is that, since it is running a virtualized OS, more than one application can be run in the same environment. Meaning, applications can communicate with each other would be easier to set up. Docker, on the other hand, is one application per container. Multiple containers can run and talk to each other but with a bit more setup.