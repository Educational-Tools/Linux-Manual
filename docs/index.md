# Linux School Server

!!! note
    This manual is available in a PDF format and can be downloaded and printed.<br>
    [:fontawesome-solid-file-pdf: Download the PDF](https://educational-tools.github.io/Linux-Manual/linux_man.pdf){.md-button}

## **What is LTSP?**
Let's begin with the core concept of a Linux School Server, often implemented using the [Linux Terminal Server Project](https://ltsp.org/), or LTSP. Imagine a classroom full of computers, each needing its own operating system, software installations, and updates. This can quickly become a management headache and a significant expense. LTSP offers a more efficient solution. It allows multiple student workstations, which we'll refer to as "fat clients" in this manual (meaning they have their own local processing power), to boot and operate using resources from a single, powerful central server. [More Info](https://en.wikipedia.org/wiki/Linux_Terminal_Server_Project)

Instead of each computer running its own full operating system from its local hard drive, the fat clients primarily use their own hardware for processing tasks, while the server provides the core operating system, applications, and user data over the network. This setup transforms the network into a shared computing environment. When a student turns on their computer, it connects to the server, which provides the necessary files to start the desktop environment. The actual applications run on the client machine itself, thus the name "fat client".

This approach brings several key advantages:

  * Cost Savings: By centralizing the operating system and applications on a single server, you reduce the need for high-end hardware on each student workstation. You can often repurpose older computers as fat clients, saving on hardware costs. Additionally, software licensing costs are reduced as you only need to license software for the server, not for each individual machine (depending on the licensing model of the software used).
  * Easier Deployment: Installing and configuring software becomes significantly simpler. You only need to install and update software on the central server, and all client machines automatically benefit from these changes. This eliminates the need to individually configure and maintain each workstation.
  * Centralized Management: Managing user accounts, software updates, and system configurations becomes much more efficient. Administrators can control the entire network from a single point, simplifying tasks like applying security patches, installing new software, and managing user access. This saves valuable time and resources for IT staff.

This centralized approach greatly simplifies IT management in a school environment, making it easier to provide consistent and up-to-date software for all students while reducing costs and administrative overhead.