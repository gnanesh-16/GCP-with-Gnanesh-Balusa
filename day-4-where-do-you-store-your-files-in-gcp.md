# Day-4 Where Do You Store Your Files in GCP?

_Hey everyone, welcome to Day 4! Today, we're going to talk about something we all need: **storage**. Whether it's photos, videos, or application data, you need a place to keep it. In GCP, you have a few great options, so let's understand what they are and when to use them._

<figure><img src=".gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

#### **1. Cloud Storage: Your "Google Drive" for Everything**

The simplest way to think about **Google Cloud Storage** is that it's like a massive, super-powered Google Drive or Dropbox. It's a place where you can store pretty much any kind of file or object.

You store your files in something called a **bucket**. You can think of a bucket as a main folder. A key thing to remember is that bucket names have to be **globally unique** meaning no one else in the entire world can have a bucket with the same name as yours!

_**Key takeaway:**_ _Cloud Storage is for unstructured data_&#x20;

_things like images, videos, backups, and log files. It's incredibly scalable and you only pay for what you store._

#### **2. Storage Classes: How to Save Money**

Not all data is the same. Some files you need instantly, while others you might only look at once a year. Cloud Storage lets you choose a "Storage Class" for your data to save money.

* _**Standard:**_ This is for "hot" data that you access all the time, like images for a popular website. It's the fastest but costs the most to store.
* _**Nearline:**_ For data you access less than once a month, like monthly backups. Storage is cheaper, but there's a small fee to retrieve the data.
* _**Coldline:**_ For data you access less than once every 90 days. Storage is even cheaper.
* _**Archive:**_ This is the cheapest option, for long term "cold" storage, like legal archives or data you might need years from now. You access it less than once a year.

_**Key takeaway:**_ _By choosing the right storage class based on how often you need your data, you can significantly cut down your storage costs._

#### **3. Persistent Disk: The Hard Drive for Your VM**

In the last lesson, we talked about Compute Engine and VMs. Well, a **Persistent Disk** is the hard drive that attaches to your VM. It's where you install your operating system and store the files that your application needs to access quickly.

It's called "persistent" because the data stays there even if you shut down or delete your VM. You can think of it like an external hard drive that you can plug into different computers.

_**Key takeaway:**_ _Persistent Disk is block storage that acts as the local hard drive for your Virtual Machines. It's fast and reliable for your active applications._

#### **4. Filestore: A Shared Folder for Your VMs**

Imagine you have multiple VMs that all need to access and modify the same set of files at the same time. That's where **Filestore** comes in. It provides a managed network file system (NFS) that you can "mount" on multiple VMs.

It works just like a shared network drive in an office. Any change one VM makes to a file is instantly visible to all the other VMs connected to it.

_**Key takeaway:**_ _Use Filestore when you need a shared file system for multiple applications or VMs to use simultaneously._

_And that's a wrap for Day 4! You now have a clear picture of the main storage services in GCP. Next time, we'll dive into another core topic. See you then!_
