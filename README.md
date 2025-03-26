# SEA:ME Project - Hypervisor

- [\*\* SEA:ME Project - Hypervisor\*\*](#-seame-project---Hypervisor)
  - [Introduction](#introduction)
  - [Project Goals and Objectives](#project-goals-and-objectives)
  - [Technical Requirements](#technical-requirements)
  - [System Architecture](#system-architecture)
  - [Implementation](#implementation)
  - [Project Timeline](#project-timeline)
  - [Submission](#submission)
  - [References](#references)

## Introduction

Recent vehicles are making efforts to adopt Zonal Architecture rather than the conventional ECU placement that centers on functionalities. In this context, secure isolation between different system domains is essential for a single controller to meet diverse safety requirements of multiple systems. To achieve this, there have been continuous efforts to introduce hypervisor technology—originally used in servers—into vehicles, aiming to accomplish safe data transfer between different domains while minimizing performance degradation.
This project aims to integrate the Cluster Qt application and the PDC-System into a Mixed Criticality System. Both systems, developed in the previous project, will be separated into different domains on a single RPi using a hypervisor, and exchanged data through interdomain communication.
</br>


## Project Goals and Objectives

The goals and objectives of the project are as follows:

1.  * Cluster application과 PDC-System를 서로 다른 리눅스 OS로 분리하여 실행
2.  * interdomain communication을 구현하여 ultrasonic sensor의 데이터 및 제어 결과를 Cluster application으로 전달
3.  * 하드웨어 가상화로 인한 오버헤드 및 성능 저하를 최소화하도록 시스템 최적화
</br>


## Technical Requirements
* Cluster application과 PDC-System를 서로 다른 리눅스 OS로 분리하여 실행
* interdomain communication을 구현하여 ultrasonic sensor의 데이터 및 제어 결과를 Cluster application으로 전달
* 하드웨어 가상화로 인한 오버헤드 및 성능 저하를 최소화하도록 시스템 최적화
</br>


## System Architecture

</br>


## Implementation

</br>


## Project Timeline
 
</br>


## Submission

</br>


## References

* Yocto Project. (2021). Yocto Project. https://www.yoctoproject.org/
* Qt Project. (2021). Qt Project. https://www.qt.io/
* Raspberry Pi Foundation. (2021). Raspberry Pi. [https://www.raspberrypi.org/](https://www.raspberrypi.org/)
* CAN specification documents: These documents provide detailed information on the CAN (Controller Area Network) protocol and its implementation.
* VsomIp/Autosar documents: These documents provide information on the Inter-Process Communication (IPC) frameworks VsomIp and Autosar and their implementation in the automotive industry.
* meta-virtualization: This layer provides support for virtualization. [meta-virtualization](https://layers.openembedded.org/layerindex/branch/master/layer/meta-virtualization/)
</br>
