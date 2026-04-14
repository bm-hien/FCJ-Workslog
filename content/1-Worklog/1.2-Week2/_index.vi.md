---
title: "Tuần 2: Lưu trữ, cơ sở dữ liệu và định hướng kiến trúc hệ thống"
date: 2026-01-12
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### 1. Mục tiêu

* Tìm hiểu sâu hơn về các dịch vụ lưu trữ và cơ sở dữ liệu của AWS.
* Thực hành bài toán upload file để hiểu luồng backend kết nối với object storage.
* Tham gia giai đoạn khởi động dự án và thảo luận định hướng kiến trúc hệ thống.

### 2. Chi tiết công việc trong tuần

| Thứ | Công việc chính | Chi tiết | Trạng thái |
|:---:|:---|:---|:---:|
| **Hai** | **Storage & Database Study** | - Nghiên cứu S3, EBS và RDS với góc nhìn backend.<br>- Tập trung vào cách lưu trữ dữ liệu, snapshot và khả năng mở rộng. | Hoàn thành |
| **Ba** | **Hands-on Upload Flow** | - Thực hành xây dựng luồng upload file với S3.<br>- Tìm hiểu cách backend tiếp nhận, xử lý và lưu trữ nội dung trên cloud. | Hoàn thành |
| **Tư** | **Architecture Discussion** | - Tham gia thảo luận proposal giai đoạn đầu.<br>- Đánh giá hướng tổ chức dữ liệu và khả năng tách core logic khỏi hạ tầng triển khai. | Hoàn thành |
| **Năm** | **Portability Review** | - Đánh giá cách thiết kế để hệ thống có thể vận hành ở local và cloud.<br>- Hạn chế phụ thuộc cứng vào một nền tảng duy nhất. | Hoàn thành |
| **Sáu** | **Weekly Review** | - Tổng hợp lại kiến thức về storage và database.<br>- Rút ra các điểm cần lưu ý cho những bài toán backend có xử lý file. | Hoàn thành |

### 3. Kết quả đạt được

* Nắm rõ hơn vai trò của object storage trong các bài toán backend có xử lý file.
* Có trải nghiệm thực tế về cách backend kết nối với S3 và tổ chức luồng upload.
* Bắt đầu hình thành tư duy kiến trúc theo hướng tách lớp xử lý nghiệp vụ khỏi lớp hạ tầng.

### 4. Vấn đề & Giải pháp

* **Vấn đề:** Việc xác định phạm vi dự án ở giai đoạn đầu còn rộng và nhiều khả năng mở rộng.
* **Giải pháp:** Ưu tiên phân tích các thành phần backend cốt lõi trước để giữ kiến trúc đủ linh hoạt cho thay đổi sau này.

### 5. Bước tiếp theo

* Tiếp tục củng cố kiến thức về networking và security trên AWS.
* Chuẩn bị nền tảng cho việc thiết kế backend an toàn hơn trong các giai đoạn tiếp theo.
