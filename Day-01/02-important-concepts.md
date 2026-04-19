# Vocabulary in Cloud Computing

## Virtualization

Virtualization is the process of creating a virtual version of something, such as an operating system, server, storage, or network resources.

Virtualization = Creating multiple virtual systems on one physical machine

💡 Example:
1 powerful computer → behaves like 5 separate computers

##Hypervisor 

Hypervisor = Software (or firmware) that creates and manages Virtual Machines (VMs)

👉 It sits between:
Physical hardware (CPU, RAM, disk)
Virtual machines (guest OS)

👉 Its job:
Divide resources
Allocate them to VMs
Keep VMs isolated

⚙️How Hypervisor Works (Step-by-Step)
You create a VM (e.g., Ubuntu on Azure)
Hypervisor:
Allocates CPU cores
Allocates RAM
Allocates storage
VM runs like a real computer
Multiple VMs share same hardware safely

👉 Without hypervisor → cloud doesn’t exist

🔥 Types of Hypervisors
🥇 Type 1 (Bare Metal Hypervisor)
Runs directly on hardware (no OS in between)

🧠 Structure:

Hardware → Hypervisor → VMs

✅ Advantages:
High performance
More secure
Used in cloud data centers
💡 Real Examples:
VMware ESXi
Microsoft Hyper-V
Xen

🥈 Type 2 (Hosted Hypervisor)
Runs on top of an existing OS

🧠 Structure:

Hardware → Host OS → Hypervisor → VMs

❌ Disadvantages:
Slower than Type 1
Depends on host OS
💡 Real Examples:
Oracle VirtualBox
VMware Workstation

## Virtual Machine

A Virtual Machine (VM) is a software-based emulation of a physical computer. It allows running multiple operating systems on a single physical machine.

## API (Application Programming Interface)

API is a set of rules and protocols that allows different software applications to communicate with each other. It defines how software components should interact.

We can access application and or Azure User interface with the help of Shell scripting and python programmatically we can say with the help of API ...

## Regions

Regions in cloud computing refer to geographic locations where cloud providers have data centers. Each region contains multiple data centers.

In same regions thera rae availability zones or data centers all data center have replicas (Copy) of the applications in case of 1 data center shuts down load balancer sends the request to the another data center 

LB Deploys the copies of app in different AZs and LB splits the load between the copies 

## Availability Zones

Availability Zones are isolated locations within a region that have their own power, cooling, and networking. They are designed to provide high availability and fault tolerance.

## Scalability

Scalability is the ability of a system to handle an increasing amount of work or its potential to be enlarged to accommodate that growth.

Types:-
1. Horizontal scaling
2. vertical scaling
3. Dynamic Scaling

## Auto-scaling 

Auto Scaling = Automatically increasing or decreasing resources (servers/VMs) based on demand

👉 Goal:
Handle traffic efficiently
Avoid crashes
Reduce cost

## Elasticity

Elasticity in cloud computing refers to the ability to **dynamically scale** resources up or down based on demand.

## Agility

Agility is the capability of quickly and easily adapting to changes. In the context of cloud computing, it involves the rapid deployment of resources and applications.

## High Availability

High Availability (HA) ensures that a system or application is operational and accessible for a high percentage of time, typically 99.9% or higher.

## Fault Tolerance

Fault Tolerance is the ability of a system to continue operating without interruption in the presence of hardware or software failures.

## Disaster Recovery

DR is a technique or mechanism where we need to plan if something goes wrong....

Disaster Recovery involves the planning and processes for restoring and recovering data and systems after a natural or human-induced disaster.

## Load Balancing

Load Balancing is the distribution of network traffic or computing workload across multiple servers to ensure no single server is overwhelmed.

Load Balancer = Distributes traffic across multiple servers

💡 Example:

1000 users visit website
→ Load balancer sends:

300 to Server A
300 to Server B
400 to Server C

👉 Prevents overload

LB Deploys the copies of app in different AZs and LB splits the load between the copies 

[Load balancer topic in detail for interview questions...]

Refer college notes for theory ..
subjects:- CN
           VAPT
           Cloud Computing
           virtualization 
           cloud orchestration 
           
           
