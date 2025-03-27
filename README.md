# SEA:ME Project - Mixed Criticality System

- [SEA:ME Project - Hypervisor](#-seame-project---Hypervisor)
  - [Introduction](#introduction)
  - [Background Information](#background-information)
  - [Project Goals and Objectives](#project-goals-and-objectives)
  - [System Architecture](#system-architecture)
  - [Project Timeline](#project-timeline)
  - [Submission](#submission)
  - [References](#references)

## Introduction

Recent vehicles are making efforts to adopt Zonal Architecture rather than the conventional ECU placement that centers on functionalities. In this context, secure isolation between different system domains is essential for a single controller to meet diverse safety requirements of multiple systems. To achieve this, there have been continuous efforts to introduce hypervisor technology—originally used in servers—into vehicles, aiming to accomplish safe data transfer between different domains while minimizing performance degradation.
This project aims to integrate the Cluster Qt application and the PDC-System into a Mixed Criticality System (MCS). Both systems, developed in the previous project, will be separated into different domains on a single RPi using a hypervisor, and exchanged data through interdomain communication.
</br>


## Background Information

The [meta-virtualization](https://layers.openembedded.org/layerindex/branch/master/layer/meta-virtualization/) layer provided by the Yocto project supplies virtualization technologies such as Xen, KVM, Libvirt and others, along with the necessary packages for building virtualized systems. Students can implement a basic virtualization platform using several recipes from the meta-virtualization layer, and port the system implemented in a previous project to MCS.
</br>


## Project Goals and Objectives

The goals and objectives of the project are as follows:

1. Execute the Cluster application and the PDC-System on separate Linux virtual domain using hypervisor.
2. Transfer ultrasonic sensor data and control results to the Cluster application using interdomain communication protocol.
3. Optimize the system to minimize the overhead and performance degradation caused by hardware virtualization.
</br>


## System Architecture

![Example system architecture](https://github.com/user-attachments/assets/439234e3-07ed-4109-a104-6f0aac6722a3)
</br>


## Project Timeline

 The following is a sample project timeline:
 
 1. Week 1: Study about the virtualization and analyze the technical requirements of the project.
 2. Week 2: Build a basic linux image that runs on a hypervisor, rather than on the hardware itself and configure the network settings.
 3. Week 3-4: Integrate your Cluster application into a virtual machine and run application using various qt plugins (vnc, linuxfb, etc.).
 4. Week 5-6: Integrate your PDC-System into a virtual machine that supports a real-time environment such as rt linux.
 5. Week 7: Implement a interdomain communication between Cluster and PDC-System, output sensor data and control results to the cluster.
 6. Week 8-10: Analyze and optimize system performance from various perspectives, including responsiveness, stability, and safety.
 7. Week 11-12: Final preparation and submission. Participants should use this time to finalize their project reports, document their code, and prepare their submissions. The final project submissions are due at the end of week 12.
</br>


## Submission

Upon completion of the project, participants should submit a GitHub repository that includes the following components:

1. Software Code: Participants should provide the source code for their systems, including the system configurations and applications. The code should be well-documented, with clear explanations of the algorithms and techniques used.
2. Performance Results: Participants should provide a comparison of the overall performance measurement results with the previous system. This may include screenshots or videos in action, as well as metrics and statistics that measure the performance.
3. Project Report: Participants should provide a project report that describes their experience with the project, including any challenges faced and how they were overcome. The report should also include a discussion of the algorithms and techniques used, aswell as the results and conclusions of the project.

By providing these components, the participants will demonstrate their understanding of the concepts and techniques involved in the project, and will provide evidence of their ability to implement a virtualization system. The GitHub repository will serve as a portfolio of the participants' work, and will provide a record of their achievements and contributions to the field of embedded systems.
</br>


## References

* Yocto Project. (2021). Yocto Project. https://www.yoctoproject.org/
* Qt Project. (2021). Qt Project. https://www.qt.io/
* Raspberry Pi Foundation. (2021). Raspberry Pi. [https://www.raspberrypi.org/](https://www.raspberrypi.org/)
* CAN specification documents: These documents provide detailed information on the CAN (Controller Area Network) protocol and its implementation.
* VsomIp/Autosar documents: These documents provide information on the Inter-Process Communication (IPC) frameworks VsomIp and Autosar and their implementation in the automotive industry.
* meta-virtualization: This layer provides support for virtualization. [meta-virtualization](https://layers.openembedded.org/layerindex/branch/master/layer/meta-virtualization/)
</br>
