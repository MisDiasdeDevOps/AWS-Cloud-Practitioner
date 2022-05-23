---
title: '#90DaysOfDevOps - Plan > Code > Build > Testing > Release > Deploy > Operate > Monitor > - Day 5'
published: false
description: 90DaysOfDevOps - Plan > Code > Build > Testing > Release > Deploy > Operate > Monitor >
tags: "devops, 90daysofdevops, learning"
cover_image: null
canonical_url: null
id: 1048830
---
## Plan > Code > Build > Testing > Release > Deploy > Operate > Monitor > 

Today we are going to focus on the individual steps from start to finish and the continous cycle of an Application in a DevOps world. 

![DevOps](Images/Day5_DevOps8.png)

### Plan:

It all starts with the planning process this is where the development team gets together and figure out what types of features and bug fixes that they're going to roll out in their next sprint. This is an opportunity as a DevOps Engineer for you to get involved with that and learn what kinds of ththat's going to work better for them in case they're not on that path and so one key thing to point out here is the developers or software engineering team is your customer as a DevOps engineer so this is your opportunity to work with your customer before they go down a bad path.ending again on what type of application you're working on this may be a non-step. You know the code may just live in the GitHub repo or the git repository or wherever it lives but it may be the process of taking your compiled code or the docker image that you've built and putting it into a registry or a repository where it's accessible by your production servers for the deployment process g slow or their application is running slow right so you need to figure out why that is and then possibly build auto-scaling you know to handle increase the number of servers available during peak periods and decrease the number of servers during off-peak periods either way that's all operational type metrics, another operational thing that you do is include like a feedback loop from production back to your ops team letting you know about key events that happened in production such as a deployment back one step on the deployment thing this may or may not get automated depending on your environment the goal is to always automate it when possible there are some environments where you possibly need to do a few steps before you're ready to do that but ideally you want to deploy automatically as part of your automation process but if you're doing that it might be a good idea to include in your operational steps some type of notification so that your ops team knows that a deployment has happened 

## Monitor:

All of the above parts lead to the final step because you need to have monitoring, especially around operational issues auto-scaling troubleshooting like you don't know
there's a problem if you don't have monitoring in place to tell you that there's a problem so some of the things you might build monitoring for are memory utilization CPU utilization disk space, api endpoint,  response time,  how quickly that endpoint is responding and a big part of that as well is logs. Logs give developers the ability to see what is happening without having to access production systems. 

## Rince & Repeat: 

Once that's in place you go right back to the beginning to the planning stage and go through the whole thing again

## Continuous:

Many tools help us achieve the above continuous process, all this code and the ultimate goal of being completely automated, cloud infrastructure or any environment is often described as Continuous Integration/ Continuous Delivery/Continous Deployment or “CI/CD” for short. We will spend a whole week on CI/CD later on in the 90 Days with some examples and walkthroughs to grasp the fundamentals. 

### Continuous Delivery:

Continuous Delivery = Plan > Code > Build > Test 

### Continuous Integration:

This is effectively the outcome of the Continuous Delivery phases above plus the outcome of the Release phase. This is the case for both failure and success but this is fed back into continuous delivery or moved to Continuous Deployment. 

Continuous Integration = Plan > Code > Build > Test > Release 

### Continuous Deployment: 

If you have a successful release from your continuous integration then move to Continuous Deployment which brings in the following phases 

CI Release is Success = Continuous Deployment = Deploy > Operate > Monitor 

You can see these three Continuous notions above as the simple collection of phases of the DevOps Lifecycle. 

This last bit was a bit of a recap for me on Day 3 but think this actually makes things clearer for me. 

### Resources:

- [DevOps for Developers – Software or DevOps Engineer?](https://www.youtube.com/watch?v=a0-uE3rOyeU)
- [Techworld with Nana -DevOps Roadmap 2022 - How to become a DevOps Engineer? What is DevOps? ](https://www.youtube.com/watch?v=9pZ2xmsSDdo&t=125s)
- [How to become a DevOps Engineer in 2021 - DevOps Roadmap](https://www.youtube.com/watch?v=5pxbp6FyTfk)

If you made it this far then you will know if this is where you want to be or not. 

See you on [Day 6](day06.md). 
