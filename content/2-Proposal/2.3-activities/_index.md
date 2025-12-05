---
title: "Activities & Deliverables"
date: "2025-09-09"
weight: 3
chapter: false
pre: " <b> 2.3 </b> "
---

# 3. Activities & Deliverables

## 3.1 Activities and Deliverables Matrix

The project is executed over a **12-week timeline**, following Agile methodology with 2-week sprints.

| Project Phase | Timeline | Key Activities | Deliverables / Milestones | Est. Effort |
| :--- | :--- | :--- | :--- | :--- |
| **I. Design & Foundation** | Week 1-2 | • Finalize Architecture & DB Schema<br>• Setup AWS Account & IAM Roles<br>• Initialize Terraform State (S3) | • Architecture Document (LLD)<br>• Terraform Backend Setup<br>• Database Schema Design | 10 man-days |
| **II. Firmware Development** | Week 3-4 | • Wire ESP32 with AS608, MQ-3, MAX30102<br>• Implement MQTT Auth Logic<br>• Calibrate Sensors | • Flashed ESP32 Device<br>• "Hello World" to IoT Core<br>• Sensor Reading Logs | 15 man-days |
| **III. Backend Services** | Week 5-7 | • Develop Lambda Functions (Node.js)<br>• Configure API Gateway & Rules Engine<br>• Setup CodePipeline for Backend | • Deployed Serverless Stack<br>• Working REST APIs<br>• Automated Backend Pipeline | 20 man-days |
| **IV. Frontend Development** | Week 8-9 | • Build Web Portal (React/Vue)<br>• Integrate APIs & Cognito (if any)<br>• Setup AWS Amplify Hosting | • Public Website URL<br>• Admin Dashboard UI<br>• Citizen Lookup Feature | 15 man-days |
| **V. Security & Testing** | Week 10-11 | • Implement AWS WAF Rules<br>• End-to-End System Testing<br>• Security Scanning (tfsec) | • Security Audit Report<br>• UAT Sign-off<br>• WAF ACL Configured | 10 man-days |
| **VI. Handover & Closure** | Week 12 | • Final Demo to Stakeholders<br>• Documentation & Knowledge Transfer<br>• Cleanup Sandbox Resources | • Final Project Report<br>• Source Code Repository<br>• User Manual | 5 man-days |

---

## 3.2 Out of Scope

The following items are explicitly **excluded** from this Proof of Concept (PoC) to ensure focused delivery within the 12-week timeframe:

* **Mobile Application:** No native iOS or Android apps will be developed; the mobile-responsive Web Portal will serve mobile users.
* **Industrial Hardware Design:** The prototype will use breadboards or a basic 3D-printed case, not an IP67-rated industrial enclosure.
* **Legal Admissibility:** The alcohol sensor readings are for technical demonstration only and are not certified for legal enforcement in court.
* **Legacy Integration:** No integration with existing on-premise government SQL servers or legacy police databases.

---

## 3.3 Path to Production

The current system represents a **Technical Proof of Concept (PoC)**. To transition this solution to a Production-ready environment for real-world deployment, the following steps are required:

1.  **High Availability:**
    * Enable **DynamoDB Global Tables** for multi-region redundancy.
    * Deploy API Gateway across multiple Availability Zones (AZs).
2.  **Offline Resilience:**
    * Implement **AWS IoT Greengrass** on a local gateway to buffer violation data when network connectivity is lost.
3.  **Security Hardening:**
    * Migrate hardcoded configuration secrets to **AWS Secrets Manager**.
    * Conduct rigorous 3rd-party Penetration Testing.
4.  **Operational Excellence:**
    * Set up advanced **CloudWatch Anomaly Detection** alerts.
    * Establish a formal **Incident Response Plan**.