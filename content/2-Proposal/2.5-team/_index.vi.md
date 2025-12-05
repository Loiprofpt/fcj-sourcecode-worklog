---
title: "Cơ Cấu Nhóm"
date: "2025-09-09"
weight: 5
chapter: false
pre: " <b> 2.5 </b> "
---

# 5. Cơ Cấu Nhóm

## 5.1 Các Bên Liên Quan & Nhà Tài Trợ Dự Án

| Vai trò | Tên | Mô tả |
| :--- | :--- | :--- |
| **Partner Executive Sponsor** | **[Tên Giảng Viên]** | Giảng viên hướng dẫn tại **Đại học FPT TP.HCM**. Chịu trách nhiệm chấm điểm và định hướng học thuật. |
| **Project Stakeholder** | **[Khách Hàng / Phòng CSGT]** | Đại diện người dùng cuối (ví dụ: Phòng Cảnh Sát Giao Thông) chịu trách nhiệm xác nhận tính ứng dụng thực tế của hệ thống. |

---

## 5.2 Nhóm Dự Án (SPICA)

**Nhóm SPICA** gồm 4 thành viên chủ chốt từ Đại học FPT, chuyên về IoT, Điện toán đám mây và Kỹ thuật phần mềm.

| Tên | Vai trò | Trách nhiệm chính |
| :--- | :--- | :--- |
| **Phạm Viết Lợi** | **Kỹ sư IoT & Firmware** | • **Kiến trúc phần cứng:** Chọn linh kiện (ESP32, AS608, MQ-3) và thiết kế mạch.<br>• **Lập trình nhúng:** Viết firmware C++/PlatformIO để đọc cảm biến và xử lý logic thiết bị.<br>• **Bảo mật thiết bị:** Triển khai quy trình xác thực vân tay trên thiết bị. |
| **Đặng Đình Bắc** | **Kiến trúc sư Cloud (Backend)** | • **Serverless Computing:** Thiết kế & triển khai các hàm AWS Lambda.<br>• **Thiết kế cơ sở dữ liệu:** Mô hình DynamoDB và tối ưu hóa hiệu năng.<br>• **IaC:** Quản lý hạ tầng bằng **Terraform** và **CodePipeline**. |
| **Trần Quốc Dinh** | **Kỹ sư IoT Cloud & Fullstack** | • **Kết nối IoT:** Cấu hình AWS IoT Core, MQTT Topics và Rules Engine.<br>• **Tích hợp hệ thống:** Kết nối giữa thiết bị và giao diện Web.<br>• **Hỗ trợ Frontend:** Tích hợp API và xử lý logic giao diện. |
| **Dương Hải Nam** | **Lập trình viên Frontend** | • **Thiết kế UI/UX:** Xây dựng cổng tra cứu công khai và dashboard quản trị.<br>• **Web Development:** Phát triển SPA bằng **React/Vue.js**.<br>• **Triển khai:** Cấu hình **AWS Amplify** và CI/CD cho frontend. |

---

## 5.3 Kế Hoạch Giao Tiếp

Để đảm bảo làm việc hiệu quả, nhóm SPICA áp dụng quy trình giao tiếp như sau:

* **Daily Stand-up:** 15 phút mỗi sáng để cập nhật tiến độ và trở ngại.
* **Weekly Sprint Review:** Họp vào mỗi thứ Sáu để demo các tính năng hoàn thành cho Giảng viên.
* **Công cụ sử dụng:**
    * **Quản lý mã nguồn:** GitHub (Monorepo).
    * **Quản lý công việc:** Trello / Jira / GitHub Projects.
    * **Giao tiếp:** Slack / Discord / Microsoft Teams.
