<p align="center">
  <img src="https://www.especial.gr/wp-content/uploads/2019/03/panepisthmio-dut-attikhs.png" alt="UNIWA" width="150"/>
</p>

<p align="center">
  <strong>UNIVERSITY OF WEST ATTICA</strong><br>
  SCHOOL OF ENGINEERING<br>
  DEPARTMENT OF COMPUTER ENGINEERING AND INFORMATICS
</p>

<hr/>

<p align="center">
  <strong>Cloud Computing and Services</strong>
</p>

<h1 align="center" style="letter-spacing: 1px;">
  Use Cases at CloudSim
</h1>

<p align="center">
  <strong>Vasileios Evangelos Athanasiou</strong><br>
  Student ID: 19390005<br>
</p>

<p align="center">
  Supervisor: Vasileios Mamalis, Professor<br>
  Co-supervisor: Dimitrios Kallergis, Lecturer in Applications
</p>

<p align="center">
  Athens, June 2024
</p>

## Overview

This project explores the simulation of cloud computing environments using the **CloudSim** framework. It focuses on both theoretical and practical analysis of datacenter configurations, **Virtual Machine (VM)** allocation policies, and **Cloudlet** scheduling mechanisms.

---

## Table of Contents

| Section | Title          | Description                                    |
|--------:|----------------|------------------------------------------------|
| assign  | Assignment     | Contains assignments and tasks                 |
| docs    | Documentation  | Project documentation, guides, and notes       |
| src     | Source Code    | All source code files of CloudSim              |

---

## Project Components

### 1. Theoretical Analysis

The project analyzes a specific simulation case (**CloudSimExample6**) in order to understand how cloud resources are provisioned and managed. The main areas of investigation include:

#### Infrastructure Setup
- Detailed breakdown of the simulated **Datacenters**:
  - `Datacenter_0`
  - `Datacenter_1`
- Analysis of their underlying **Hosts** and resource composition.

#### Hardware Specifications
- **Hosts**
  - RAM: 2048 MB  
  - Storage: 1 TB  
  - Bandwidth: 10,000 MB/s  

- **Processing Units (PEs)**
  - Host 0: 4 PEs  
  - Host 1: 2 PEs  
  - Each PE operates at **1,000 MIPS**

#### Virtual Machine (VM) Configuration
- Total requested VMs: **20**
- VM requirements:
  - RAM: 512 MB  
  - Processing Elements: 1 PE  
  - Performance: 1,000 MIPS  

#### Allocation Policies
- Examination of **`VmAllocationPolicySimple`**  
- Uses a **Worst-Fit policy**, selecting the host with the fewest Processing Elements currently in use.

---

### 2. Practical Implementation & Exercises

The project includes a set of experimental scenarios designed to test the flexibility and limitations of the CloudSim simulator:

#### Policy Comparisons
- Execution of simulations using different scheduling strategies:
  - **Space-Sharing**
  - **Time-Sharing**
- Applied at both levels:
  - Cloudlets-to-VMs
  - VMs-to-Hosts

#### Resource Optimization
- Modification of:
  - Host attributes
  - Number of Processing Elements
  - Number of Hosts
- Goal: Ensure that all **20 VMs** can be executed without resource over-subscription.

#### Code Intervention
- Identification of specific sections in the **CloudSim source code** where:
  - Custom VM allocation policies
  - Custom Cloudlet scheduling algorithms  
  can be implemented.

---

## Summary of Resources (CloudSimExample6)

| Resource          | Quantity        | Key Attributes |
|-------------------|-----------------|----------------|
| Datacenters       | 2               | Architecture: x86, OS: Linux, VMM: Xen |
| Hosts             | 2 per Datacenter| 2048 MB RAM, 1000 MIPS per PE |
| Virtual Machines  | 20              | 512 MB RAM, 1000 MIPS, 1 PE |
| Cloudlets         | Multiple        | Assigned to VMs using specific scheduling algorithms |

---

## Installation and Run Guide

### Prerequisites

- **CloudSim Framework**: Ensure the [CloudSim 4.0 framework](https://github.com/Cloudslab/cloudsim/releases) is installed and configured.
- **Java Development Kit (JDK)**: A compatible version of JDK (8 or higher) is required.
- **IDE**: An integrated development environment (IDE) for Java development.

---

### Install

Clone the Repository
Download the repository to your local machine:
```
git clone https://github.com/Cloud-Computing-and-Services/CloudSim.git
```

### Run
Open the project in IDE for Java Development such as Eclipse

From package `/cloudsim-examples/src/main/java/org/cloudbus/cloudsim/examples/` run `CloudSimExample6.java` to see the simulation
