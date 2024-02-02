---
title: "What are Blue-Green Deployments?"
seoTitle: "What are Blue-Green Deployments?"
seoDescription: "Learn the ins and outs of Blue-Green Deployments - a revolutionary approach for deploying software. Achieve smooth transitions and minimal risks"
datePublished: Wed Jan 31 2024 03:39:11 GMT+0000 (Coordinated Universal Time)
cuid: cls18nit6000208l4aco46cee
slug: what-are-blue-green-deployments
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1706672227503/d2c571f0-71e1-4d47-953f-b2f91493cf31.png
tags: deployment, devops, devops-articles, bluegreen-deployment

---

## Overview

"Blue-Green deployment" is an **application release model**, **software deployment strategy** and **deployment technique**, which offers:

* Near zero-downtime 🤯
    
* Simple roll-back capabilities
    
* Very low chances of failure 📉
    
* No maintenance windows
    
* Improved testing
    

> Blue/green deployments can mitigate common risks associated with deploying software, such as downtime and rollback capability
> 
> \- Amazon in the [AWS White paper on blue/green deployments](https://d0.awsstatic.com/whitepapers/AWS_Blue_Green_Deployments.pdf)

## How does "Blue-Green Deployments" work?

In Blue-Green Deployments, we have 2 servers, named `green` and `blue`. Both of them have **identical environments** but **different versions**. In the `blue` server, you have your production application which handles almost all of your traffic. Whereas in the `green` server, you have, a **semi-production** or **staging** version.

Now we test the `green` server if it works and is ready. We start *slowly* channelling away traffic to the `green` server. In other words, we follow a **rolling release** to publish the `green` server version.

So for instance, we have `blue` running on v1.0.0 (prod), and `green` on v1.0.0-beta (staging). We test the green server's version internally, then roll out the new version in chunks to our users. In this example, we give 25% of the people access to use it.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1706623728567/ac9a76ad-ba77-4328-a4c7-d69ad7651ef1.png align="center")

And this is repeated till eternity ✨ Here is the graph of the same scenario:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1706633803813/d7976edd-a6a8-42d7-b0a4-14fc044ab2dc.png align="center")

## What happens if my beta app breaks?

Let's take a second scenario, in this scenario, somehow the application passes the internal testing phase, but when users use it, it breaks apart 🥲. We can do an **instant** roll-back by redirecting all the traffic to the blue server!

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1706624700475/4d2fa865-277d-4621-87bd-02fe748573d2.png align="center")

## Rolling releases with Blue-Green Deployments

Since we have 2 servers where we are diving the traffic, we get to offer a certain feature to a set of users. This provides different benefits:

* You **minimise risks** since your release does not affect your entire user base
    
* **A/B Testing** allows you to analyse user groups' performance (both system & conversion).
    
* **Feedback Loops**: You can constantly collect feedback from users and iterate to improve your application.
    

You can send out the version to your users by directing traffic based on various factors such as:

* **Randomly:** You can send it out randomly to your users
    
* **Geographically**: Want a feature to only be available in the USA while you test it? You can!
    
* **Beta-testers**: Enrol users in a beta program or a select group of users like your friends and team 👀
    

So basically it is like feature-flags but for versions!

## More benefits

* Production testing! Since the app is on a replica of the production environment you can say we're testing on production 💥
    
* Since you are switching servers and resources, you do not have to worry about upgrading the application without breaking everything else!
    
* Since with the cloud, we can tear apart and provision new services instantly, it is also more lucrative/cost-efficient for us.
    

## Challenges

It does not make sense to have 2 databases and to sync between them for the environments, instead, we do the obvious and use the same database. The problem occurs when you make a breaking change to your schema because then your production version falls apart as it no longer can query for the same data schemas.

Other challenges include the inability to use the components of this method due to project, regulation or infrastructure-based restrictions.

## Further resources

* [Blue/Green Deployments on AWS](https://d0.awsstatic.com/whitepapers/AWS_Blue_Green_Deployments.pdf) *(a Whitepaper by AWS)*
    
* [Continuous Blue-Green Deployments With Kubernetes](https://semaphoreci.com/blog/continuous-blue-green-deployments-with-kubernetes) *(an Article by semaphoreci.com)*