---
title: "Event 2"
date: "2025-09-09"
weight: 2
chapter: false
pre: " <b> 4.2. </b> "
---

# Summary Report: “AWS Cloud Mastery Series #3 – Security Pillar”

### General Introduction

**AWS Cloud Mastery Series #3 – Security Pillar** là một **workshop buổi sáng** được tổ chức vào **ngày 29 tháng 11 năm 2025** tại **Văn phòng AWS Việt Nam, Tòa Bitexco Financial, TP. Hồ Chí Minh**.  
Sự kiện tập trung vào **trụ cột bảo mật trong AWS Well-Architected Framework**, cung cấp kiến thức chuyên sâu về **bảo mật, quản lý danh tính, phát hiện mối đe dọa, bảo vệ hạ tầng, bảo vệ dữ liệu và phản ứng sự cố**.  
Workshop dành cho **developer, kiến trúc sư giải pháp và chuyên gia cloud** mong muốn nâng cao kỹ năng trong việc thiết kế **các workload AWS an toàn và bền vững**.

---

### Event Objectives

- Hiểu rõ **nguyên tắc của trụ cột bảo mật trong AWS Well-Architected Framework**.  
- Học các **best practice** về quản lý danh tính, giám sát và bảo vệ hạ tầng.  
- Khám phá **mã hóa dữ liệu, quản lý secrets và tự động hóa phản ứng sự cố**.  
- Nhận biết các **thực tiễn sai lầm phổ biến** và tình huống thực tế tại Việt Nam.  
- Xây dựng lộ trình học tập nâng cao: **Security Specialty và Solutions Architect Professional**.

---

### Event Schedule & Key Sessions

#### 8:30 – 8:50 | Opening & Security Foundation
- Vai trò của **Security Pillar** trong Well-Architected Framework.  
- Nguyên tắc cốt lõi: *Least Privilege*, *Zero Trust*, *Defense in Depth*.  
- Giải thích **Shared Responsibility Model**.  
- Tổng quan **mối đe dọa phổ biến trong môi trường cloud tại Việt Nam**.

#### 8:50 – 9:30 | Pillar 1 – Identity & Access Management (IAM)
- Kiến trúc IAM hiện đại: Users, Roles, Policies, tránh long-term credentials.  
- IAM Identity Center: SSO và permission sets.  
- Service Control Policies (SCPs) và permission boundaries cho multi-account.  
- MFA, xoay vòng credentials và Access Analyzer.  
- Mini demo: kiểm tra và mô phỏng quyền truy cập IAM.

#### 9:30 – 9:55 | Pillar 2 – Detection & Continuous Monitoring
- Giám sát liên tục với **CloudTrail, GuardDuty và Security Hub**.  
- Logging ở mọi tầng: VPC Flow Logs, ALB logs, S3 logs.  
- Cảnh báo và tự động hóa với **EventBridge**.  
- Detection-as-Code: tự động hóa cơ sở hạ tầng và quy tắc.

#### 9:55 – 10:10 | Coffee Break

#### 10:10 – 10:40 | Pillar 3 – Infrastructure Protection
- Bảo mật mạng & workload: phân đoạn VPC, bố trí private/public.  
- So sánh và ứng dụng **Security Groups vs NACLs**.  
- Sử dụng **WAF, Shield, Network Firewall**.  
- Bảo vệ workload cơ bản cho **EC2, ECS, EKS**.

#### 10:40 – 11:10 | Pillar 4 – Data Protection
- Quản lý key với **KMS**: policies, grants, xoay vòng.  
- Mã hóa dữ liệu tại-rest & in-transit: S3, EBS, RDS, DynamoDB.  
- **Secrets Manager & Parameter Store** – patterns xoay vòng.  
- Phân loại dữ liệu và thiết lập guardrails truy cập.

#### 11:10 – 11:40 | Pillar 5 – Incident Response (IR)
- Chu trình IR theo AWS.  
- Playbook ví dụ:
  - IAM key bị xâm phạm  
  - S3 public exposure  
  - EC2 nhiễm malware  
- Snapshot, cách ly và thu thập bằng chứng.  
- Tự động phản ứng bằng **Lambda** và **Step Functions**.

#### 11:40 – 12:00 | Wrap-Up & Q&A
- Tổng kết 5 trụ cột bảo mật.  
- Thảo luận các **thực tiễn sai lầm và tình huống thực tế tại Việt Nam**.  
- Hướng dẫn lộ trình học tập nâng cao: **Security Specialty, SA Pro**.

---

### Key Learnings

- Hiểu toàn diện về **nguyên tắc bảo mật AWS**.  
- Nắm các phương pháp thực tiễn về **quản lý danh tính, giám sát và bảo vệ hạ tầng**.  
- Hiểu cách **bảo vệ dữ liệu và tự động phản ứng sự cố**.  
- Nhận thức được các **thực tiễn sai lầm phổ biến và cách khắc phục**.  
- Xây dựng lộ trình học tập tiếp theo với **chứng chỉ bảo mật AWS**.

---

### Application in Work

- Áp dụng **best practice IAM** trong các dự án multi-account.  
- Thiết lập **logging và monitoring tiêu chuẩn** cho workloads hiện tại.  
- Lập kế hoạch **tự động phản ứng sự cố** bằng Lambda & Step Functions.  
- Tích hợp **Well-Architected Security principles** khi đánh giá kiến trúc hạ tầng.

---

### Experience at the Event

- Tham gia **workshop tập trung và thực hành**, cung cấp kiến thức chuyên sâu về bảo mật cloud.  
- Học hỏi trực tiếp từ **chuyên gia AWS và thực chiến trong ngành**.  
- Nhận các **chiến lược thực tế** để bảo vệ hạ tầng và workloads.  
- Nâng cao tự tin trong việc áp dụng **best practice bảo mật** vào dự án thực tế.

---

### Event Photos

![AWS Cloud Mastery Series #3 HCMC 1](/images/4-EventPaticipated/event2new.jpg)

---

> **Conclusion:**  
> Workshop cung cấp kiến thức chuyên sâu về **trụ cột bảo mật AWS**, nâng cao kỹ năng thực hành và hướng dẫn cách áp dụng **Well-Architected security principles** vào môi trường sản xuất. Nó nhấn mạnh tầm quan trọng của **hạ tầng cloud an toàn, tuân thủ và bền vững**.
