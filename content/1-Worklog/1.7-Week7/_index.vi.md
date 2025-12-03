---
title: "Worklog Tuần 7"
date: "2025-09-10"
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu tuần 7:

* Nắm vững các kiến thức toàn diện về **AWS Lambda** và vai trò của nó trong các kiến trúc điện toán không máy chủ (serverless).
* Phát triển kỹ năng **cài đặt, cấu hình AWS CLI** và triển khai các hàm Java lên Lambda.
* Hiểu rõ các mô hình tích hợp giữa **API Gateway** và **AWS Lambda** để xây dựng các API backend có khả năng mở rộng.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| Thứ Hai | - Tổng quan về AWS Lambda: các khái niệm cốt lõi, nguyên tắc kiến trúc, lợi ích của mô hình serverless và luồng thực thi hàm | 20/10/2025 | 20/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| Thứ Ba | - Khám phá AWS CLI: chức năng, quy trình cài đặt, cấu hình IAM User để truy cập AWS account và cú pháp lệnh cơ bản | 21/10/2025 | 21/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| Thứ Tư | - Thực hành cài đặt AWS CLI trên máy cá nhân, cấu hình thông tin đăng nhập, và kiểm tra với các lệnh quản lý tài nguyên (S3, EC2, Lambda) | 22/10/2025 | 22/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| Thứ Năm | - Học quy trình triển khai hàm Java lên AWS Lambda: chuẩn bị dự án Maven, đóng gói tệp .jar và tạo/tải lên hàm qua AWS CLI | 23/10/2025 | 23/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| Thứ Sáu | - Thực hành triển khai hàm Java lên Lambda thông qua AWS CLI, cấu hình vai trò IAM thích hợp, và kiểm tra hoạt động của hàm | 24/10/2025 | 24/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| Thứ Bảy | - Tìm hiểu cách API Gateway tích hợp với AWS Lambda để phát triển API backend; cấu hình các endpoint và kiểm tra lệnh gọi API | 25/10/2025 | 25/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| Chủ Nhật | - Tổng hợp kiến thức về mối quan hệ giữa Lambda, API Gateway và AWS CLI; ghi chép quy trình triển khai và chuẩn bị báo cáo tuần | 26/10/2025 | 26/10/2025      | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 7:

#### 1. Hiểu Biết Toàn Diện về AWS Lambda

* Nắm vững các khái niệm cơ bản và vai trò của **AWS Lambda** trong các mô hình điện toán không máy chủ.

* Hiểu rõ cơ chế hoạt động của Lambda bao gồm quá trình kích hoạt, vòng đời thực thi hàm và cách trả về kết quả.

* Phân biệt rõ ràng các khác biệt kiến trúc và hoạt động giữa **Lambda** và **EC2** trên nhiều khía cạnh:
  * Trách nhiệm quản lý cơ sở hạ tầng
  * Các mô hình chi phí và cấu trúc lập hóa đơn
  * Các đặc tính khả năng mở rộng và linh hoạt hoạt động

#### 2. Thành Thạo Sử Dụng AWS CLI

* Cài đặt và cấu hình thành công **AWS CLI** trên máy cá nhân sử dụng thông tin xác thực IAM User phù hợp.

* Thể hiện kinh nghiệm thực tế với các lệnh CLI thiết yếu:
  * Liệt kê các tài nguyên S3 bucket
  * Tạo và truy xuất siêu dữ liệu hàm Lambda
  * Quản lý các tài nguyên đám mây AWS
  
* Hiểu toàn diện về cơ chế yêu cầu AWS CLI và các giao thức xác thực sử dụng các cặp Access Key/Secret Key.

#### 3. Kinh Nghiệm Thực Tế: Triển Khai Hàm Java lên AWS Lambda qua CLI

* Xây dựng dự án Java sử dụng framework **Maven**, triển khai các lớp handler và tạo ra các tạo tác .jar có thể thực thi được.

* Thực hiện thành công triển khai hàm Lambda sử dụng lệnh `aws lambda create-function` để tải lên và xuất bản hàm.

* Cấu hình và gán các chính sách **IAM Role** thích hợp để tạo điều kiện thực thi hàm Lambda với các quyền cần thiết.

* Xác thực tính toàn vẹn hoạt động của hàm thông qua các quy trình kiểm tra có hệ thống.


