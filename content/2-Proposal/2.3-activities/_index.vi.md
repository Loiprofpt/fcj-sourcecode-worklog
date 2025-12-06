---
title: "Hoạt động & Sản phẩm bàn giao"
date: "2025-09-09"
weight: 3
chapter: false
pre: " <b> 2.3 </b> "
---

# 3. Hoạt động & Sản phẩm bàn giao

## 3.1 Ma trận Hoạt động & Sản phẩm bàn giao

Dự án được triển khai trong **12 tuần** (tháng 9 – tháng 11/2025), với **Tuần 1–7** tập trung vào kiến thức AWS và chuẩn bị nền tảng, và **Tuần 8–12** dành cho phát triển thực tế theo mô hình Agile.

| Giai đoạn dự án | Timeline | Hoạt động chính | Sản phẩm / Mốc hoàn thành | Nỗ lực (ước tính) |
| :--- | :--- | :--- | :--- | :--- |
| **I. Kiến thức nền tảng AWS & Lập kế hoạch** | Tuần 1–7 | • Học các dịch vụ cốt lõi của AWS<br>• Hoàn thiện kiến trúc & mô hình DB<br>• Tạo AWS Account & IAM Roles<br>• Khởi tạo Terraform State (S3) | • Kiến thức AWS Certification<br>• Tài liệu kiến trúc (LLD)<br>• Thiết lập Terraform Backend<br>• Thiết kế Database Schema | 40 man-days |
| **II. Tích hợp phần cứng & IoT** | Tuần 8 | • Nối ESP32 với AS608, MQ-3, MAX30102<br>• Implement logic xác thực MQTT<br>• Cấu hình AWS IoT Core Pipeline<br>• Hiệu chỉnh cảm biến | • ESP32 được flash hoàn tất<br>• Kết nối với IoT Core thành công<br>• Log dữ liệu cảm biến | 8 man-days |
| **III. Hệ thống xác thực & Backend** | Tuần 9 | • Phát triển Lambda Functions (Python)<br>• Cấu hình API Gateway & Rules Engine<br>• Xây dựng hệ thống xác thực lai (Hybrid Auth) | • Bộ serverless backend hoàn chỉnh<br>• REST API hoạt động<br>• Xác thực vân tay | 8 man-days |
| **IV. Phát triển Frontend** | Tuần 10 | • Xây dựng Web Portal (HTML/CSS/JS)<br>• Tích hợp API<br>• Triển khai AWS Amplify Hosting | • URL website công khai<br>• Dashboard giao diện<br>• Chức năng tra cứu công dân | 8 man-days |
| **V. IaC & CI/CD** | Tuần 11 | • Viết Terraform triển khai hạ tầng<br>• Tạo pipeline GitHub Actions<br>• Cấu hình AWS WAF<br>• Tăng cường bảo mật hệ thống | • Pipeline CI/CD tự động hóa<br>• WAF bảo vệ website<br>• CloudWatch Monitoring | 8 man-days |
| **VI. Kiểm thử & Tài liệu** | Tuần 12 | • Kiểm thử toàn hệ thống End-to-End<br>• Demo cuối cho stakeholder<br>• Viết tài liệu và bàn giao | • Báo cáo cuối cùng<br>• Source code đầy đủ<br>• Tài liệu hướng dẫn sử dụng | 8 man-days |

---

## 3.2 Phạm vi Không bao gồm (Out of Scope)

Những hạng mục sau **không nằm trong phạm vi** của PoC này nhằm đảm bảo tiến độ 12 tuần:

- **Ứng dụng Mobile:** Không phát triển ứng dụng iOS/Android; web responsive sẽ hỗ trợ mobile.
- **Thiết kế phần cứng công nghiệp:** Chỉ sử dụng breadboard hoặc vỏ in 3D cơ bản, không thiết kế vỏ chuẩn IP67.
- **Hiệu lực pháp lý:** Dữ liệu nồng độ cồn chỉ phục vụ demo kỹ thuật, không dùng cho mục đích pháp lý.
- **Tích hợp hệ thống cũ:** Không kết nối với SQL on-premise hoặc database của lực lượng công an.

---

## 3.3 Lộ trình đưa vào Sản xuất (Path to Production)

Giải pháp hiện tại là **PoC kỹ thuật**. Để triển khai cấp độ Production, cần thực hiện:

1. **Tính sẵn sàng cao (High Availability):**
   - Kích hoạt **DynamoDB Global Tables**.
   - Triển khai API Gateway đa AZ.

2. **Khả năng hoạt động ngoại tuyến:**
   - Sử dụng **AWS IoT Greengrass** để buffer dữ liệu khi mất mạng.

3. **Tăng cường bảo mật:**
   - Di chuyển secrets vào **AWS Secrets Manager**.
   - Thực hiện kiểm thử xâm nhập (PenTest) bởi bên thứ 3.

4. **Vận hành – Giám sát:**
   - Cấu hình **CloudWatch Anomaly Detection**.
   - Thiết lập **Incident Response Plan** chuẩn.

