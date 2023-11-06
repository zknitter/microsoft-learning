# Microsoft Learning
This repository contains notes and learning resources for Microsoft software. It is intended to serve both as an annotated study guide for the relevant exams and as a persistent resource for ongoing documentation.

# Contents
* [AZ-900: Microsoft Azure Fundamentals](#az-900-microsoft-azure-fundamentals)

# AZ-900: Microsoft Azure Fundamentals

* [Exam URL](https://learn.microsoft.com/en-us/credentials/certifications/exams/az-900/)
* [Study Guide URL](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/az-900)
* [Journey PDF](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4AElB)
* [Certification URL](https://learn.microsoft.com/en-us/credentials/certifications/azure-fundamentals/)

## Overview

As a candidate for this exam, you’re a technology professional who wants to demonstrate foundational knowledge of cloud concepts in general and Microsoft Azure in particular. This exam is a common starting point in a journey towards a career in Azure.

You can describe Azure architectural components and Azure services, such as:

* Compute
* Networking
* Storage

You can also describe features and tools to secure, govern, and administer Azure.

You should have skills and experience working with an area of IT, such as:

* Infrastructure management
* Database management
* Software development

## Study Guide

This section captures skills measured as of July 31, 2023.

### Audience profile
Candidates for this exam are technology professionals who want to demonstrate foundational knowledge of cloud concepts in general and Azure in particular. This certification is a common starting point in a journey towards a career in Azure.

These professionals can describe Azure architectural components and Azure services, such as compute, networking, and storage. They can also describe features and tools to secure, govern, and administer Azure.

Candidates for this exam have skills and experience working with an area of information technology (IT), such as infrastructure management, database management, or software development.

* Describe cloud concepts (25–30%)
* Describe Azure architecture and services (35–40%)
* Describe Azure management and governance (30–35%)

### Describe cloud concepts (25–30%)

**Learning Path** :point_right: [Microsoft Azure Fundamentals: Describe cloud concepts](https://learn.microsoft.com/en-us/training/paths/microsoft-azure-fundamentals-describe-cloud-concepts/)

#### Describe cloud computing

**Learning Module** :point_right: [Describe cloud computing](https://learn.microsoft.com/en-us/training/modules/describe-cloud-compute/)

| **Task** | **Status** |
|:----|:----:|
|  Read content | :white_check_mark: |
|  Took notes | :white_check_mark: |
|  Reviewed/revised notes | :no_entry_sign: |

**Objectives**

* [Define cloud computing](#cloud-computing)
* [Describe the shared responsibility model](#the-shared-responsibility-model)
* [Define cloud models, including public, private, and hybrid](#cloud-models)
* [Identify appropriate use cases for each cloud model](#cloud-models)
* [Describe the consumption-based model](#the-consumption-based-model)
* [Compare cloud pricing models](#cloud-pricing-models)
* ~~Describe serverless~~ (NOTE: Serverless computing was not described in this module)

##### Cloud Computing

**Cloud computing** is defined as the delivery of computing services over the Internet. 

The main difference between cloud computing and traditional hosting models is that cloud computing allows for rapid scaling in response to increasing or decreasing demand - businesses do not need to build new data centers or sell off servers to expand or manage costs. Cloud providers also offer services that require customers to perform less maintenance and upkeep, thereby allowing them to focus on application development and delivery without worrying about operations.

The basic services provided by all cloud providers are *compute power* and *storage*. **Compute power** refers to the processing power of the machines in use. **Storage** is the volume of data that can be stored on a machine. Cloud computing allows customers to avoid the traditional requirement of buying physical hardware for these services, which can be prone to errors in estimation and may constrain growth.

##### The Shared Responsibility Model

The **shared responsibility model** is a high-level description of how cloud computing services operate relative to the traditional self-hosted approach. Under the traditional model, a company is responsible for all aspects of physical IT infrastructure, including the maintenance of physical security, physical networking, and physical host machines within a data center. With cloud computing, those responsibilities shift to the cloud provider. 

Importantly, the cloud provider is *always* responsible for maintaining physical infrastructure under any cloud computing services. Similarly, the customer is *always* responsible for the data accessed and stored via cloud services, physical devices used to connect to cloud resources, and managing accounts and identities used to access resources. Responsibility for other operations, such as patches to operating systems or network controls, vary depending on the type of service utilized.

Additional information related to the shared responsibility model is available in [Microsoft's security documentation](https://learn.microsoft.com/en-us/azure/security/fundamentals/shared-responsibility).

![Shared Responsibility Model](assets/shared-responsibility-diagram.svg)

##### Cloud Models

There are at least four models that define the deployment of cloud computing services.

The **private cloud** model refers to the deployment of computing services over the Internet that is used by a single business entity. 

The **public cloud** model refers to cloud computing services offered to the general public, meaning multiple different business entities might have data located in the same data center.

The **hybrid cloud** model refers to a business entity's use of public cloud computing services for some tasks and private cloud services for others. Such an arrangement might be used for temporary purposes or over longer periods of time related to specific configurations. Microsoft has specific Azure services oriented around hybrid cloud solutions [described in a separate learning module](https://learn.microsoft.com/en-us/training/modules/intro-to-azure-hybrid-services/).

A **multi-cloud** model refers to a business entity's use of public cloud computing services from multiple different providers, such as AWS and Azure.

Comparing the three main models:

* Private cloud offers the greatest amount of control over resources and security; data are also segregated from that belonging to other entities. The disadvantages of this approach are similar to those for the traditional data center - the entity is responsible for purchasing and managing the physical hardware involved, increasing maintenance costs and decreasing scalability.
* Public cloud offers the greatest ability to control costs while minimizing responsibility for physical hardware. The disadvantage of this approach is that it gives entities less control over resources and security than the other cloud models.
* Hybrid cloud offers the greatest flexibility by allowing companies to decide which services to use from public cloud providers and which to keep separate. The disadvantage of this approach is that it places responsibility on companies to manage the boundaries between these two different cloud environments.

:question: Microsoft specifically mentions two services in the context of these cloud types:
* Azure Arc, which enables companies to manage cloud environments (including those in hybrid and multi-cloud configurations)
* [Azure VMware Solution](https://learn.microsoft.com/en-us/training/modules/intro-azure-vmware-solution/), which facilitates the transition of VMware workloads to Azure

##### The Consumption-Based Model

Cloud computing allows companies to implement a **consumption-based model** for IT resource costs, meaning that companies have the ability to only pay for what they consume. This transforms IT spending from a model based upon *capital expenditures (CapEx)* to one based upon *operating expenditures (OpEx)*. The primary benefit of cloud computing is this ability to avoid costly investments in the development of data centers or physical infrastructure based upon estimated needs (i.e. CapEx). Instead, companies can pay for only the resources they *actually* need as they need them.

##### Cloud Pricing Models

Cloud computing uses a "pay-as-you-go" pricing model, meaning that companies only pay for services that they use. This is essentially renting compute, storage, or other capabilities from cloud service provider's data center.

#### Describe the benefits of using cloud services

**Learning Module** :point_right: [Describe the benefits of using cloud services](https://learn.microsoft.com/en-us/training/modules/describe-benefits-use-cloud-services/)

| **Task** | **Status** |
|:----|:----:|
|  Read content | :white_check_mark: |
|  Took notes | :no_entry_sign: |
|  Reviewed/revised notes | :no_entry_sign: |

* [Describe the benefits of high availability and scalability in the cloud](#cloud-in-the-cloud-high-availability-and-scalability)
* [Describe the benefits of reliability and predictability in the cloud](#cloud-in-the-cloud-reliability-and-predictability)
* [Describe the benefits of security and governance in the cloud](#cloud-in-the-cloud-security-and-governance)
* [Describe the benefits of manageability in the cloud](#cloud-in-the-cloud-manageability)

##### :cloud: In the Cloud: High Availability and Scalability

**High Availability**

**Availability** refers to the accessibility of a service (i.e. uptime). 

Because cloud computing involves renting resources from cloud service providers, it is important that customers have guarantees as to how often those rented resources will remain available in any given time period. These guarantees are enshrined in service level agreements (SLAs) that guarantee service availability at set percentages, such as 99%, 99.9%, 99.95%, and 99.99%.

There are substantial differences in these availability guarantees. For example, a service that is 99% available can have as much as 432 minutes/month of downtime, whereas a service that is 99.9% available can only have 43.2 minutes/month of downtime before violating the SLA.

**Scalability**

**Scalability** refers to the ability to adjust resources to meet demand (in either direction that it might change). 

*Vertical scaling* involves adding or removing capabilities to/from an existing resource to meet demands. For example, a single VM could scale vertically through the addition of processing power in RAM or CPU.(:computer: + RAM :arrow_up: + CPU :arrow_up:)

*Horizontal scaling* involves adding or removing identical resources as demand changes. For example, a configuration consisting of a load balancer and two VMs could scale horizontally by adding a new VM. (:computer: + :computer: + :computer::new:)

##### :cloud: In the Cloud: Reliability and Predictability

**Reliability**

**Reliability** refers to the ability of a system to recover from failures and continue to function. Reliability can be thought of as resilience against adverse events, such as power outages or natural disasters.

The cloud, as a decentralized system, presents an infrastructure for reliability. Data and compute can be shifted from one data center or region with minimal latency compared to traditional data centers or on-premises approaches. Additional features of Azure, such as availability zones and regions add to this reliability.

**Predictability**

Microsoft distinguishes between two different types of predictability: performance and cost.

**Performance predictability** means providing a predictably positive experience for customers. This includes features such as:
* Autoscaling
* Load balancing
* High availability

**Cost predictability** means forecasting the cost of expenditures on computing resources. Microsoft provides various resources to aid consumers when predicting costs, including:
* Standard Azure resource monitoring tools
* The Pricing Calculator:tm:
* The Total Cost of Ownership:tm: (TCO) tool

##### :cloud: In the Cloud: Security and Governance

**Compliance and Security**
* Azure services include offerings like set templates aligned to compliance regimes, corporate standards, and regulatory requirements
* Cloud-based auditing allows visibility into vulnerabilities that might impact cloud resources
* Cloud providers are optimized to deliver services over the Internet making them uniquely suited to prevent DDoS and similar attacks

**Governance**
* Cloud-based monitoring tools enable administrators to identify resources that are out of alignment with corporate policies
* These same tools often allow the creation and enforcement of policies throughout different levels of a resource hierarchy

##### :cloud: In the Cloud: Manageability

Microsoft distinguishes between management of the cloud and management in the cloud. 

**Management *of* the cloud** refers to the management of cloud resources, including actions like scaling and deploying resources as well as monitoring. 

**Management *in* the cloud** simply refers to the manner in which management is performed. Much of the learning modules revolve around the Azure Web portal, but management tasks can also be performed using a CLI, PowerShell, or APIs.

##### The Well-Architected Framework

This section in the learning path includes references to the [Microsoft Azure Well-Architected Framework](https://learn.microsoft.com/en-us/training/paths/azure-well-architected-framework/). There is an entire learning path dedicated to this resource and it would be a good idea to review its content prior to taking the `AZ-900` Exam.

<!-- TODO: Review Microsoft Azure Well-Architected Framework -->
#### Describe cloud service types

**Learning Module** :point_right: [Describe cloud service types](https://learn.microsoft.com/en-us/training/modules/describe-cloud-service-types/)

| **Task** | **Status** |
|:----|:----:|
|  Read content | :white_check_mark: |
|  Took notes | :no_entry_sign: |
|  Reviewed/revised notes | :no_entry_sign: |

* Describe infrastructure as a service (IaaS)
* Describe platform as a service (PaaS)
* Describe software as a service (SaaS)
* Identify appropriate use cases for each cloud service (IaaS, PaaS, and SaaS)

### Describe Azure architecture and services (35–40%)

**Learning Path** :point_right: [Microsoft Azure Fundamentals: Describe Azure architecture and services](https://learn.microsoft.com/en-us/training/paths/azure-fundamentals-describe-azure-architecture-services/)

#### Describe the core architectural components of Azure

**Learning Module** :point_right: [Describe the core architectural components of Azure](https://learn.microsoft.com/en-us/training/modules/describe-core-architectural-components-of-azure/)

| **Task** | **Status** |
|:----|:----:|
|  Read content | :white_check_mark: |
|  Took notes | :no_entry_sign: |
|  Reviewed/revised notes | :no_entry_sign: |

* Describe Azure regions, region pairs, and sovereign regions
* Describe availability zones
* Describe Azure datacenters
* Describe Azure resources and resource groups
* Describe subscriptions
* Describe management groups
* Describe the hierarchy of resource groups, subscriptions, and management groups

#### Describe Azure compute and networking services

**Learning Module** :point_right: [Describe Azure compute and networking services](https://learn.microsoft.com/en-us/training/modules/describe-azure-compute-networking-services/)

| **Task** | **Status** |
|:----|:----:|
|  Read content | :white_check_mark: |
|  Took notes | :no_entry_sign: |
|  Reviewed/revised notes| :no_entry_sign: |

* Compare compute types, including containers, virtual machines, and functions
* Describe virtual machine options, including Azure virtual machines, Azure Virtual Machine Scale Sets, availability sets, and Azure Virtual Desktop
* Describe the resources required for virtual machines
* Describe application hosting options, including web apps, containers, and virtual machines
* Describe virtual networking, including the purpose of Azure virtual networks, Azure virtual subnets, peering, Azure DNS, Azure VPN Gateway, and ExpressRoute
* Define public and private endpoints

#### Describe Azure storage services

**Learning Module** :point_right: [Describe Azure storage services](https://learn.microsoft.com/en-us/training/modules/describe-azure-storage-services/)

| **Task** | **Status** |
|:----|:----:|
|  Read content | :white_check_mark: |
|  Took notes | :no_entry_sign: |
|  Reviewed/revised notes | :no_entry_sign: |

* Compare Azure Storage services
* Describe storage tiers
* Describe redundancy options
* Describe storage account options and storage types
* Identify options for moving files, including AzCopy, Azure Storage Explorer, and Azure File Sync
* Describe migration options, including Azure Migrate and Azure Data Box

#### Describe Azure identity, access, and security

**Learning Module** :point_right: [Describe Azure identity, access, and security](https://learn.microsoft.com/en-us/training/modules/describe-azure-identity-access-security/)

| **Task** | **Status** |
|:----|:----:|
|  Read content | :white_check_mark: |
|  Took notes | :no_entry_sign: |
|  Reviewed/revised notes | :no_entry_sign: |

* Describe directory services in Azure, including Azure Active Directory (Azure AD), part of Microsoft Entra and Azure Active Directory Domain Services (Azure AD DS)
* Describe authentication methods in Azure, including single sign-on (SSO), multi-factor authentication (MFA), and passwordless
* Describe external identities in Azure, including business-to-business (B2B) and business-to-customer (B2C)
* Describe Conditional Access in Azure AD
* Describe Azure role-based access control (RBAC)
* Describe the concept of Zero Trust
* Describe the purpose of the defense-in-depth model
* Describe the purpose of Microsoft Defender for Cloud

### Describe Azure management and governance (30–35%)

**Learning Path** :point_right: [Microsoft Azure Fundamentals: Describe Azure management and governance](https://learn.microsoft.com/en-us/training/paths/describe-azure-management-governance/)

#### Describe cost management in Azure

**Learning Module** :point_right: [Describe cost management in Azure](https://learn.microsoft.com/en-us/training/modules/describe-cost-management-azure/)

| **Task** | **Status** |
|:----|:----:|
|  Read content | :white_check_mark: |
|  Took notes | :no_entry_sign: |
|  Reviewed/revised notes | :no_entry_sign: |

* Describe factors that can affect costs in Azure
* Compare the pricing calculator and the Total Cost of Ownership (TCO) Calculator
* Describe cost management capabilities in Azure
* Describe the purpose of tags

#### Describe features and tools in Azure for governance and compliance

**Learning Module** :point_right: [Describe features and tools in Azure for governance and compliance](https://learn.microsoft.com/en-us/training/modules/describe-features-tools-azure-for-governance-compliance/)

| **Task** | **Status** |
|:----|:----:|
|  Read content | :white_check_mark: |
|  Took notes | :no_entry_sign: |
|  Reviewed/revised notes | :no_entry_sign: |

* Describe the purpose of Microsoft Purview in Azure
* Describe the purpose of Azure Policy
* Describe the purpose of resource locks

#### Describe features and tools for managing and deploying Azure resources

**Learning Module** :point_right: [Describe features and tools for managing and deploying Azure resources](https://learn.microsoft.com/en-us/training/modules/describe-features-tools-manage-deploy-azure-resources/)

| **Task** | **Status** |
|:----|:----:|
|  Read content | :white_check_mark: |
|  Took notes | :no_entry_sign: |
|  Reviewed/revised notes | :no_entry_sign: |

* Describe the Azure portal
* Describe Azure Cloud Shell, including Azure Command-Line Interface (CLI) and Azure PowerShell
* Describe the purpose of Azure Arc
* Describe infrastructure as code (IaC)
* Describe Azure Resource Manager (ARM) and ARM templates

#### Describe monitoring tools in Azure

**Learning Module** :point_right: [Describe monitoring tools in Azure](https://learn.microsoft.com/en-us/training/modules/describe-monitoring-tools-azure/)

| **Task** | **Status** |
|:----|:----:|
|  Read content | :white_check_mark: |
|  Took notes | :no_entry_sign: |
|  Reviewed/revised notes | :no_entry_sign: |

* Describe the purpose of Azure Advisor
* Describe Azure Service Health
* Describe Azure Monitor, including Log Analytics, Azure Monitor alerts, and Application Insights

