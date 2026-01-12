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
  Student ID: 19390005
</p>

<p align="center">
  <a href="https://github.com/Ath21" target="_blank">GitHub</a> ·
  <a href="https://www.linkedin.com/in/vasilis-athanasiou-7036b53a4/" target="_blank">LinkedIn</a>
</p>

<p align="center">
  Supervisor: Vasileios Mamalis, Professor
</p>
<p align="center">
  <a href="https://ice.uniwa.gr/en/emd_person/vassilios-mamalis/" target="_blank">UNIWA Profile</a>
</p>

<p align="center">
  Co-supervisor: Dimitrios Kallergis, Lecturer in Applications
</p>
<p align="center">
  <a href="https://ice.uniwa.gr/en/emd_person/20972/" target="_blank">UNIWA Profile</a> ·
    <a href="https://www.linkedin.com/in/dkallergis/" target="_blank">LinkedIn</a>
</p>

<p align="center">
  Athens, June 2024
</p>

---

# Project Overview

This project explores the simulation of cloud computing environments using the **CloudSim** framework. It focuses on both theoretical and practical analysis of datacenter configurations, **Virtual Machine (VM)** allocation policies, and **Cloudlet** scheduling mechanisms.

---

## Table of Contents

| Section | Folder / File | Description |
|------:|---------------|-------------|
| 1 | `assign/` | Assignment material for the CloudSim course |
| 1.1 | `assign/ASSIGNMENT #1.pdf` | Assignment description in English |
| 1.2 | `assign/ΕΡΓΑΣΙΑ #1.pdf` | Assignment description in Greek |
| 2 | `cloudsim-cloudsim-4.0/` | Main CloudSim 4.0 library source and build files |
| 2.1 | `cloudsim-cloudsim-4.0/src/main/resources/` | Build and project resources (`pom.xml`, `build.xml`, `readme.txt`, etc.) |
| 2.2 | `cloudsim-cloudsim-4.0/src/main/java/org/cloudbus/cloudsim/` | Core CloudSim classes, including: |
| 2.2.1 | `container/` | Container-based simulation: policies, provisioners, VM selection, scheduling |
| 2.2.2 | `core/` | Core simulation classes: CloudSim engine, SimEntity, SimEvent, predicates |
| 2.2.3 | `distributions/` | Statistical distributions for simulation (Uniform, Exponential, etc.) |
| 2.2.4 | `lists/` | Utility lists for Cloudlets, Hosts, VMs, PEs |
| 2.2.5 | `network/datacenter/` | Network-aware datacenter simulation classes |
| 2.2.6 | `power/` | Power-aware datacenter simulation classes and VM allocation policies |
| 2.2.7 | `provisioners/` | RAM, BW, PE provisioners for VMs and Containers |
| 2.2.8 | `util/` | Utility classes for workload, math, and execution measurement |
| 2.2.9 | `vmSelectionPolicies/` | Power VM selection policies |
| 2.3 | `cloudsim-cloudsim-4.0/src/test/java/org/cloudbus/cloudsim/` | Unit tests for all major modules (lists, power, provisioners, schedulers) |
| 2.4 | `cloudsim-cloudsim-4.0/target/` | Compiled classes and Maven metadata |
| 3 | `cloudsim-examples/` | Example simulations using CloudSim 4.0 |
| 3.1 | `cloudsim-examples/src/main/java/org/cloudbus/cloudsim/examples/container/` | Container simulation examples |
| 3.2 | `cloudsim-examples/src/main/java/org/cloudbus/cloudsim/examples/network/datacenter/` | Network simulation examples |
| 3.3 | `cloudsim-examples/src/main/java/org/cloudbus/cloudsim/examples/power/` | Power-aware simulation examples (PlanetLab and Random traces) |
| 3.4 | `cloudsim-examples/src/main/resources/` | Example datasets for simulations (`.dat`, `.swf.gz`) |
| 4 | `docs/` | Documentation and use-case PDFs |
| 4.1 | `docs/Use-Cases-at-CloudSim.pdf` | English version |
| 4.2 | `docs/Σενάρια-Χρήσης-στο-CloudSim.pdf` | Greek version |
| 5 | `README.md` | Repository overview and instructions |

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

# Installation and Run Guide

## Prerequisites

- **CloudSim Framework**: Ensure the [CloudSim 4.0 framework](https://github.com/Cloudslab/cloudsim/releases) is installed and configured.
- **Java Development Kit (JDK)**: A compatible version of JDK (8 or higher) is required.
- **IDE**: An integrated development environment (IDE) for Java development.

---

## Install

Clone the repository to your local machine:
```
git clone https://github.com/Cloud-Computing-and-Services/CloudSim.git
```

### Run
Open the project in IDE for Java Development such as Eclipse

From package `/cloudsim-examples/src/main/java/org/cloudbus/cloudsim/examples/` run `CloudSimExample6.java` to see the simulation
