# Day-2  GCP Hierarchy & Avoiding Surprising Costs

_Welcome back! Today, for Day 2, we're getting into the really important stuff: how to properly structure everything in GCP and, most importantly, how to make sure you don't get any surprise bills. Chalo, let's get started._

<figure><img src=".gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

#### **1. Why Does This Hierarchy Matter?** _The Plan for Your Cloud Setup_

Think about it, if you build a house without a proper plan, it's going to be a mess, right? The GCP Hierarchy is exactly that the plan for your cloud setup. Keeping it well organized is super important for two big reasons:

* _**Seeing Your Costs Clearly:**_ It lets you see exactly where your money is going. You can track spending for each team (like a Payments Team), for different environments (like Production vs. Development), or even for one specific service.
* _**Cutting Down Costs:**_ Once you can clearly _see_ where you're spending, you can start to _reduce_ it. A good hierarchy helps you find and remove any resources that are just wasting money.

_**Key takeaway:**_ _A proper hierarchy isn't just for keeping things tidy; it's a basic funda for controlling your cloud costs._

#### **2. The GCP Hierarchy, Explained Simply** _From Top to Bottom_

GCP arranges everything in a simple top-to-bottom structure.

* _**Organization:**_ This is the main root level, usually connected to your company's official account (like `gnaneshbalusa.in`). If you're using the free trial, you won't have this level; you'll start directly with Projects.
* _**Folders:**_ This is the best way to group your projects. A very common and useful method is to use folders to keep your **Development**, **Staging**, and **Production** environments separate. This way, you don't accidentally make a change in dev that breaks your live production site.
* _**Projects:**_ Now, this is where all the action happens! A project is basically a box where you keep all your GCP services. You can have one project for your payments team, another for your UI team, and so on.
* _**Resources:**_ These are the actual services you use inside a project, like your **Virtual Machines**, **Databases**, and **Storage Buckets**.

#### **3. Billing Accounts & Budget Alerts** _Your Financial Safety Net_

Controlling your spending is probably the most important thing in the cloud.

* _**Billing Accounts:**_ This is the account used to pay for everything you use. You can link one billing account to many projects, which makes payment easy. For your free trial, this is set up for you automatically.
* _**Budget Alerts:**_ This is your best friend, seriously. It will save you from getting a shock at the end of the month! You can set a monthly budget for your project and tell GCP to send you an email when you've spent **50%**, **90%**, and **100%** of that budget. This way, you always know where you stand.

_**Key takeaway:**_ _My advice? Setting up budget alerts is a must-do. Don't even think of it as optional, whether you're just starting or you're a pro._

#### **4. Enabling APIs** _Just Switching It On_

Simple point here: before you can use any GCP service (like creating a Virtual Machine), you have to first **enable its API** inside your project. It's just like switching on the power for that service, allowing it to be used.

_And that's it for Day 2! Now you have a solid idea of how to structure your GCP setup and keep an eye on your expenses. See you in the next lesson!_
