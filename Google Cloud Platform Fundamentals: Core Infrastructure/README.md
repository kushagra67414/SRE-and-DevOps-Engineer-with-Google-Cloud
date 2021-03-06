# Google Cloud Platform Fundamentals: Core Infrastructure

## What is Cloud Computing

Cloud computing is a way of using I.T. that has these five equally important traits. First, you get computing resources on-demand and self-service. All you have to do is use a simple interface and you get the processing power, storage, and network you need, with no need for human intervention. Second, you access these resources over the net from anywhere you want. Third, the provider of those resources has a big pool of them and allocates them to customers out of that pool. That allows the provider to get economies of scale by buying in bulk and pass the savings on to the customers. Customers don't have to know or care about the exact physical location of those resources. Fourth, the resources are elastic. If you need more resources you can get more, rapidly. If you need less, you can scale back. And last, the customers pay only for what they use or reserve as they go. If they stop using resources, they stop paying. That's it. That's the definition of cloud.

## GCP computing architectures

![104838175-3bd99a80-58df-11eb-9f3d-9d787febd28c](https://user-images.githubusercontent.com/46487696/105801136-7bc70e80-5fbe-11eb-9eda-479ec789a541.png)


## The Google Network
According to some estimates out there publicly, Google's network carries as much as 40 percent of the world's Internet traffic every day. Google's network is the largest of its kind on earth and the company has invested billions of dollars over the years to build it. It's designed to give its users the highest possible throughput and the lowest possible latencies for their applications. The network interconnects at more than 90 Internet exchanges and more than 100 points of presence worldwide. When an Internet user sends traffic to a Google resource, Google responds to the user's request from an edge network location that will provide the lowest latency. Google's Edge-caching network sites content close to end users to minimize latency.

# Environmental Responsibility

![104838175-3bd99a80-58df-11eb-9f3d-9d787febd28c](https://user-images.githubusercontent.com/46487696/105801196-a2854500-5fbe-11eb-8927-123422409cac.png)

## Why Choose Google Cloud Platform

Google Cloud Platform lets you choose from computing, storage, big data, machine learning and application services for your web, mobile, analytics and back-end solutions. It's global, it's cost effective, it's open source friendly and it's designed for security. Let's sum up. Google Cloud Platform's products and services can be broadly categorized as compute, storage, big data, machine learning, networking and operations and tools. This course considers each of the compute services and discusses why customers might choose each. The course will examine each of Google Cloud Platform storage services, how it works and when customers use it. To learn more about these services, you can participate in the training courses in Google Cloud's Data Analyst learning track. This course also examines the function and purpose of Google Cloud Platform's big data and machine learning services. More details about these services are also available in the training courses in Google Cloud's Data Analyst learning track.

## Multi-layered security approach

Because Google has seven services with more than a billion users, you can bet security is always on the minds of Google's employees. Design for security is pervasive, throughout the infrastructure, the GCP and Google services run-on. Let's talk about a few ways Google works to keep customers' data safe, starting at the bottom and working up. Both the server boards and the networking equipment in Google data centers are custom designed by Google. Google also designs custom chips, including a hardware security chip called Titan that's currently being deployed on both servers and peripherals. Google server machines use cryptographic signatures to make sure they are booting the correct software. Google designs and builds its own data centers which incorporate multiple layers of physical security protections. Access to these data centers is limited to only a very small fraction of Google employees, not including me. Google's infrastructure provides cryptographic privacy and integrity for remote procedure called data-on-the-network, which is how Google services communicate with each other. The infrastructure automatically encrypts our PC traffic in transit between data centers. Google Central Identity Service, which usually manifests to end users as the Google log-in page, goes beyond asking for a simple username and password. It also intelligently challenges users for additional information based on risk factors such as whether they have logged in from the same device or a similar location in the past. Users can also use second factors when signing in, including devices based on the universal second factor U2F open standard. Here's mine. Most applications at Google access physical storage indirectly via storage services and encryption is built into those services. Google also enables hardware encryption support in hard drives and SSDs. That's how Google achieves encryption at rest of customer data. Google services that want to make themselves available on the Internet register themselves with an infrastructure service called the Google Front End, which checks incoming network connections for correct certificates and best practices. The GFE also additionally, applies protections against denial of service attacks. The sheer scale of its infrastructure, enables Google to simply absorb many denial of service attacks, even behind the GFEs. Google also has multi-tier, multi-layer denial of service protections that further reduce the risk of any denial of service impact. Inside Google's infrastructure, machine intelligence and rules warn of possible incidents. Google conducts Red Team exercises, simulated attacks to improve the effectiveness of its responses. Google aggressively limits and actively monitors the activities of employees who have been granted administrative access to the infrastructure. To guard against phishing attacks against Google employees, employee accounts including mine require use of U2F compatible security keys. I don't forget my keys as much as I used to. To help ensure that code is as secure as possible Google stores its source code centrally and requires two-party review of new code. Google also gives its developers libraries that keep them from introducing certain classes of security bugs. Externally, Google also runs a vulnerability rewards program, where we pay anyone who is able to discover and inform us of bugs in our infrastructure or applications.

![104849599-8a535d00-5910-11eb-9b86-d96addab2a1c](https://user-images.githubusercontent.com/46487696/105801437-1fb0ba00-5fbf-11eb-81e4-bca50ac203e1.png)

## Identity and Access Management (IAM)

IAM lets administrators authorize who can take action on specific resources. An IAM policy has a "who" part, a "can do what" part, and an "on which resource" part. The "who" part names the user or users you're talking about. The "who" part of an IAM policy can be defined either by a Google account, a Google group, a Service account, an entire G Suite, or a Cloud Identity domain. The "can do what" part is defined by an IAM role. An IAM role is a collection of permissions. Most of the time, to do any meaningful operations, you need more than one permission. For example, to manage instances in a project, you need to create, delete, start, stop, and change an instance. So the permissions are grouped together into a role that makes them easier to manage.

## Identity and Access Management (IAM)

IAM lets administrators authorize who can take action on specific resources. An IAM policy has a "who" part, a "can do what" part, and an "on which resource" part. The "who" part names the user or users you're talking about. The "who" part of an IAM policy can be defined either by a Google account, a Google group, a Service account, an entire G Suite, or a Cloud Identity domain. The "can do what" part is defined by an IAM role. An IAM role is a collection of permissions. Most of the time, to do any meaningful operations, you need more than one permission. For example, to manage instances in a project, you need to create, delete, start, stop, and change an instance. So the permissions are grouped together into a role that makes them easier to manage.

![105208909-3befc980-5b6f-11eb-8398-9bf33d9f2372](https://user-images.githubusercontent.com/46487696/105801593-73bb9e80-5fbf-11eb-9650-44e780faa5ed.png)
![105208914-3e522380-5b6f-11eb-8f49-27fea89cd04a](https://user-images.githubusercontent.com/46487696/105801596-74eccb80-5fbf-11eb-9a68-e15dc0169b94.png)
![105209846-4eb6ce00-5b70-11eb-9d0b-1565f5c2cb4c](https://user-images.githubusercontent.com/46487696/105801597-75856200-5fbf-11eb-9682-f43fc9a99e26.png)
![105209853-50809180-5b70-11eb-9e62-d70d66d587af](https://user-images.githubusercontent.com/46487696/105801598-761df880-5fbf-11eb-9a95-babf4fe554b1.png)
![105209854-51192800-5b70-11eb-95d3-ba0885ab66c9](https://user-images.githubusercontent.com/46487696/105801599-761df880-5fbf-11eb-80d7-e0bb7c739d88.png)
![105209855-51b1be80-5b70-11eb-80b9-65df5005241f](https://user-images.githubusercontent.com/46487696/105801601-76b68f00-5fbf-11eb-9b78-50b0e2e2121b.png)


## Virtual Private Cloud networks

The Virtual Private Cloud networks that you define have global scope. They can have subnets in any GCP region worldwide and subnets can span the zones that make up a region. This architecture makes it easy for you to define your own network layout with global scope. You can also have resources in different zones on the same subnet. You can dynamically increase the size of a subnet in a custom network by expanding the range of IP addresses allocated to it. Doing that doesn't affect already configured VMs. In this example, your VPC has one network. So far, it has one subnet defined in GCP us-east1 region. Notice that it has two Compute Engine VMs attached to it. They're neighbors on the same subnet even though they are in different zones. You can use this capability to build solutions that are resilient but still have simple network layouts

![105722215-711f6180-5f4b-11eb-9e9f-3c1cf8cc5d4c](https://user-images.githubusercontent.com/46487696/105801684-aa91b480-5fbf-11eb-928a-557bb37e343d.png)
![105722221-72508e80-5f4b-11eb-942d-39ed92442799](https://user-images.githubusercontent.com/46487696/105801687-abc2e180-5fbf-11eb-8b82-23d2ee680840.png)


## Compute Engine

Compute Engine offers managed  Virtual machine=>

* No ufront investment
* fast and consistent performance 
* Create VMs with GCP console or gcloud
* Run images of windows or linux server
* pick persistent disks
* pick local SSd for scratch space too if you need it 
* take disks snapshot as backup or migration tools
* Define a Startup Script


Compute Engine offers innovating pricing=>

* Per-second biling , Sustained use discount
* Preemtible instances
* High throughput to storage at no extra cost
* Customer machine types : Only pay for the hardware you need 


![Screenshot (1171)](https://user-images.githubusercontent.com/46487696/105804512-ff382e00-5fc5-11eb-8ab5-c668a34a84cd.png)
