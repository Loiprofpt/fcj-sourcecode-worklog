---
title: "Worklog Tuần 11"
date: "2025-09-10"
weight: 2
chapter: false
pre: " <b> 1.11. </b> "
---

### Mục tiêu tuần 11:

* Mua sắm và lắp ráp **các thành phần phần cứng IoT** bao gồm vi điều khiển ESP32 và bộ cảm biến toàn diện.
* Phát triển **phần mềm nhúng** cho các module cảm biến riêng lẻ và tích hợp hệ thống hoàn chỉnh.
* Triển khai **kết nối AWS IoT Core** để truyền dữ liệu lên đám mây và quản lý thiết bị từ xa.
* Thiết lập **kiểm tra và xác thực phần cứng end-to-end** của tất cả các thành phần hệ thống.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| Thứ Hai   | - Mua sắm ESP32 và các module cảm biến: MAX30201, cảm biến nhịp tim, cảm biến vân tay, màn hình OLED, keypad 4x4, buzzer, LED, cảm biến đo nồng độ rượu/O2                                                                                   | 11/17/2025   | 11/17/2025      | <https://cloudjourney.awsstudygroup.com/> |
| Thứ Ba   | - Thiết kế kiến trúc phần cứng và phát triển code driver cho từng cảm biến (nhiệt độ, nhịp tim, vân tay, cảm biến môi trường)                                             | 11/18/2025   | 11/18/2025      | <https://cloudjourney.awsstudygroup.com/> |
| Thứ Tư   | - Tích hợp các module cảm biến với ESP32, cấu hình kết nối WiFi, và triển khai giao thức tuần tự hóa dữ liệu | 11/19/2025   | 11/19/2025      | <https://cloudjourney.awsstudygroup.com/> |
| Thứ Năm   | - Cấu hình AWS IoT Core MQTT, triển khai xác thực chứng chỉ thiết bị, và thiết lập đường ống truyền dữ liệu an toàn                            | 11/20/2025   | 11/20/2025      | <https://cloudjourney.awsstudygroup.com/> |
| Thứ Sáu   | - Thực hiện kiểm tra phần cứng toàn diện, xác thực độ chính xác cảm biến, xác minh truyền dữ liệu lên đám mây, và tài liệu hóa thông số kỹ thuật                                                                                     | 11/21/2025   | 11/21/2025      | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 11:

#### 1. Mua Sắm và Tích Hợp Thành Phần Phần Cứng IoT

* Thành công mua sắm và kiểm kê tất cả các thành phần phần cứng cần thiết:
  * **Bảng ESP32** làm vi điều khiển chính
  * **Cảm Biến Nhiệt Độ MAX30201** cho phép đo lường cấp độc lập phòng khám
  * **Cảm Biến Nhịp Tim** để theo dõi tim mạch
  * **Module Nhận Dạng Vân Tay** cho xác định sinh trắc học
  * **Màn Hình OLED** để hiển thị dữ liệu thực tế
  * **Ma Trận Keypad 4x4** cho giao diện nhập người dùng
  * **Buzzer và Chỉ Báo LED** để phản hồi hệ thống
  * **Cảm Biến Nồng Độ Rượu/O2** cho giám sát môi trường

#### 2. Phát Triển Phần Mềm Nhúng

* Phát triển **thư viện driver thiết bị** toàn diện cho từng cảm biến với chức năng đầy đủ:
  * Cảm biến nhiệt độ với triển khai giao thức MAX30201
  * Phát hiện nhịp tim và thuật toán tính BPM
  * Cơ chế khớp và lưu trữ vân tay
  * Điều khiển hiển thị OLED và kết xuất dữ liệu
  * Xử lý đầu vào keypad nhiều nút
  * Hiệu chuẩn cảm biến hóa học và tối ưu hóa đọc số

* Triển khai **kiến trúc phần mềm mô-đun** cho phép kiểm tra cảm biến độc lập và hoạt động hệ thống tích hợp.

#### 3. Tích Hợp AWS IoT Core

* Thành công cấu hình **kết nối WiFi ESP32** với xử lý mạng mạnh mẽ và logic tái kết nối.

* Thiết lập **giao tiếp AWS IoT Core MQTT** với:
  * Xác thực và ủy quyền chứng chỉ thiết bị thích hợp
  * Truyền dữ liệu được mã hóa an toàn TLS/SSL
  * Cấu trúc chủ đề Pub-Sub cho các luồng dữ liệu cảm biến
  * Xếp hàng tin nhắn và cơ chế thử lại khả năng ngoại tuyến

#### 4. Lắp Ráp Phần Cứng và Tích Hợp Hệ Thống

* Hoàn thành **lắp ráp phần cứng vật lý** với thiết kế mạch thích hợp và kết nối thành phần.

* Tích hợp tất cả các module cảm biến vào hệ thống dựa trên ESP32 thống nhất với:
  * Phân phối điện năng thích hợp và điều chỉnh điện áp
  * Điều hòa tín hiệu và lọc tiếng ồn
  * Thu thập và xử lý dữ liệu cảm biến phối hợp

#### 5. Kiểm Tra Phần Cứng Toàn Diện và Xác Thực

* Tiến hành **kiểm tra phần cứng có hệ thống** xác thực:
  * Độ chính xác và hiệu chuẩn cảm biến riêng lẻ
  * Độ tin cậy truyền dữ liệu qua WiFi và MQTT
  * Thu thập dữ liệu cảm biến thực tế và đồng bộ hóa đám mây
  * Ổn định hệ thống dưới hoạt động kéo dài
  * Tối ưu hóa hiệu quả pin và tiêu thụ điện năng

* Tạo **tài liệu kỹ thuật** bao gồm thông số cảm biến, quy trình hiệu chuẩn và hướng dẫn tích hợp.


