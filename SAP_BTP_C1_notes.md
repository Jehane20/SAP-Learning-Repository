# SAP BTP Exam Notes

---

# 1. SAP BTP Strategy: Overview

## 1.1 What is SAP BTP?

**SAP Business Technology Platform (BTP)** is SAP's **Platform as a Service (PaaS)**.

### Purpose

- Extend SAP applications
- Integrate SAP and non-SAP systems
- Manage data
- Build applications
- Automate processes
- Enable AI capabilities

> **Exam Keyword:** BTP = Foundation of SAP Business Suite

---

## 1.2 Main Components of SAP BTP

| Component | Purpose |
| --- | --- |
| SAP Build | Application development and automation |
| Integration Suite | Connect SAP and third-party systems |
| HANA Cloud | Cloud database platform |
| Business Data Cloud | Unified business data |
| Business AI | AI and machine learning services |

---

## 1.3 SAP Business Suite

Business applications running on top of BTP:

| Area | Solution |
| --- | --- |
| ERP | SAP S/4HANA Cloud |
| HR | SAP SuccessFactors |
| Procurement | SAP Ariba |
| Expense Management | SAP Concur |
| Customer Experience | SAP Customer Experience |

---

## 1.4 Cloud Service Models

| Model | Meaning |
| --- | --- |
| IaaS | Infrastructure as a Service |
| PaaS | Platform as a Service |
| SaaS | Software as a Service |

> **Exam Fact:** SAP BTP is primarily a **PaaS** offering.

---

## 1.5 Cloud Deployment Models

| Model | Description |
| --- | --- |
| Public Cloud | Shared cloud environment |
| Private Cloud | Dedicated organization environment |
| Hybrid Cloud | Combination of public and private |

---

## 1.6 Clean Core

### Core

Business processes, data, integrations, and extensions in S/4HANA.

### Clean

Keep the core:

- Standard
- Up-to-date
- Cloud compliant
- Easy to upgrade

### Best Practice

Build customizations on **SAP BTP** instead of modifying S/4HANA directly.

> **Exam Keyword:** Side-by-Side Extensions

---

## 1.7 Key Benefits of BTP

- Application development
- Process automation
- System integration
- AI-powered insights
- Unified data management
- Security and identity management

---

## 1.8 SAP Integration Suite

Provides:

- API Management
- B2B Integration
- Event-driven Integration
- Prebuilt Integrations

> **Exam Fact:** SAP offers **3,400+ prebuilt integrations**.

---

## 1.9 SAP HANA Cloud

Cloud database that:

- Stores and processes data
- Supports real-time analytics
- Supports intelligent applications

---

## 1.10 SAP Business AI

### Capabilities

- Generative AI
- Document AI
- AI recommendations
- Process automation

### Purpose

- Improve productivity
- Enhance decision-making
- Increase efficiency

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

- **Pay-As-You-Go (PAYG)** → Pay only for usage.
- **Enterprise Agreement (EA)** → Prepaid contract with fixed services.
- **Free Tier** → Free access to selected services.

---

## 2.2 SAP BTP Account Structure

```text
Global Account
 └─ Directory (Optional)
      └─ Subaccount
           └─ Environment
```

### Components

- **Global Account** → Top-level SAP contract/account.
- **Directory** → Optional grouping of subaccounts.
- **Subaccount** → Independent unit for projects/resources.
- **Region** → Hosting location assigned to a subaccount.
- **Environment** → Runtime where applications are developed and deployed.

> **Exam Fact:** One subaccount belongs to **one region only**.

---

## 2.3 BTP Environments

| Environment | Purpose |
| --- | --- |
| Kyma | Kubernetes-based applications and microservices |
| ABAP | ABAP development and S/4HANA extensions |
| Neo | Legacy environment for HTML5, Java, and HANA XS |

### Remember

- **Kyma = Kubernetes**
- **ABAP Environment = ABAP Cloud Development**
- **Neo = Legacy**

---

## 2.4 SAP BTP Cockpit

### Purpose

Main graphical administration tool.

### Used For

- Managing accounts
- Managing subaccounts
- Security administration
- Service management
- Monitoring and analytics

> **Exam Fact:** BTP Cockpit is the **primary administration interface**.

---

## 2.5 SAP BTP Services

### Before Using a Service

1. Subscribe to it, **or**
2. Create an instance

### Service Types

- UI-based
- API-based

> **Exam Fact:** A service cannot be used until it is subscribed or instantiated.

---

## 2.6 Connectivity Services

### Connectivity Types

#### Internet Connectivity

- Access external systems via HTTPS.

#### Cloud-to-On-Premise Connectivity

- Access on-premise systems from SAP BTP.

---

### Core Components

| Component | Purpose |
| --- | --- |
| Connectivity Service | Connectivity proxy |
| Cloud Connector | Secure encrypted tunnel |
| Destination Service | Stores connection details |

---

### Cloud Connector

- Reverse invoke proxy
- Creates secure tunnel
- Keeps on-premise systems hidden from the public internet

---

### Destination Service

Stores:

- URL
- Credentials
- Authentication settings
- Connection parameters

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

- Build applications
- Extend SAP and non-SAP systems
- Automate business processes
- Create AI-powered agents
- Maintain a Clean Core strategy

> **Exam Keyword:** Extend, Don't Modify

---

## 3.2 Development Approaches

### Professional Development

- Complex enterprise applications
- Custom backend services
- Advanced integrations
- Full software lifecycle management

### Citizen Development

- Low-code/no-code development
- Workflow automation
- Business process improvements
- AI-assisted application creation

> **Exam Fact:** SAP supports both professional developers and citizen developers.

---

## 3.3 Key Roles

| Role | Responsibility |
| --- | --- |
| Professional Developer | Build and maintain complex applications |
| Citizen Developer | Create workflows and business solutions using visual tools |
| IT Administrator | Governance, security, operations, and lifecycle management |

### Fusion Teams

Combination of:

- Professional Developers
- Citizen Developers
- Business Experts
- IT Administrators

### Purpose

- Faster innovation
- Better business alignment
- Expanded talent pool

> **Exam Keyword:** Fusion Teams

---

## 3.4 Clean Core Strategy

### Goal

Keep SAP S/4HANA standard and upgrade-safe.

### Best Practice

Build:

- Extensions
- Applications
- Automations

on **SAP BTP** instead of modifying the ERP core.

> **Exam Keyword:** Side-by-Side Extensions

---

## 3.5 SAP Build

### What is SAP Build?

SAP's unified platform for:

- Application Development
- Process Automation
- AI Agents
- Digital Workspaces

Built on:

- SAP BTP
- SAP Business Suite
- SAP S/4HANA

### Components of SAP Build

| Component | Purpose |
| --- | --- |
| SAP Build Code | Professional application development |
| SAP Build Process Automation | Workflow automation and RPA |
| Joule Studio | AI agent development |
| SAP Build Work Zone | Digital workplace experience |
| Joule | AI copilot |

### SAP Build Benefits

- AI-powered development
- Low-code and pro-code development
- Clean Core compliance
- Faster application delivery
- Reduced IT workload

---

## 3.6 Joule

### What is Joule?

SAP's AI Copilot.

### Capabilities

- Code generation
- Logic explanation
- Data model creation
- AI-assisted development
- Business process automation

### Joule Agents

Custom AI agents that can:

- Reason
- Plan
- Execute tasks
- Trigger workflows
- Interact with SAP and non-SAP systems

### Difference

| Type | Purpose |
| --- | --- |
| Joule Skill | Single task |
| Joule Agent | Multi-step reasoning and execution |

> **Exam Fact:** Joule Agents perform business actions, not just conversations.

---

## 3.7 Enterprise Automation

### Three-Step Automation Journey

#### 1. Discover

Use:

- SAP Signavio

Purpose:

- Identify inefficiencies

#### 2. Connect

Use:

- SAP Integration Suite

Purpose:

- Connect SAP and non-SAP systems

#### 3. Automate

Use:

- SAP Build

Purpose:

- AI-powered workflows and automation

### Hyperautomation

Combines:

- AI
- Workflow automation
- RPA
- Event-driven processes

Goal:

- End-to-end process automation

> **Exam Keyword:** Hyperautomation

---

## 3.8 Development Frameworks

### Frontend Frameworks

| Framework | Purpose |
| --- | --- |
| SAPUI5 | Enterprise web applications |
| OpenUI5 | Open-source version of SAPUI5 |

#### SAPUI5 Features

- MVC architecture
- Model-driven development
- Enterprise tooling

---

### Backend Frameworks

| Framework | Purpose |
| --- | --- |
| CAP | Cloud-native services and APIs |
| RAP | ABAP-based OData services |

#### CAP (Cloud Application Programming Model)

Features:

- Node.js
- Java
- CDS
- OData
- Fiori integration

Use For:

- Cloud-native development

> **Exam Keyword:** CAP = Node.js / Java

#### RAP (RESTful Application Programming Model)

Features:

- ABAP-based
- HANA optimized
- CDS
- OData services
- Fiori generation

Use For:

- ABAP Cloud Development

> **Exam Keyword:** RAP = ABAP

---

## 3.9 Development Environments

| Environment | Purpose |
| --- | --- |
| SAP Business Application Studio (BAS) | Cloud-native development |
| Eclipse + ABAP Development Tools | ABAP development |

### BAS Supports

- SAPUI5
- CAP
- Fiori
- SAP Build Code

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

| Solution | Purpose |
| --- | --- |
| SAP BTP SDK for Android | Native Android development |
| Fiori Guidelines for Android | Android design standards |

---

## Most Likely Exam Questions

### Q: What is SAP Build?

**A:** SAP's unified platform for application development, process automation, AI agents, and digital workspaces.

### Q: What is Joule?

**A:** SAP's AI copilot for development, automation, and AI-powered business processes.

### Q: What is the difference between Joule Skills and Joule Agents?

**A:**

- Skill = Single task
- Agent = Multi-step reasoning and execution

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

# 4. SAP BTP Integration

## 4.1 Application Programming Interfaces (APIs)

An introductory guide to APIs explaining their definition, importance, and implementation in enterprise systems.

### Key Details

- APIs are application programming interfaces that act as mediators between applications and users, enabling communication between different software systems.
- APIs separate communication from the underlying task, allowing users to focus on functionality rather than implementation details.
- REST APIs are the most commonly used type, implementing CRUD operations (Create, Read, Update, Delete).
- APIs enable faster system integration, reduce human effort, and save costs in IT architecture.

### Real-World Examples

- Google Search: When searching "SAP," Google's backend calls its API to retrieve and display results.
- WhatsApp messaging: Messages are sent through API calls to recipients.
- Voice assistants: Convert spoken queries into text and call APIs for processing.

### API Types

| API Type | Key Characteristics |
| --- | --- |
| REST API | Most common, uses HTTP methods; implements CRUD operations |
| Other Types | Various global standards exist for defining and implementing APIs |

### REST API Operations

| Method | Purpose |
| --- | --- |
| GET | Retrieve data (Read) |
| POST | Create new data (Create) |
| PUT | Update entire resource (Update) |
| DELETE | Remove data (Delete) |
| PATCH | Update partial resource (Update) |

### Business Value

- Enables integration between SAP and non-SAP systems.
- Facilitates cloud/hybrid environment integration.
- Allows commercialization and management of APIs through SAP Integration Suite.
- Reduces development time and costs for system integration.

### Why It Matters

APIs are omnipresent in modern technology, enabling seamless communication between devices and applications while allowing developers to focus on business logic rather than infrastructure details.

---

## 4.2 SAP Business Accelerator Hub

A developer platform offering sandbox APIs for testing SAP products without requiring direct access to production systems.

### Key Details

| Feature | Description |
| --- | --- |
| Primary Function | Provides sandbox APIs for testing SAP applications including S/4HANA, SAP BTP, SuccessFactors, and Concur |
| Testing Capability | Allows developers to create extensions, applications, and integrations using testing data provided through sandbox APIs |
| Authentication | Requires only an API key for authentication; automatically generated when logging in with SAP ID account |
| Access Method | Direct access available at https://api.sap.com/ |
| API Discovery | Offers API reference documentation, schemas, and direct testing capabilities for different SAP products |

### Key Takeaways

- SAP Business Accelerator Hub is a web application specifically designed for developers and integrators.
- Enables discovery, testing, and consumption of APIs across multiple SAP products.
- Sandbox APIs allow testing without production environment access.
- API keys are generated within the platform and used for authentication.
- Direct API testing and reference documentation are available.

---

## 4.3 SAP Integration Suite: Enterprise Integration Platform

SAP Integration Suite is a managed multi-cloud service in SAP BTP that enables seamless integration of on-premise and cloud applications across hybrid, large, and heterogeneous enterprise environments.

### Key Features

| Feature | Description |
| --- | --- |
| Core Capabilities | Four core capabilities provided as a service on SAP BTP |
| Integration Flexibility | Seamless integration of on-premise and cloud applications |
| AI-Powered | Utilizes artificial intelligence to simplify integration development |
| Open Connectors | Pre-built connectors for SAP and non-SAP applications |
| Multi-Environment | Same integration artifacts can run across multiple environments |
| Out-of-the-Box Solutions | Pre-packaged integration scenarios for common use cases |

### Why It Matters

- Creates a completely connected IT landscape for intelligent, sustainable enterprises.
- Simplifies integration of diverse applications and business processes.
- Provides flexibility through SAP-managed service with pre-built content.
- Enables integration of both SAP and non-SAP systems using open connectors.
- Leverages AI to streamline the development of integration scenarios.

### Use Cases

- Integrating business processes across hybrid environments.
- Connecting legacy systems with modern cloud applications.
- Integrating non-SAP applications using open connectors.
- Building customized integration solutions based on specific enterprise needs.

### Additional Resources

- Solution brief available for detailed positioning.
- Help page for technical information.
- Learning journeys including "Developing with SAP Integration Suite".
- Open connector documentation for non-SAP integrations.

---

## 4.4 SAP Integration Suite

SAP Integration Suite is an iPaaS (Integration Platform as a Service) solution that enables seamless integration of on-premise and cloud applications within SAP Business Technology Platform (BTP).

### Key Capabilities

| Feature | Description |
| --- | --- |
| Core Capabilities | Four core capabilities provided as a SAP-managed multi-cloud service |
| Hybrid Integration | Designed for simplified enterprise integration of hybrid, large, and heterogeneous environments |
| AI-Driven Integration | Utilizes artificial intelligence to simplify development of integration scenarios |
| Out-of-the-Box Solutions | Pre-built integration scenarios ready for immediate use |
| Open Connectors | Open connector capabilities to integrate non-SAP applications |

### Key Benefits

- Enables a completely connected IT landscape for intelligent, sustainable enterprises.
- Supports integration across on-premise and cloud environments.
- Simplifies development with AI-powered capabilities.
- Provides flexibility to run the same integration artifacts across multiple environments.
- Offers both pre-packaged solutions and customizable integration options.

### Use Cases

- Integration of SAP and non-SAP applications.
- Business process integration across hybrid environments.
- Enterprise-wide integration to create a unified IT landscape.
- Seamless connection of applications and processes for enhanced enterprise operations.

### Additional Resources

- Solution brief available for detailed information.
- Learning journeys available for developers.
- Help page for additional information.
- Open connector documentation available.

### Summary

SAP Integration Suite is SAP's comprehensive solution for enterprise integration scenarios, combining pre-built tools with flexible, AI-enhanced capabilities to streamline application integration across hybrid environments.

# 5. SAP BTP AI and Data Foundation

## 5.1 SAP Business AI: Enterprise Artificial Intelligence Platform

SAP Business AI is an integrated artificial intelligence platform that embeds AI capabilities directly into SAP business processes to drive enterprise transformation through automation, enhanced decision-making, and scalable innovation.

### Key Components of SAP Business AI

| Component | Description | Key Features |
| --- | --- | --- |
| Joule | Generative AI copilot | 1,800+ skills, works across 80% of most-used transactions, conversational interface, handles tasks from time off requests to outbound deliveries |
| Joule Agents | Collaborative AI agents | Specialized AI agents that leverage SAP business data, operate autonomously or collaboratively across departments, break down organizational silos |
| Embedded AI | Native integration | AI capabilities built into SAP applications, delivered as standard product experience without additional setup |
| AI Foundation | Platform backbone | Tools and technologies for building, extending, and running custom AI solutions and agents at scale |

### Core AI Products in SAP BTP

| Product | Purpose | Key Details |
| --- | --- | --- |
| SAP AI Launchpad | AI use case management | Multitenant SaaS application for managing AI use cases across multiple AI runtime instances |
| SAP AI Core | AI execution service | Service designed to handle execution and operations of AI assets |
| SAP HANA Cloud | Machine learning capabilities | Embeds machine learning libraries optimized for in-memory processing |

### Business Value Demonstrations

#### HR Transformation

SAP Business AI integrated across the "Hire to Retire" process in SAP SuccessFactors:

- Identifies internal talent and plans for future workforce needs
- Creates accurate skill architectures
- Enables faster identification of skill gaps

#### Process Automation

- Automates complex business tasks through intelligent agent orchestration

#### Decision Enhancement

- Provides real-time insights and cross-enterprise optimization

### Why It Matters

SAP Business AI represents SAP's comprehensive approach to enterprise AI, transforming fragmented systems into a unified intelligent platform that delivers measurable business value across all business functions through AI-powered automation, enhanced decision-making, and scalable innovation.

---

## 5.2 SAP HANA Cloud: AI & Data Foundation

SAP HANA Cloud is a fully managed in-memory multi-tier cloud database as a service that serves as the central data platform for SAP Business Technology Platform, enabling AI-driven applications with real-time analytics and semantic context.

### Key Details

| Feature | Description |
| --- | --- |
| Data Platform | Central database connecting enterprise business data with AI use cases, intelligent applications, and autonomous agents |
| Architecture | Fully managed in-memory multi-tier DBaaS with real-time analytics, hybrid transactional capabilities, and multi-model support |
| Core Capabilities | In-memory processing, multi-model (transactional, analytical, spatial, graph, text), predictive analytics, and native vector processing |
| AI Integration | Supports Model Context Protocol (MCP) for direct AI agent integration, agentic memory for persistent conversation context, and specialized database agents |
| Data Management | Unified access layer that consolidates and harmonizes data from multiple sources without requiring all data to be loaded into a single storage solution |
| Multi-Model Engine | Combines vector, graph, hierarchy, and spatial data processing in one system for advanced analytics and generative AI scenarios |

### Key Value Propositions

- Real-time processing with in-memory architecture
- Multi-model capabilities – handles transactional, analytical, spatial, graph, and text data simultaneously
- Cost efficiency with cloud qualities including low TCO, elasticity, and serverless principles
- Simplified architecture – reduces complexity by eliminating multiple databases and complex data pipelines
- Enterprise governance with built-in security standards for AI operations
- Scalability – handles constantly growing data volumes in a central location

### AI-Powered Capabilities

| AI Feature | Implementation |
| --- | --- |
| Vector Processing | Native support for semantic embedding creation |
| Graph Processing | Networked data modeling (supply chains, communities) |
| Hierarchical Analysis | Ancestry, dependency, and distance queries |
| Predictive Analytics | Built-in ML algorithms for forecasting |
| Agentic Memory | Persistent long-term context for multi-turn conversations |
| Model Context Protocol (MCP) | Direct database access for Joule agents and custom AI models |

### Use Cases

- Enterprise AI applications requiring semantic context
- Real-time decision-making with live data
- Hybrid cloud/on-premise application environments
- Generative AI workflows with direct database embedding
- Intelligent agents for data discovery and analysis
- Complex data relationships analysis across enterprise systems

### Why It Matters

SAP HANA Cloud transforms SAP Business Technology Platform into an AI-native foundation by providing a single, trusted data layer that enables real-time analytics, semantic understanding, and autonomous application development while maintaining enterprise governance and security standards.

---

## 5.3 SAP AI Foundation: Document Processing and Generative AI Services

This documentation explains SAP's AI Foundation architecture, focusing on Document AI capabilities and the Generative AI Hub for enterprise AI integration.

### Key Services

| Service | Purpose | Key Features |
| --- | --- | --- |
| SAP Document AI | Automates business document processing | OCR extraction, document classification, field identification using AI models, human-in-the-loop validation, integration with SAP applications |
| Generative AI Hub | Unified access to generative AI models | Multiple LLM providers, prompt design/test/validation tools, model orchestration, consistent interface across runtimes |
| SAP AI Core | AI runtime infrastructure | GPU-accelerated processing, cost-efficient scaling, automated model deployments, unified API for AI workloads |

### Document AI Processing Workflow

1. Documents (PDFs, scanned images, emails) are received via APIs or SAP interfaces.
2. OCR technology extracts text content from documents.
3. Document type classification identifies business context.
4. Predefined AI models identify and extract specific fields.
5. Human validation allows for error correction and quality improvement.
6. Extracted data can be matched with existing SAP business objects.

### Architecture Components

| Component | Function |
| --- | --- |
| Generative AI Hub | Central interface for LLMs and generative AI orchestration |
| SAP AI Core | Runtime engine for AI workloads with GPU support and autoscaling |
| SAP AI Launchpad | Central management platform for AI lifecycle (model deployments, monitoring, optimization) |
| Unified AI API | Shared API interface that allows applications to consume AI services across different runtimes |

### Business Value

- Automates manual document processing workflows (invoice validation, delivery note matching, order processing)
- Reduces manual data entry while maintaining integration with standard SAP business processes
- Enables enterprises to leverage AI without deep technical expertise in model development
- Provides scalable, managed AI solutions with built-in monitoring and optimization capabilities

# 6. SAP BTP Security Fundamentals

## 6.1 User and Authorization Management on SAP BTP

This guide explains how SAP Business Technology Platform (BTP) manages users and authorizations across its hierarchical architecture.

### Key Details

| Component | Description |
| --- | --- |
| Global Account | Highest level representing the SAP contract; contains entitlements, billing, and directory/subaccount structure |
| Directories | Used to organize subaccounts within a global account when there are too many subaccounts |
| Subaccounts | Individual accounts with 3 possible environments (Cloud Foundry, Kyma, or ABAP) for different development approaches |
| Platform Users | Administrators and operators who manage resources; assigned at specific architecture levels with administrator permissions |
| Business Users | Consumers of applications and services who can use apps without needing BTP cockpit access, created by subaccount administrators |

### Authorization Structure

| Authorization Level | User Type | Permissions |
| --- | --- | --- |
| Global Account | Platform Administrator | Full entitlement management, directory/subaccount creation |
| Subaccount | Subaccount Administrator | Local entitlements, service subscriptions, user management within subaccount |
| Subaccount | Business User | Application access only (no administrative privileges) |

### Role Management

| Element | Details |
| --- | --- |
| Role Collections | Groups of roles that combine authorizations; assigned to users instead of individual roles |
| Predefined Collections | SAP provides standard collections for platform and application users |
| Custom Collections | Administrators can create custom collections for specific applications |
| Federation | Most efficient approach; assign role collections to user groups in custom identity providers |

### Key Takeaways

- SAP BTP provides built-in functionalities for role collections and user assignment at all architecture levels.
- Platform users must be managed at global accounts, directories, subaccounts, and spaces.
- Business users consume applications and services but cannot perform administrative tasks.
- Role collections streamline user onboarding by applying permissions to entire user groups automatically.

---

## 6.2 SAP Cloud Identity Services

SAP Cloud Identity Services provides identity management solutions for SAP Business Technology Platform, enabling centralized authentication and user lifecycle management.

### Key Details

| Feature | Description |
| --- | --- |
| Authentication Architecture | Applications in SAP BTP do not store user information; authentication requires redirect to an Identity Provider (IdP) |
| Default Identity Provider | SAP ID Service (account.sap.com); pre-configured, shared by all customers with automatic trust connections to SAP BTP subaccounts |
| SAP ID Service Capabilities | Managed by SAP, allows only free user creation; manages S-Users, P-Users, and D-Users; used for official SAP sites |
| Recommended Solution | SAP Cloud Identity Services – Identity Authentication Service (IAS) as a central hub for integration |
| Identity Authentication Service | Validates authentication between IdPs and applications using standards like SAML; enables Single Sign-On (SSO) across systems |
| Identity Provisioning Service | Manages identity lifecycle (create, change, delete users and groups) for cloud and on-premise applications |

### Why It Matters

- Decouples authentication from application functionality.
- Centralizes identity management across SAP BTP and enterprise systems.
- Enables secure, standardized authentication methods (SAML, SSO).
- Provides integration capabilities with corporate identity providers.
- Supports hybrid cloud environments with both SAP and third-party applications.

---

## 6.3 SAP Authorization and Trust Management Service (XSUAA)

XSUAA is SAP's internal cloud service that handles user authentication and authorization between applications and identity providers within SAP BTP.

### Key Details

| Feature | Description |
| --- | --- |
| Core Function | Authenticates users and grants access through business roles between applications and identity providers |
| Authentication Protocol | Uses OAuth to authenticate services without sharing passwords (uses JWT tokens) |
| Data Handling | Does not store user data or user records |
| Integration | Built on Cloud Foundry's UAA (User Authorization and Authentication) with SAP-specific enhancements |
| Identity Providers | Can connect to SAP ID Service or other integrated corporate identity providers |

### Key Components

#### XSUAA Service

- Acts as central infrastructure for business user authentication and authorization in SAP BTP.
- Uses OAuth to create authorization tokens between services and identity providers.
- JWT (JSON Web Token) tokens are used to securely transmit user information and access rights.
- Requires a trusted connection to an identity provider.

#### App Router

- Node.js-based application serving as a single entry point for business applications.
- Configured via `xs-app.json` file to define routes and bind to XSUAA service instances.
- Routes authentication requests to the XSUAA service.
- Routes between different microservices.
- Serves static resources (documents/images) from the file system.

### Why It Matters

XSUAA provides a secure, centralized authorization solution for SAP BTP that enables businesses to manage user access through roles without storing sensitive user data, ensuring secure authentication across applications while maintaining the flexibility of microservices architecture.