---
{"dg-publish":true,"permalink":"/blog-articles/aveva-pi-system/pi-to-connect-agent-behavior-in-usage-reporting-mode/","dgPassFrontmatter":true}
---

## **1. Overview**

The **PI to CONNECT Agent** serves as a secure and reliable communication bridge between on‑premises PI Systems and **AVEVA Connect**. Its primary function is to facilitate data exchange and system registration with AVEVA’s cloud environment in accordance with corporate security and licensing policies.

When configured in **Usage‑Reporting‑Only** mode, the Agent restricts outbound data transmission solely to essential licensing and usage metrics required by AVEVA Flex licensing. This operational mode is designed to protect sensitive operational data by minimizing exposure while maintaining full compliance with licensing terms. It ensures that no real‑time process or asset information is ever transmitted beyond the customer network.

---

## **2. Deployment and Connectivity**

- **Connection Initiation:**  
    All communication sessions are initiated **outbound** from the PI to CONNECT Agent to AVEVA Connect. This architecture eliminates the need to open inbound ports on the corporate firewall, simplifying network security configurations.
    
- **Middleware and Proxy Support:**  
    The Agent fully supports corporate proxy configurations and integrates seamlessly with **AVEVA’s DMZ Secure Link** technology, providing an additional layer of isolation for customers operating within segmented or restricted network environments.
    
- **DMZ Deployment Option:**  
    For enhanced security, the Agent can be deployed on a dedicated host located in a demilitarized zone (DMZ). When operating in Usage‑Reporting‑Only mode, the Agent transmits only a minimal set of license usage fields—no PI time‑series data or Asset Framework (AF) metadata leave the customer network.
    
- **PI Server Internet Exposure:**  
    The **PI Server** itself maintains a complete air‑gap from the internet. All communication is managed through the Agent, ensuring that the PI System remains isolated and internally contained.
    

---

## **3. Data Scope and Payload**

- **Outbound Data in Usage‑Reporting‑Only Mode:**  
    The following fields represent the complete set of outbound data transmitted in this mode:
    
    - PI Server name
        
    - Licensed tag count (total number of PI points under license)
        
    - Basic usage metrics necessary for **AVEVA Flex** licensing validation
        
- **Exclusion of Operational Data:**  
    No time‑series records, tag names, timestamps, values, or AF attributes are included in the transmitted payload. Operational data remains entirely within the on‑premises environment.
    
- **Inbound Data:**  
    Inbound communication is strictly limited to lightweight configuration control messages targeting the Agent itself—such as start, stop, or retry operations. No inbound commands can modify or influence the configuration or operation of the PI Server.
    

---

## **4. Security**

- **Encryption:**  
    All communications between the Agent and AVEVA Connect utilize **TLS 1.2 or higher**, ensuring transport‑level encryption of all transmitted data. At present, the Agent does not implement payload‑level encryption or encryption‑at‑rest for locally stored information.
    
- **Authentication:**
    
    - **Agent to PI System:** Authentication is performed via **Windows Integrated Security**, supporting Kerberos and service account configurations.
        
    - **Agent to AVEVA Connect:** Authentication relies on **secure, token‑based client credentials** issued at the time of initial registration with AVEVA Connect. These credentials are managed through controlled provisioning workflows to ensure traceability and secure access.
        

---

## **5. Connection Behavior**

- **Data Transmission Frequency:**  
    Usage data is transmitted automatically once per day in a small, resource‑efficient payload.
    
- **Effect of Disconnection:**  
    A temporary loss of connectivity between the Agent and AVEVA Connect has **no effect** on the operation of the PI Server or any associated PI System components. However, if disconnection persists for an extended period, it may lead to potential non‑compliance with AVEVA Flex licensing terms. AVEVA monitors license reporting activity daily and may identify prolonged inactivity for follow‑up.
    

---

## **6. API Access and Control**

- The PI to CONNECT Agent **does not expose** a public API interface for external programmatic control or data retrieval.
    
- Certain **cloud‑side management APIs** exist to perform administrative actions, such as initiating or halting the Agent service remotely. These APIs are restricted to authorized AVEVA services, and related documentation is available upon request.
    
- License usage reporting involves retrieving the PI point count from the connected **PI Data Archive**:
    
    - For installations using the **aggregate PI point licensing model**, the Agent transmits the **actual active PI point count** from the Data Archive.
        
    - For systems licensed under a **traditional point count limit**, the Agent reports the **maximum licensed PI point total** as the official usage value.
        

---

## **7. Compliance and Governance**

- Customers maintain full administrative control over the activation and configuration of **Usage‑Reporting‑Only mode**, including the ability to enable, disable, or reconfigure reporting options as needed.
    
- The destination configuration for outbound usage data is also under customer control, ensuring transparency and flexibility in governance and compliance management.
    

---

## **Summary**

The **Usage‑Reporting‑Only** mode within the PI to CONNECT Agent provides a controlled, secure, and compliant method for reporting license usage data to AVEVA Connect. It is specifically designed to:

- Limit data transfer to essential licensing information
    
- Ensure all communication is **outbound‑only** from the customer environment
    
- Prevent any operational or real‑time PI System data from leaving the premise
    
- Maintain compliance with **AVEVA Flex licensing** and corporate data protection standards
    