# Identification of Cloud Infrastructure Components

## 1. Compute Resources

* **Purpose:** Process instructions, run applications, and execute workloads using the available CPU resources.
* **Importance in Cloud:** Provides the processing power required to run applications, services, and virtualized workloads in a cloud environment.
* **KillerCoda Relation:** Represented by the virtualized CPU allocated to the Ubuntu environment, with **1 CPU core** available for processing tasks.

## 2. Storage Resources

* **Purpose:** Store the operating system, applications, files, and other data required by the system.
* **Importance in Cloud:** Provides the storage capacity needed for operating systems, applications, user data, and system files.
* **KillerCoda Relation:** Represented by the **19 GB** disk storage available to the Ubuntu environment, including the `/dev/vda1` partition mounted as the root filesystem.

## 3. Networking Resources

* **Purpose:** Enable communication between the system, other services, and connected network resources.
* **Importance in Cloud:** Allows cloud systems to communicate with internal and external services and supports data transmission between resources.
* **KillerCoda Relation:** Represented by the network interfaces and private IP addresses assigned to the Ubuntu environment, including **172.30.1.2** and **172.17.0.1**.

## 4. Operating System

* **Purpose:** Manage system resources, provide an environment for applications, and control access to hardware and software resources.
* **Importance in Cloud:** Provides the foundation for running applications and managing cloud-based workloads in a stable and controlled environment.
* **KillerCoda Relation:** Represented by **Ubuntu 24.04.4 LTS**, running on the Linux kernel version **6.8.0-138-generic**.

## 5. Memory Resources

* **Purpose:** Temporarily store data and instructions that are actively being used by running processes and applications.
* **Importance in Cloud:** Provides the memory required for applications and services to operate efficiently.
* **KillerCoda Relation:** Represented by the **1.9 GB of RAM** allocated to the Ubuntu environment.

## 6. Virtualization

* **Purpose:** Allows physical computing resources to be divided into virtual resources that can be used by separate environments.
* **Importance in Cloud:** Enables efficient resource allocation, isolation, scalability, and flexible management of computing environments.
* **KillerCoda Relation:** Represented by the virtualized Ubuntu environment provided through the KillerCoda cloud laboratory platform.
