---
title: "Blog 2"
date: "2025-09-09"
weight: 1
chapter: false
pre: " <b> 3.2. </b> "
---

# Mở rộng hybrid DNS setup của bạn bằng các endpoint metrics của Amazon Route 53 Resolver

Khi các tổ chức mở rộng môi trường hybrid cloud, việc quản lý phân giải DNS (DNS resolution) giữa on-premises và AWS trở nên phức tạp. Việc chỉ dựa vào các số liệu cũ để dự đoán dung lượng thường không chính xác do chưa tính đến độ trễ mạng và các giao thức phức tạp.

Bài viết này giới thiệu một metric mới trên **Amazon CloudWatch** giúp đơn giản hóa việc ra quyết định mở rộng (scaling) cho **Amazon Route 53 Resolver endpoints**.

---

## Thách thức trong môi trường Hybrid

Trong các kiến trúc DNS tập trung (Centralized DNS architecture), toàn bộ lưu lượng DNS thường đi qua một Hub VPC. Khi lưu lượng tăng, việc thêm các Resolver Networking Interface (RNI) là cần thiết.

Tuy nhiên, các metric truyền thống như `InboundQueryVolume` không phản ánh đúng mức độ sử dụng thực tế vì mỗi RNI chịu ảnh hưởng bởi nhiều yếu tố:
* Giao thức DNS (UDP vs DoH).
* Kích thước phản hồi (Response size).
* Độ trễ khứ hồi (Round-trip latency).

---

## Giải pháp: Metric ResolverEndpointCapacityStatus

AWS đã ra mắt metric **`ResolverEndpointCapacityStatus`** để cung cấp cái nhìn tổng thể về sức khỏe của endpoint. Metric này tự động tính toán các yếu tố hiệu suất và báo cáo trạng thái dựa trên RNI bận rộn nhất.

Metric sử dụng bộ chỉ thị 3 cấp độ đơn giản:

* **0 (OK):** Hoạt động bình thường.
* **1 (Warning):** Đang tiến gần ngưỡng dung lượng.
* **2 (Critical):** Đã vượt quá giới hạn khuyến nghị.

---

## Thử nghiệm và Triển khai

Thông qua các thử nghiệm mô phỏng lưu lượng lớn và độ trễ mạng, metric này cho thấy khả năng cảnh báo sớm chính xác.

1.  **Thiết lập:** Sử dụng Amazon ECS để tạo lưu lượng DNS giả lập và Amazon EC2 để mô phỏng độ trễ.
2.  **Quan sát:** Khi lưu lượng tăng, trạng thái chuyển từ 0 sang 1 và 2, giúp quản trị viên biết chính xác khi nào cần thêm RNI.
3.  **Lưu ý quan trọng:** Cần đảm bảo **cân bằng tải (load balancing)** hiệu quả giữa các RNI để tránh trường hợp một RNI bị quá tải trong khi RNI khác không được sử dụng.

---

## Kết luận

Metric `ResolverEndpointCapacityStatus` loại bỏ sự phỏng đoán trong quản lý dung lượng DNS. Nó cung cấp các tín hiệu rõ ràng, giúp doanh nghiệp thực hiện các hành động mở rộng (scaling) kịp thời và duy trì độ tin cậy cho hạ tầng hybrid cloud.