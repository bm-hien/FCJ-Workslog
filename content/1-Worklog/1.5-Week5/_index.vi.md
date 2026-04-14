---
title: "Tuần 5: Tìm hiểu serverless và hình thành ý tưởng backend cho GuardScript"
date: 2026-02-02
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### 1. Mục tiêu

* Nghiên cứu sâu hơn về kiến trúc serverless trên AWS.
* Đánh giá cách Lambda, API Gateway và DynamoDB có thể ghép thành backend cho sản phẩm thực tế.
* Brainstorm ý tưởng dự án và xác định hướng bài toán phù hợp với năng lực triển khai của nhóm.

### 2. Chi tiết công việc trong tuần

| Thứ | Công việc chính | Chi tiết | Trạng thái |
|:---:|:---|:---|:---:|
| **Hai** | **Lambda Deep Dive** | - Tìm hiểu mô hình thực thi Lambda, statelessness, cold start và Function URL.<br>- Đánh giá cách Lambda có thể dùng làm nền cho backend. | Hoàn thành |
| **Ba** | **API Gateway & DynamoDB** | - Nghiên cứu API Gateway và DynamoDB theo hướng query pattern.<br>- Tìm hiểu partition key, GSI và cách thiết kế dữ liệu phục vụ API. | Hoàn thành |
| **Tư** | **Hands-on Serverless API** | - Xây dựng CRUD API đơn giản theo hướng serverless.<br>- Kiểm chứng khả năng làm backend không cần server truyền thống. | Hoàn thành |
| **Năm** | **Project Brainstorming** | - Tham gia brainstorming cùng team về secure code distribution, licensing và script management.<br>- Cùng nhóm hình thành ý tưởng ban đầu cho **GuardScript**. | Hoàn thành |
| **Sáu** | **Pre-Tet Review** | - Tổng hợp lại các điểm kỹ thuật đã học trong tuần 1-5.<br>- Chuẩn bị nền tư duy cho việc chốt scope và thiết kế backend sau Tết. | Hoàn thành |

### 3. Kết quả đạt được

* Có cơ sở kỹ thuật rõ ràng cho việc chọn hướng serverless cho giai đoạn triển khai sau này.
* Kiểm chứng được cách triển khai API backend đơn giản bằng Lambda kết hợp DynamoDB.
* Hình thành ý tưởng sản phẩm GuardScript với các thành phần backend cốt lõi tương đối rõ ràng.

### 4. Vấn đề & Giải pháp

* **Vấn đề:** DynamoDB yêu cầu tư duy thiết kế khác với mô hình cơ sở dữ liệu quan hệ quen thuộc.
* **Giải pháp:** Tiếp cận theo query pattern trước, sau đó mới suy ra schema và index cần thiết.

### 5. Bước tiếp theo

* Sau kỳ nghỉ Tết sẽ quay lại để chốt phạm vi GuardScript.
* Bắt đầu thiết kế chi tiết kiến trúc backend, API surface và luồng bảo mật của hệ thống.
