---
title: "BLog 3"
date: "2025-09-09"
weight: 1
chapter: false
pre: " <b> 3.3. </b> "
---

# Cách Khoa Thể thao Đại học Minnesota xây dựng một lớp dữ liệu thống nhất để tăng tương tác với người hâm mộ bằng AWS

Mỗi vé bán ra cho một sự kiện thể thao của Đại học Minnesota được chuyển tay trung bình ba lần. Với hơn một triệu người đi qua cổng soát vé mỗi năm, khối lượng dữ liệu giao dịch là khổng lồ.

Minnesota Athletics đã đối mặt với thách thức về dữ liệu phân mảnh và quy trình xử lý thủ công tốn thời gian. Chỉ trong chưa đầy một năm, họ đã thay thế sự phức tạp đó bằng một **data lake** có khả năng mở rộng trên AWS.

---

## "Hiên nhà" của trường đại học

Minnesota Athletics hỗ trợ hơn 600 vận động viên sinh viên và đóng vai trò là "hiên nhà" kết nối công chúng với trường đại học. Tuy nhiên, hệ thống cũ bao gồm các công cụ của bên thứ ba kết nối lỏng lẻo, khiến dữ liệu chỉ được chia sẻ một chiều và không đủ để phân tích sâu về hành vi người hâm mộ.

---

## Giải pháp: Data Lake thống nhất trên AWS

Với mục tiêu sở hữu dữ liệu để phân tích thời gian thực, nhóm đã xây dựng một lớp dữ liệu tập trung mà không cần đại tu toàn bộ hệ thống cũ.

#### Tại sao chọn AWS?
* **Chi phí hiệu quả:** Mô hình pay-as-you-go cho phép bắt đầu nhỏ và mở rộng dần.
* **Quyền kiểm soát:** Nhóm giữ toàn quyền kiểm soát dữ liệu của mình.
* **Triển khai nhanh:** Tận dụng thỏa thuận có sẵn của trường với AWS để provisioning nhanh chóng.

---

## Kiến trúc hệ thống: An toàn và Linh hoạt

Một nhóm nội bộ nhỏ gồm 3 người đã hoàn thành nền tảng này trong chưa đầy 8 tháng. Kiến trúc sử dụng các dịch vụ serverless để đảm bảo tính tự động hóa và bảo mật:

1.  **Thu thập:** Dữ liệu bán vé được chuyển an toàn qua SFTP vào **Amazon S3** (môi trường riêng tư).
2.  **Bảo mật:** Quản lý quyền truy cập chặt chẽ bằng **AWS Secrets Manager**.
3.  **Xử lý:** **AWS Lambda** và **AWS Glue** tự động làm sạch, loại bỏ bản sao và chuẩn hóa dữ liệu ngay khi file đến.
4.  **Dự phòng:** Các kiểm tra tự động và versioning trong S3 giúp ngăn ngừa mất dữ liệu.

---

## Tác động kinh doanh

Việc tập trung dữ liệu đã mang lại những kết quả tức thì:

* **Tối ưu doanh thu:** Mô hình dự đoán giá vé giúp dự báo tăng **3–5% doanh thu** và giảm thiểu thua lỗ ngay cả trong những năm khó khăn.
* **Golden Record:** Tạo ra hồ sơ khách hàng thống nhất bằng cách liên kết dữ liệu từ vé, bán lẻ, và đóng góp để hiểu rõ giá trị của từng người hâm mộ.

---

## Bài học kinh nghiệm

Travis Cameron chia sẻ lời khuyên cho các tổ chức khác:
* **Bắt đầu nhỏ:** Tập trung vào một mục tiêu rõ ràng (ví dụ: chỉ dữ liệu bán vé) cho giai đoạn đầu.
* **Tận dụng nguồn lực:** Sử dụng các thỏa thuận AWS hiện có của tổ chức.
* **Nhóm nhỏ vẫn hiệu quả:** Một nhóm 3 người có thể chuẩn hóa hạ tầng dữ liệu nếu có tầm nhìn rõ ràng.