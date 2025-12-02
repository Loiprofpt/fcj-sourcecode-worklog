---
title: "Worklog Tuần 11"
date: "2025-09-10"
weight: 2
chapter: false
pre: " <b> 1.11. </b> "
---

### Mục tiêu tuần 11:

* Xây dựng **cơ sở hạ tầng AWS toàn diện sử dụng Terraform** cho việc cấp phát và quản lý infrastructure-as-code.
* Thiết lập **các đường ống tự động hóa GitHub Actions** cho các quy trình tích hợp liên tục và triển khai.
* Triển khai một **cơ sở hạ tầng đường ống CI/CD hoàn chỉnh** hỗ trợ triển khai dịch vụ backend và quản lý vòng đời.
* Đảm bảo **bảo mật cơ sở hạ tầng, tuân thủ và căn chỉnh kiến trúc** với các thông số kỹ thuật thiết kế dự án.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| Thứ Hai   | - Tiến hành phân tích kiến trúc hệ thống toàn diện và xác định các tài nguyên AWS cần thiết cho triển khai cơ sở hạ tầng                                                                                   | 11/17/2025   | 11/17/2025      | <https://cloudjourney.awsstudygroup.com/> |
| Thứ Ba   | - Viết và tổ chức các module Terraform cho các dịch vụ cốt lõi: lưu trữ S3, cơ sở dữ liệu DynamoDB và chính sách bảo mật IAM                                             | 11/18/2025   | 11/18/2025      | <https://cloudjourney.awsstudygroup.com/> |
| Thứ Tư   | - Triển khai cơ sở hạ tầng nhắn tin IoT Core, các dịch vụ tính toán Lambda và các endpoint API Gateway sử dụng Terraform | 11/19/2025   | 11/19/2025      | <https://cloudjourney.awsstudygroup.com/> |
| Thứ Năm   | - Cấu hình quản lý trạng thái từ xa Terraform và triển khai các cơ chế khóa trạng thái                            | 11/20/2025   | 11/20/2025      | <https://cloudjourney.awsstudygroup.com/> |
| Thứ Sáu   | - Thiết lập các quy trình công việc CI/CD GitHub Actions cho các hoạt động Terraform tự động hóa (init, plan, apply)                                                                                     | 11/21/2025   | 11/21/2025      | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 11:

#### 1. Triển Khai Cơ Sở Hạ Tầng AWS Hoàn Chỉnh

* Thành công cấp phát cơ sở hạ tầng AWS toàn diện sử dụng Terraform, đảm bảo quản lý cơ sở hạ tầng có thể tái tạo và được kiểm soát phiên bản.

* Triển khai các thành phần cơ sở hạ tầng quan trọng:
  * **AWS IoT Core** để quản lý thiết bị IoT và nhắn tin
  * **AWS Lambda** để hoạt động tính toán không máy chủ
  * **API Gateway** để quản lý endpoint API RESTful
  * **DynamoDB** cho các dịch vụ cơ sở dữ liệu NoSQL
  * **Chính sách IAM và Vai trò** để kiểm soát truy cập toàn diện

#### 2. Quản Lý Trạng Thái Terraform

* Cấu hình **lưu trữ trạng thái từ xa Terraform** sử dụng S3, cho phép quản lý cơ sở hạ tầng dựa trên nhóm và tính nhất quán trạng thái.

* Triển khai **khóa trạng thái dựa trên DynamoDB** để ngăn chặn các sửa đổi trạng thái đồng thời và đảm bảo tính nhất quán cơ sở hạ tầng.

#### 3. Triển Khai Đường Ống CI/CD Tự Động Hóa

* Thành công thiết lập **các quy trình công việc tự động hóa GitHub Actions** bao gồm:
  * `terraform init` để khởi tạo phụ thuộc
  * `terraform plan` để dự đoán và xác thực thay đổi cơ sở hạ tầng
  * `terraform apply` để cấp phát cơ sở hạ tầng tự động

#### 4. Độ Tin Cậy và Ổn Định Đường Ống

* Đạt được **ổn định đường ống mạnh mẽ** hỗ trợ nhiều lần lặp triển khai mà không có lỗi hoạt động hoặc không nhất quán.

* Xác thực khả năng phục hồi đường ống thông qua các chu kỳ triển khai lặp lại, đảm bảo độ tin cậy sẵn sàng sản xuất.

#### 5. Căn Chỉnh Kiến Trúc

* Đảm bảo cơ sở hạ tầng được triển khai **phù hợp chính xác với các thông số kỹ thuật kiến trúc dự án**, duy trì tính nhất quán giữa tài liệu thiết kế và cơ sở hạ tầng sản xuất.


