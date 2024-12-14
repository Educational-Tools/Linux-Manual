# Linux School Server

!!! note
    This manual is available in a PDF format and can be downloaded and printed.<br>
    [:fontawesome-solid-file-pdf: Download the PDF](https://educational-tools.github.io/Linux-Manual/linux_man.pdf){.md-button}

## What is LTSP?
Let's begin with the core concept of a Linux School Server, often implemented using the [Linux Terminal Server Project](https://ltsp.org/), or LTSP. Imagine a classroom full of computers, each needing its own operating system, software installations, and updates. This can quickly become a management headache and a significant expense. LTSP offers a more efficient solution. It allows multiple student workstations, which we'll refer to as "fat clients" in this manual (meaning they have their own local processing power), to boot and operate using resources from a single, powerful central server. [More Info](https://en.wikipedia.org/wiki/Linux_Terminal_Server_Project)

Instead of each computer running its own full operating system from its local hard drive, the fat clients primarily use their own hardware for processing tasks, while the server provides the core operating system, applications, and user data over the network. This setup transforms the network into a shared computing environment. When a student turns on their computer, it connects to the server, which provides the necessary files to start the desktop environment. The actual applications run on the client machine itself, thus the name "fat client".

This approach brings several key advantages:

  * Cost Savings: By centralizing the operating system and applications on a single server, you reduce the need for high-end hardware on each student workstation. You can often repurpose older computers as fat clients, saving on hardware costs. Additionally, software licensing costs are reduced as you only need to license software for the server, not for each individual machine (depending on the licensing model of the software used).
  * Easier Deployment: Installing and configuring software becomes significantly simpler. You only need to install and update software on the central server, and all client machines automatically benefit from these changes. This eliminates the need to individually configure and maintain each workstation.
  * Centralized Management: Managing user accounts, software updates, and system configurations becomes much more efficient. Administrators can control the entire network from a single point, simplifying tasks like applying security patches, installing new software, and managing user access. This saves valuable time and resources for IT staff.

This centralized approach greatly simplifies IT management in a school environment, making it easier to provide consistent and up-to-date software for all students while reducing costs and administrative overhead.

## LMDE not Ubuntu!
Now, let's discuss why we've chosen Linux Mint Debian Edition (LMDE) as the server operating system for our Linux School Server, rather than Ubuntu Mate, which is sometimes used in similar setups. Both are excellent Linux distributions, but LMDE offers some distinct advantages that make it particularly well-suited for this purpose.

A crucial factor in our decision is the underlying base of each distribution. Ubuntu Mate is based on Ubuntu, which in turn is based on Debian. While Ubuntu is a popular and user-friendly distribution, it has increasingly adopted "snap" packages. Snaps are containerized software packages that bundle all their dependencies, aiming to simplify software installation and updates. However, they have also introduced some concerns, especially in server environments:

* Resource Consumption: Snap packages can often consume more disk space and system resources compared to traditional Debian packages (.deb). This can be a concern on a server serving multiple clients, potentially impacting performance.
* Background Processes: Snaps often run background services that might not be necessary in a server environment, further contributing to resource usage.
* Integration with the System: Snaps operate in a more isolated environment, which can sometimes lead to integration issues with the rest of the system, particularly in server-specific configurations.
* Control over Updates: Snap updates are often automatic and can be less granularly controlled than traditional package updates, which might not be desirable in a stable server environment where administrators prefer to manage updates carefully.

LMDE, on the other hand, is directly based on Debian, a distribution renowned for its stability and long-term support. This direct Debian base provides several benefits:

* Stability: Debian is known for its rigorous testing and stable release cycle, ensuring a reliable and predictable server environment.
* Performance: Utilizing traditional .deb packages, LMDE generally offers better performance and resource efficiency compared to systems relying heavily on snaps.
* Control: Administrators have fine-grained control over software updates and system configurations, allowing for a more tailored and stable server setup.
* Familiar Package Management: The use of the apt package manager, familiar to many Linux users, makes software installation and management straightforward.

In summary, while Ubuntu Mate is a fine desktop operating system, the increasing prevalence of snap packages and their associated issues make LMDE a more suitable and efficient choice for our Linux School Server. Its Debian base provides the stability, performance, and control that are crucial for a reliable and manageable server environment.