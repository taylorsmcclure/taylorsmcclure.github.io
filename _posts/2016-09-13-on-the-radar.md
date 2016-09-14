---
layout: post
title: "09.13.16 On the Radar"
categories:
  - Tech
  - Lifestyle
tags:
  - rpi3
  - projects
  - keto
  - keto fuel
  - docker
  - docker swarm
---

### On the Radar

So I have some projects on the radar that I am excited to get going. This will serve as a post get my goals/projects organized. Currently I have two things planned:

* Raspberry Pi 3 Cluster
* Keto Fuel Meal Replacements 

#### Raspberry Pi 3 Cluster

After seeing an article about a dude creating a [Raspberry Pi 2 cluster](http://makezine.com/projects/build-a-compact-4-node-raspberry-pi-cluster/){:target="_blank"} I was inspired to do the same but with a twist. I will be using Raspberry Pi 3s and the goal is to make them a [Docker Swarm](https://docs.docker.com/swarm/){:target="_blank"} cluster. The TLDR; on Docker Swarm is it is a high-availability cluster of machines that serve Docker containers. In my setup I will have 1 master node and 3 worker nodes. 

##### Critics

I had one of my friends present me with the question: "Why are you doing a cluster of Pis? Their network chips can only handle 100Mbps." This is definitely a true statement. While my local network is 1000Mbps for my use case(s) I will not need more than 100Mbps. I am not serving a massive webserver or creating a high traffic VPN.

Another issue raised by myself is in the article mentioned before the pi cluster all uses the same power supply and network switch. Those are two single points of failure. If you are familiar with Docker Swarm this almost completely defeats the purpose of it. My answer to that is "meh." This is <strong>project</strong>, this won't be in production and I don't plan on having it running surviving more than a few years.

##### What Will Go on It?

Currently I have only one Raspberry Pi 2 that manages the following on my home network:

* Hosts [AwesomeBot](https://github.com/taylorsmcclure/AwesomeBot){:target="_blank"}
* Hosts [AirhornBot](https://github.com/taylorsmcclure/airhornbot){:target="_blank"}
* Recursive DNS (named)
* Easy RSA VPN

While the one raspberry pi 2 has shown no issues managing all of this, I would like to have a more distributed environment, learn more about Docker Swarm, and eventually add a bunch more microservices.

#### Keto Fuel Diet

My Keto Fuel from [Super Body Foods](http://superbodyfuel.com/shop/keto-fuel/){:target="_blank"} has been on back order for quite a while now. There has been some production and supply chain issues on their end, so I hope I get it soon. Once I get it I will be doing a meal plan of 4 shakes a day and no other foods.

Ahh yes, that should be fun...

I plan on documenting as much as I can on a day-by-day basis, so stay tuned for that.
