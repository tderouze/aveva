---
{"dg-publish":true,"tags":["OperationalData","TechInsider"],"permalink":"/blog-articles/data/building-a-robust-industrial-data-platform-7-essential-capabilities/","dgPassFrontmatter":true}
---

In today's data-driven industrial landscape, a modern [[Blog Articles/AVEVA PI System/Unlocking the Power of Real-Time Data Operation Platforms\|Industrial Data Platform]] (IDP) is no longer a luxury, but a necessity. It's the foundation for unlocking insights, optimizing operations, and driving innovation. But what capabilities are _essential_ when building a state-of-the-art IDP? This post outlines seven core capabilities, serving as a guide to help you navigate the complexities of building or selecting the right platform for your needs.

Think of this as a starting point for your Request for Information (RFI) or Request for Proposal (RFP) process. This is version one, and we are eager to hear your thoughts. Feel free to leave comments and help us improve this guide. We plan to release a second version in the coming months.

## Important Considerations Up Front

Before we dive in, keep these points in mind:
- **Prioritization is Key:** We deliberately _don't_ rank these capabilities. Your specific needs and priorities will determine which are most important to your organization.
- **Vendor Agnostic (For Now):** We aren't mapping these capabilities to specific vendors yet. The goal is to focus on the "what" before the "who."
- **Beyond the Unified Namespace (UNS):** The UNS is a critical piece, but this is about the bigger picture of a comprehensive data platform.

## Why "Industrial Data Platform?"

We've intentionally chosen the term "[[Blog Articles/AVEVA PI System/Unlocking the Power of Real-Time Data Operation Platforms\|Industrial Data Platform]]" to move beyond outdated terms like "Historian" or overly broad terms like "IoT Platform". This is about a holistic approach to operational data.

If you are new to the topic, check out these previous blog posts for essential background information:
- **Part 1** (The IT and OT view on Data)
- **Part 2** (Introducing the Operational Data Platform)
- **Part 3** (The need for Better Data)
- **Part 4** (Breaking the OT Data Barrier: It's the Platform)
- **Part 5** (The Unified Namespace)

## Open Source Friendly

You can freely use, share and adapt it as long as you attribute us and you distribute your work again under the same license (CC BY-SA 4.0).

## The 7 Core Capabilities

![](https://i.imgur.com/zI8C0TL.png)


## 1. Connectivity: Bridging the Data Source Gap

The first step is connecting to your diverse data sources. This means more than just the latest sensors; it's about integrating legacy systems, modern devices, and everything in between.

- **Data Source Identification:**
    - Local Time Series Data: Historians, SCADA, PLCs
    - Cloud Data: IIoT devices, cloud platforms
    - MOM Data: MES, Quality Systems, Planning Systems
    - Engineering & GIS Data: Digital twins, GIS systems
- **Protocol Support:**
    - OPC (DA, HDA, UA)
    - MQTT (with/without Sparkplug B)
    - Machine/Sensor Protocols (Profibus, Modbus, I/O Link)
    - Database Connections
    - REST APIs
    - Text File Parsing (CSV, JSON)
- **Essential Requirements:**
    - Real-time streaming / event-driven architecture
    - Buffering / backfilling
    - Redundancy

## 2. Contextualization & Data Management: Making Sense of the Numbers

Raw data is useless without context. This capability focuses on enriching data with relevant information, turning it into actionable insights.

- **Data Management Requirements**
    - Modeling, management, viewing, versioning capabilities to build your ontology, based on standards, vendor provided templates, your own templates or ‘Build-your-own’ schema;
    - Ways to manually input or automatically ingest and process metadata which leads to the model;
    - Do you need a very simple straightforward model, or do you need a complex - object oriented style - of modeling?
    - Identify ways to query the model, e.g. using GraphQL

- **Production / Maintenance Context:**
    - Linking to external data sources
    - Caching/storing relevant events within the platform
    - ETL functionality for data mapping

## 3. Data Quality: Ensuring Reliability

Garbage in, garbage out. Data quality is paramount, especially in industrial environments where decisions impact safety and efficiency.

- **Key Considerations:**
    - Data types and sources
    - Monitoring requirements (out-of-bounds, NaN, spikes, gaps, drift, calibration issues, etc.)
    - Custom monitoring needs
    - Exposure of observations (context layer, BI reports, etc.)
    - Data cleaning and augmentation tools (UI, API)
    - Automated data cleaning pipelines
    - Data quality KPIs

## 4. Data Broker & Store: The Foundation for Scalability

This is where data lands and becomes readily available. The right data store is critical for handling the volume, velocity, and variety of industrial data.

- **Data Store Capabilities:**
    - Time-Series Data Handling
    - Event and Alarm Storage
    - Publish-Subscribe (MQTT Broker) / Traditional Polling
    - Data Lifecycle Management (Hot-Warm-Cold)
    - Multi-Layered Storage (Bronze/Silver/Gold)
- **Querying and Retrieval:**
    - Subscription and Query Capabilities
    - API Accessibility (REST, GraphQL)
    - Contextual Data Retrieval

## 5. Analytics: Turning Data into Decisions

This capability enables real-time and batch analytics directly within the platform.

- **Essential Features:**
    - Real-time and batch analytics
    - Advanced calculations / virtual tags
    - Edge computing capabilities
- **Optional Features:**
    - Edge preprocessing for machine learning and statistical analysis

## 6. Visualization: Empowering Users

Making data accessible and understandable to everyone, from operators to management.

- Visualization
- Dashboarding
- Sharing and collaboration possibilities of these visuals and dashboards

## 7. Data Sharing: Opening the Platform

Providing secure and controlled access to data for external users and applications.

- APIs, SDKs
- Data Querying Capabilities (raw, cleaned, prepared, contextualized)

## Important Remark: Embrace Interoperability

Don't feel pressured to find an all-in-one solution from a single vendor. Look for best-of-breed solutions that interoperate well. Open protocols, good documentation, and standardized implementations are crucial for avoiding vendor lock-in.

## Additional Capabilities: Management & Orchestration

A often overlooked aspect, is the need for a overarching management model.

- Deployment model
    - Edge/On-Prem first
    - Edge/On-Prem first + Cloud capable = Hybrid
    - Cloud first + Edge/On-Prem Capable = Hybrid
    - Cloud first
- Supporting capabilities
    - Cyber Security
    - User Management
    - Life Cycle Management (Monitor, Deploy, Update)

## Comparing Apples to Apples: A Pricing Checklist

When evaluating solutions, consider these factors:

- Ongoing license costs (users, data points, servers, storage, data consumption)
- Support models for open-source components
- Internal/external resources required for operation
- Infrastructure costs
- Cybersecurity requirements
- Cloud costs (storage, compute, data ingress/egress)

## Where Does the Unified Namespace Fit In?

The UNS is a key concept for organizing and contextualizing data within the data broker. Connectivity, contextualization, and the central data broker are the core components linked to a UNS. The Unified Namespace - in the context of a data platform - can only be valuable, when it is part of a larger concept, but it doesn’t replace it.

## Final Thoughts

Building a modern Industrial Data Platform is a journey. By focusing on these seven core capabilities, you'll be well-equipped to create a platform that unlocks the full potential of your operational data.

That’s it for now! Make sure to subscribe to receive future releases and don’t forget to review our other content :)