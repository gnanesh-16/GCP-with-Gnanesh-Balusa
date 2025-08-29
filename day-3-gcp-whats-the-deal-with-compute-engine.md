# Day-3 GCP What's the Deal with Compute Engine?

## Day 3 Notes: What's the Deal with Compute Engine?

_Alright, welcome to Day 3! Today I'm going to talk about one of the most basic and powerful services in GCP: **Compute Engine**. If you've ever heard of "virtual machines" or "VMs," this is it. Let's break it down in a simple way._

<figure><img src=".gitbook/assets/image (2) (1).png" alt=""><figcaption></figcaption></figure>

#### **1. What Exactly is Compute Engine?** _Your Server in the Cloud_

Think of Compute Engine as renting a computer in one of Google's data centers. Instead of buying a physical server (a big, noisy machine), you can create a **Virtual Machine (VM)** on Google's hardware in just a few minutes.

This VM is basically your own private server. You can choose its configuration—how much RAM, how many CPUs, what operating system (like Linux or Windows)—and you get complete control over it.

_**Key takeaway:**_ _Compute Engine lets you create and run Virtual Machines (servers) on Google's infrastructure. It's the foundation for running all sorts of applications._

#### **2. Main Parts of a VM** _The Building Blocks_

When you create a VM, you're essentially choosing the parts for your virtual computer. Here are the main things you'll configure:

* _**Machine Family & Type:**_ This is like choosing the model of your computer. GCP offers different families for different jobs:
  * **General-Purpose (E2, N2):** Good for everyday tasks, like websites and small applications. E2 is the most cost-effective.
  * **Compute-Optimized (C2):** These have powerful CPUs, perfect for gaming servers or tasks that need a lot of processing power.
  * **Memory-Optimized (M2):** These have huge amounts of RAM, ideal for large databases or in-memory analytics.
* _**Boot Disk:**_ This is the hard drive where your operating system is installed. You can choose the OS (like Ubuntu, Debian, Windows Server) and the size of the disk.
* _**Networking (VPC):**_ Every VM is connected to a Virtual Private Cloud (VPC) network. This is your own private, isolated network space within GCP that allows your VMs to talk to each other and the internet securely.

#### **3. How is it Priced?** _Understanding the Costs_

One of the best things about the cloud is flexible pricing. With Compute Engine, you mainly have three options:

* _**On-Demand:**_ This is the standard, pay-as-you-go price. You pay for the seconds you use the VM, with no commitment. Simple and flexible.
* _**Committed Use Discounts (CUDs):**_ If you know you're going to run a VM for a long time (like 1 or 3 years), you can "commit" to using it. In return, Google gives you a big discount—up to 70%!
* _**Spot VMs:**_ These are super cheap (up to 91% off!) but come with a catch: Google can shut them down at any time if they need the resources. They are perfect for tasks that can be interrupted, like batch processing.

_**Key takeaway:**_ _You don't have to stick to one price. Use Committed Use Discounts for your stable, long-running applications to save a lot of money._

#### **4. Creating Your First VM (The Demo)**

The video shows a practical demo of creating a VM. The basic steps are:

1. **Go to Compute Engine** in the GCP Console.
2. **Click "Create Instance."**
3. **Give it a name** and choose a **Region** and **Zone** (pick one close to your users!).
4. **Select the Machine Family and Type** (the demo uses an `e2-micro`, which is in the free tier).
5. **Choose a Boot Disk** (like Debian Linux).
6. **Allow HTTP/HTTPS traffic** if you're running a web server.
7. **Click "Create,"** and in a minute, your server is ready!

_And that's the funda of Compute Engine! You now know what a VM is, what it's made of, and how to get one running. In the next lessons, we'll build on this knowledge. See you there!_
