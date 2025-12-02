---
title: "Worklog Tuần 8"
date: "2025-09-10"
weight: 1
chapter: false
pre: " <b> 1.8. </b> "
---
{{% notice warning %}}
⚠️ **Lưu ý:** Các thông tin dưới đây chỉ nhằm mục đích tham khảo, vui lòng **không sao chép nguyên văn** cho bài báo cáo của bạn kể cả warning này.
{{% /notice %}}


### Mục tiêu tuần 8:

* Hoàn thiện **đề xuất dự án nhóm toàn diện** với độ rõ ràng chiến lược và độ sâu kỹ thuật.
* Tiến hành ôn tập có hệ thống và tổng hợp **các khái niệm kiến trúc AWS cơ bản** chuẩn bị cho kỳ thi giữa kỳ.
* Giải quyết và củng cố các lĩnh vực không chắc chắn về mặt kỹ thuật để đảm bảo nắm vững toàn bộ kiến thức.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                     | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------- | --------------- | ----------------------------------------- |
| Thứ Hai   | - Hoàn thiện đề xuất dự án nhóm <br> - Ôn tập các nguyên tắc thiết kế kiến trúc bảo mật AWS: <br>&emsp; + Quản lý Danh tính & Truy cập (IAM), Xác thực Đa yếu tố (MFA), Chính sách Kiểm soát Dịch vụ (SCP) <br>&emsp; + Các cơ chế Mã hóa (KMS, TLS/ACM), Nhóm Bảo mật, Danh sách Kiểm soát Truy cập Mạng (NACLs) <br>&emsp; + Các quy tắc Phát hiện (GuardDuty, Shield, WAF), Quản lý Bí mật | 27/10/2025  | 27/10/2025       | <https://cloudjourney.awsstudygroup.com/> |
| Thứ Ba   | - Ôn tập các mô hình thiết kế kiến trúc phục hồi và khả dụng cao: <br>&emsp; + Chiến lược Vùng Khả dụng Đa (AZ), Các mô hình triển khai Đa khu vực <br>&emsp; + Chiến lược Phục hồi Thảm họa (DR) và kế hoạch phục hồi <br>&emsp; + Các cơ chế Tự động Chia tỷ lệ, Quản lý DNS (Route 53), Phân phối Tải <br>&emsp; + Các thủ tục Bảo vệ và Khôi phục Dữ liệu | 28/10/2025  | 28/10/2025       | <https://cloudjourney.awsstudygroup.com/> |
| Thứ Tư   | - Ôn tập các nguyên tắc Tối ưu hóa Hiệu suất Hệ thống cao: <br>&emsp; + Chia tỷ lệ Tính toán (EC2 Auto Scaling, AWS Lambda, AWS Fargate) <br>&emsp; + Tối ưu hóa Lưu trữ (S3, Hệ thống Tệp Đàn hồi, Kho Khối Đàn hồi) <br>&emsp; + Phân phối Nội dung và Gia tốc (CloudFront, Bộ Gia tốc Toàn cầu, Chiến lược Lưu trữ đệm) | 29/10/2025  | 29/10/2025       | <https://cloudjourney.awsstudygroup.com/> |
| Thứ Năm   | - Ôn tập các phương pháp và công cụ Tối ưu hóa Chi phí: <br>&emsp; + Phân tích Chi phí và Dự báo (Cost Explorer, Quản lý Ngân sách) <br>&emsp; + Chiến lược Mua hàng (Savings Plans, Instances được Dành riêng) <br>&emsp; + Tối ưu hóa Vòng đời Tài nguyên và Chiến lược Phân tầng Dữ liệu | 30/10/2025  | 30/10/2025       | <https://cloudjourney.awsstudygroup.com/> |
| Thứ Sáu   | - Tham gia kỳ thi đánh giá giữa kỳ FCJ. | 31/10/2025  | 31/10/2025       | <https://cloudjourney.awsstudygroup.com/> |

### Kết quả đạt được tuần 8:

#### 1. Hoàn Thiện Đề Xuất Dự Án Nhóm

* Hoàn thiện thành công đề xuất nhóm với nội dung được diễn đạt rõ ràng, cấu trúc mạch lạc và sự phù hợp toàn diện với các thông số kỹ thuật và yêu cầu dự án.

#### 2. Thành Thạo Thiết Kế Kiến Trúc Bảo Mật AWS

* Ôn tập và củng cố toàn diện kiến thức các khuôn khổ thiết kế bảo mật AWS bao gồm các nguyên tắc cơ bản về Quản lý Danh tính và Truy cập (IAM), các giao thức Xác thực Đa yếu tố, triển khai Chính sách Kiểm soát Dịch vụ và các công nghệ Mã hóa (KMS, TLS/ACM).

* Nắm vững các kiểm soát bảo mật mạng bao gồm Nhóm Bảo mật, Danh sách Kiểm soát Truy cập Mạng, các khả năng Phát hiện (GuardDuty, Shield, WAF) và cơ sở hạ tầng Quản lý Bí mật.

#### 3. Hiểu Biết Kiến Trúc Phục Hồi và Khả Dụng Cao

* Phát triển sự hiểu biết vững chắc về các nguyên tắc phục hồi hệ thống phân tán nhấn mạnh chiến lược triển khai Vùng Khả dụng Đa, các mô hình kiến trúc Đa khu vực và các phương pháp Phục hồi Thảm họa toàn diện.

* Thành thạo trong triển khai các cơ chế Tự động Chia tỷ lệ, Quản lý DNS Route 53, các kiến trúc Phân phối Tải và chiến lược Sao lưu/Khôi phục Dữ liệu để nâng cao tính khả dụng hệ thống và tính liên tục hoạt động.

#### 4. Tối Ưu Hóa Thiết Kế Hệ Thống Hiệu Suất Cao

* Tăng cường chuyên môn trong tối ưu hóa hiệu suất tận dụng các giải pháp Chia tỷ lệ Tính toán (EC2 Auto Scaling, Lambda, Fargate), các chiến lược Tối ưu hóa Lưu trữ (S3, EFS, EBS) và các công nghệ Gia tốc Phân phối Nội dung (CloudFront, Global Accelerator).

#### 5. Hiểu Biết Khuôn Khổ Tối Ưu Hóa Chi Phí

* Tăng cường hiểu biết về các chiến lược tối ưu hóa chi phí AWS bao gồm phân tích Chi tiêu (Cost Explorer, Budgets), tối ưu hóa Mua hàng (Savings Plans, Reserved Instances) và Quản lý Vòng đời Tài nguyên với Phân tầng Dữ liệu thông minh.

#### 6. Thành Tích Kỳ Thi Giữa Kỳ

* Hoàn thành thành công kỳ thi giữa kỳ FCJ, thể hiện việc ứng dụng và tổng hợp hiệu quả tất cả kiến thức kiến trúc và hoạt động đã tích lũy.


