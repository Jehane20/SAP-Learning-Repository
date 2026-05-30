# SAP BTP Exam Notes

---

# 1. SAP BTP Strategy: Overview

## 1.1 What is SAP BTP?

**SAP Business Technology Platform (BTP)** is SAP's **Platform as a Service (PaaS)**.

### Purpose

* Extend SAP applications
* Integrate SAP and non-SAP systems
* Manage data
* Build applications
* Automate processes
* Enable AI capabilities

> **Exam Keyword:** BTP = Foundation of SAP Business Suite

---

## 1.2 Main Components of SAP BTP

| Component           | Purpose                                |
| ------------------- | -------------------------------------- |
| SAP Build           | Application development and automation |
| Integration Suite   | Connect SAP and third-party systems    |
| HANA Cloud          | Cloud database platform                |
| Business Data Cloud | Unified business data                  |
| Business AI         | AI and machine learning services       |

---

## 1.3 SAP Business Suite

Business applications running on top of BTP:

| Area                | Solution                |
| ------------------- | ----------------------- |
| ERP                 | SAP S/4HANA Cloud       |
| HR                  | SAP SuccessFactors      |
| Procurement         | SAP Ariba               |
| Expense Management  | SAP Concur              |
| Customer Experience | SAP Customer Experience |

---

## 1.4 Cloud Service Models

| Model | Meaning                     |
| ----- | --------------------------- |
| IaaS  | Infrastructure as a Service |
| PaaS  | Platform as a Service       |
| SaaS  | Software as a Service       |

> **Exam Fact:** SAP BTP is primarily a **PaaS** offering.

---

## 1.5 Cloud Deployment Models

| Model         | Description                        |
| ------------- | ---------------------------------- |
| Public Cloud  | Shared cloud environment           |
| Private Cloud | Dedicated organization environment |
| Hybrid Cloud  | Combination of public and private  |

---

## 1.6 Clean Core

### Core

Business processes, data, integrations, and extensions in S/4HANA.

### Clean

Keep the core:

* Standard
* Up-to-date
* Cloud compliant
* Easy to upgrade

### Best Practice

Build customizations on **SAP BTP** instead of modifying S/4HANA directly.

> **Exam Keyword:** Side-by-Side Extensions

---

## 1.7 Key Benefits of BTP

* Application development
* Process automation
* System integration
* AI-powered insights
* Unified data management
* Security and identity management

---

## 1.8 SAP Integration Suite

Provides:

* API Management
* B2B Integration
* Event-driven Integration
* Prebuilt Integrations

> **Exam Fact:** SAP offers **3,400+ prebuilt integrations**.

---

## 1.9 SAP HANA Cloud

Cloud database that:

* Stores and processes data
* Supports real-time analytics
* Supports intelligent applications

---

## 1.10 SAP Business AI

### Capabilities

* Generative AI
* Document AI
* AI recommendations
* Process automation

### Purpose

* Improve productivity
* Enhance decision-making
* Increase efficiency

---

## Most Likely Exam Questions

### Q: What is SAP BTP?

**A:** SAP's Platform-as-a-Service that enables application development, integration, data management, automation, and AI services.

### Q: What is Clean Core?

**A:** Keeping S/4HANA standard and placing custom extensions on BTP.

### Q: What are the main BTP capabilities?

**A:** Development, Integration, Data & Analytics, AI & Automation.

### Q: What is the role of SAP Integration Suite?

**A:** Connects SAP and non-SAP systems through APIs and prebuilt integrations.

### Q: What is SAP HANA Cloud?

**A:** SAP's cloud-native database platform for data management and analytics.

### Q: What service model is SAP BTP?

**A:** Platform as a Service (PaaS).

---

# 2. SAP BTP Architecture and Services

## 2.1 SAP BTP Commercial Models

* **Pay-As-You-Go (PAYG)** → Pay only for usage.
* **Enterprise Agreement (EA)** → Prepaid contract with fixed services.
* **Free Tier** → Free access to selected services.

---

## 2.2 SAP BTP Account Structure

```text
Global Account
 └─ Directory (Optional)
      └─ Subaccount
           └─ Environment
```

### Components

* **Global Account** → Top-level SAP contract/account.
* **Directory** → Optional grouping of subaccounts.
* **Subaccount** → Independent unit for projects/resources.
* **Region** → Hosting location assigned to a subaccount.
* **Environment** → Runtime where applications are developed and deployed.

> **Exam Fact:** One subaccount belongs to **one region only**.

---

## 2.3 BTP Environments

| Environment | Purpose                                         |
| ----------- | ----------------------------------------------- |
| Kyma        | Kubernetes-based applications and microservices |
| ABAP        | ABAP development and S/4HANA extensions         |
| Neo         | Legacy environment for HTML5, Java, and HANA XS |

### Remember

* **Kyma = Kubernetes**
* **ABAP Environment = ABAP Cloud Development**
* **Neo = Legacy**

---

## 2.4 SAP BTP Cockpit

### Purpose

Main graphical administration tool.

### Used For

* Managing accounts
* Managing subaccounts
* Security administration
* Service management
* Monitoring and analytics

> **Exam Fact:** BTP Cockpit is the **primary administration interface**.

---

## 2.5 SAP BTP Services

### Before Using a Service

1. Subscribe to it, **or**
2. Create an instance

### Service Types

* UI-based
* API-based

> **Exam Fact:** A service cannot be used until it is subscribed or instantiated.

---

## 2.6 Connectivity Services

### Connectivity Types

#### Internet Connectivity

* Access external systems via HTTPS.

#### Cloud-to-On-Premise Connectivity

* Access on-premise systems from SAP BTP.

---

### Core Components

| Component            | Purpose                   |
| -------------------- | ------------------------- |
| Connectivity Service | Connectivity proxy        |
| Cloud Connector      | Secure encrypted tunnel   |
| Destination Service  | Stores connection details |

---

### Cloud Connector

* Reverse invoke proxy
* Creates secure tunnel
* Keeps on-premise systems hidden from the public internet

---

### Destination Service

Stores:

* URL
* Credentials
* Authentication settings
* Connection parameters

> **Exam Fact:** For connecting SAP BTP to on-premise systems, the answer is usually: **Cloud Connector + Destination Service**

---

## 10 Facts to Memorize

1. PAYG = Pay per use.
2. EA = Prepaid contract.
3. Free Tier = Free limited services.
4. Global Account is the highest level.
5. Directories are optional.
6. Subaccounts are independent units.
7. One subaccount = one region.
8. Kyma = Kubernetes environment.
9. BTP Cockpit = Main administration UI.
10. Cloud Connector + Destination Service enable on-premise connectivity.

---

# 3. SAP BTP Agent and Application Development

## 3.1 Core Concept

SAP BTP enables organizations to:

* Build applications
* Extend SAP and non-SAP systems
* Automate business processes
* Create AI-powered agents
* Maintain a Clean Core strategy

> **Exam Keyword:** Extend, Don't Modify

---

## 3.2 Development Approaches

### Professional Development

* Complex enterprise applications
* Custom backend services
* Advanced integrations
* Full software lifecycle management

### Citizen Development

* Low-code/no-code development
* Workflow automation
* Business process improvements
* AI-assisted application creation

> **Exam Fact:** SAP supports both professional developers and citizen developers.

---

## 3.3 Key Roles

| Role                   | Responsibility                                             |
| ---------------------- | ---------------------------------------------------------- |
| Professional Developer | Build and maintain complex applications                    |
| Citizen Developer      | Create workflows and business solutions using visual tools |
| IT Administrator       | Governance, security, operations, and lifecycle management |

### Fusion Teams

Combination of:

* Professional Developers
* Citizen Developers
* Business Experts
* IT Administrators

### Purpose

* Faster innovation
* Better business alignment
* Expanded talent pool

> **Exam Keyword:** Fusion Teams

---

## 3.4 Clean Core Strategy

### Goal

Keep SAP S/4HANA standard and upgrade-safe.

### Best Practice

Build:

* Extensions
* Applications
* Automations

on **SAP BTP** instead of modifying the ERP core.

> **Exam Keyword:** Side-by-Side Extensions

---

## 3.5 SAP Build

### What is SAP Build?

SAP's unified platform for:

* Application Development
* Process Automation
* AI Agents
* Digital Workspaces

Built on:

* SAP BTP
* SAP Business Suite
* SAP S/4HANA

### Components of SAP Build

| Component                    | Purpose                              |
| ---------------------------- | ------------------------------------ |
| SAP Build Code               | Professional application development |
| SAP Build Process Automation | Workflow automation and RPA          |
| Joule Studio                 | AI agent development                 |
| SAP Build Work Zone          | Digital workplace experience         |
| Joule                        | AI copilot                           |

### SAP Build Benefits

* AI-powered development
* Low-code and pro-code development
* Clean Core compliance
* Faster application delivery
* Reduced IT workload

---

## 3.6 Joule

### What is Joule?

SAP's AI Copilot.

### Capabilities

* Code generation
* Logic explanation
* Data model creation
* AI-assisted development
* Business process automation

### Joule Agents

Custom AI agents that can:

* Reason
* Plan
* Execute tasks
* Trigger workflows
* Interact with SAP and non-SAP systems

### Difference

| Type        | Purpose                            |
| ----------- | ---------------------------------- |
| Joule Skill | Single task                        |
| Joule Agent | Multi-step reasoning and execution |

> **Exam Fact:** Joule Agents perform business actions, not just conversations.

---

## 3.7 Enterprise Automation

### Three-Step Automation Journey

#### 1. Discover

Use:

* SAP Signavio

Purpose:

* Identify inefficiencies

#### 2. Connect

Use:

* SAP Integration Suite

Purpose:

* Connect SAP and non-SAP systems

#### 3. Automate

Use:

* SAP Build

Purpose:

* AI-powered workflows and automation

### Hyperautomation

Combines:

* AI
* Workflow automation
* RPA
* Event-driven processes

Goal:

* End-to-end process automation

> **Exam Keyword:** Hyperautomation

---

## 3.8 Development Frameworks

### Frontend Frameworks

| Framework | Purpose                       |
| --------- | ----------------------------- |
| SAPUI5    | Enterprise web applications   |
| OpenUI5   | Open-source version of SAPUI5 |

#### SAPUI5 Features

* MVC architecture
* Model-driven development
* Enterprise tooling

---

### Backend Frameworks

| Framework | Purpose                        |
| --------- | ------------------------------ |
| CAP       | Cloud-native services and APIs |
| RAP       | ABAP-based OData services      |

#### CAP (Cloud Application Programming Model)

Features:

* Node.js
* Java
* CDS
* OData
* Fiori integration

Use For:

* Cloud-native development

> **Exam Keyword:** CAP = Node.js / Java

#### RAP (RESTful Application Programming Model)

Features:

* ABAP-based
* HANA optimized
* CDS
* OData services
* Fiori generation

Use For:

* ABAP Cloud Development

> **Exam Keyword:** RAP = ABAP

---

## 3.9 Development Environments

| Environment                           | Purpose                  |
| ------------------------------------- | ------------------------ |
| SAP Business Application Studio (BAS) | Cloud-native development |
| Eclipse + ABAP Development Tools      | ABAP development         |

### BAS Supports

* SAPUI5
* CAP
* Fiori
* SAP Build Code

> **Exam Fact:** BAS is SAP's primary cloud IDE.

---

## 3.10 Development Stack

```text
Frontend
 └─ SAPUI5 / React / Angular / Vue

Backend
 └─ CAP / RAP

Platform
 └─ SAP BTP (Cloud Foundry / Kyma)

Database
 └─ SAP HANA Cloud + CDS
```

---

## 3.11 Mobile Development

| Solution                     | Purpose                    |
| ---------------------------- | -------------------------- |
| SAP BTP SDK for Android      | Native Android development |
| Fiori Guidelines for Android | Android design standards   |

---

## Most Likely Exam Questions

### Q: What is SAP Build?

**A:** SAP's unified platform for application development, process automation, AI agents, and digital workspaces.

### Q: What is Joule?

**A:** SAP's AI copilot for development, automation, and AI-powered business processes.

### Q: What is the difference between Joule Skills and Joule Agents?

**A:**

* Skill = Single task
* Agent = Multi-step reasoning and execution

### Q: What are Fusion Teams?

**A:** Teams composed of professional developers, citizen developers, business experts, and IT administrators.

### Q: What is CAP?

**A:** SAP Cloud Application Programming Model for Node.js and Java cloud-native development.

### Q: What is RAP?

**A:** ABAP RESTful Application Programming Model for ABAP-based OData services.

### Q: What is SAPUI5?

**A:** SAP's framework for enterprise web application development.

### Q: What is BAS?

**A:** SAP Business Application Studio, SAP's cloud-native development environment.

---

## High-Yield Facts to Memorize

1. SAP Build = Development + Automation + AI + Workspaces.
2. Joule = SAP AI Copilot.
3. Joule Agents can execute business processes.
4. Fusion Teams combine business and technical roles.
5. Clean Core = Extend on BTP, don't modify S/4HANA.
6. SAPUI5 = Frontend framework.
7. CAP = Node.js / Java backend framework.
8. RAP = ABAP backend framework.
9. BAS = SAP's cloud IDE.
10. Hyperautomation = AI + RPA + Workflow Automation.
11. SAP Signavio = Discover processes.
12. SAP Integration Suite = Connect systems.
13. SAP Build = Automate processes.
14. Kyma = Kubernetes runtime.
15. SAP BTP is the foundation for all development and extension activities.
