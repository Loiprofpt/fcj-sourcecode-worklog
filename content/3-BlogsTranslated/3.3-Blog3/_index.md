---
title: "BLog 3"
date: "2025-09-09"
weight: 1
chapter: false
pre: " <b> 3.3. </b> "
---

# How Minnesota Athletics built a unified data layer to boost fan engagement with AWS

Each ticket sold for a University of Minnesota athletic event changes hands an average of three times. With over a million people passing through the gates annually, the volume of transactional data is massive.

Minnesota Athletics faced challenges with fragmented data and time-consuming manual processes. In less than a year, they replaced that complexity with a scalable **data lake** built on AWS.

---

## The University's "Front Porch"

Minnesota Athletics supports over 600 student-athletes and serves as the "front porch" connecting the public to the university. However, the legacy ecosystem consisted of loosely connected third-party tools, where data was shared only one-way, insufficient for deep insights into fan behavior.

---

## Solution: A Unified Data Lake on AWS

Aiming to own their data for real-time analytics, the team built a centralized data layer without overhauling the entire existing system.

#### Why AWS?
* **Cost-Effective:** Pay-as-you-go pricing allowed them to start small and scale.
* **Control:** The team maintained full control over their data.
* **Rapid Deployment:** Leveraged the university's existing agreement with AWS for quick provisioning.

---

## System Architecture: Secure and Flexible

A small internal team of three completed this foundation in less than eight months. The architecture uses serverless services to ensure automation and security:

1.  **Ingest:** Ticketing data is transferred securely via SFTP into a private **Amazon S3** environment.
2.  **Security:** Access is tightly managed using **AWS Secrets Manager**.
3.  **Processing:** **AWS Lambda** and **AWS Glue** automatically clean, deduplicate, and normalize data as files arrive.
4.  **Redundancy:** Automated checks and S3 versioning help prevent data loss.

---

## Business Impact

Centralizing data delivered immediate results:

* **Revenue Optimization:** A ticket price prediction model forecasted a **3–5% revenue increase** and helped minimize losses even during down years.
* **Golden Record:** creating a unified customer profile by linking data from tickets, retail, and donations to understand individual fan value.

---

## Lessons Learned

Travis Cameron shares advice for other institutions:
* **Start Small:** Focus on a clear, narrow goal (e.g., ticketing data only) for phase one.
* **Leverage Resources:** Use existing organizational AWS agreements.
* **Small Teams Succeed:** A team of three can modernize data infrastructure with a clear vision.