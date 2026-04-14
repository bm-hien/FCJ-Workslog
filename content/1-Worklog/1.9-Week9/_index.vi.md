---
title: "Tuần 9: GuardScript - Migration backend lên AWS"
date: 2026-03-16
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### 1. Mục tiêu

* Chuyển GuardScript từ prototype local sang kiến trúc AWS serverless.
* Thiết kế lại lớp dữ liệu và hạ tầng backend để phù hợp với Lambda, DynamoDB và S3.
* Ổn định các luồng nghiệp vụ chính sau migration.

### 2. Chi tiết công việc trong tuần

| Thứ | Công việc chính | Chi tiết | Trạng thái |
|:---:|:---|:---|:---:|
| **Hai** | **Lập kế hoạch migration** | - Rà soát prototype cũ và xác định các thành phần cần migrate.<br>- Làm rõ thay đổi về runtime, database, storage và deployment flow. | Hoàn thành |
| **Ba** | **Tái cấu trúc backend trên Lambda** | - Tổ chức backend theo mô hình Lambda modular monolith.<br>- Gom router và tách controller theo domain để phù hợp môi trường AWS. | Hoàn thành |
| **Tư** | **Thiết kế lại dữ liệu DynamoDB** | - Thiết kế multi-table và GSI cho các query chính như users, workspaces, projects, licenses, invitations và logs.<br>- Chuẩn hóa hướng truy xuất dữ liệu phục vụ API. | Hoàn thành |
| **Năm** | **Chuyển storage sang S3** | - Chuyển luồng lưu trữ file/script sang S3 với content reference.<br>- Giảm phụ thuộc vào cách lưu dữ liệu của prototype local trước đó. | Hoàn thành |
| **Sáu** | **Xây dựng hạ tầng AWS** | - Dùng SAM/CloudFormation để triển khai Lambda, S3, CloudFront, DynamoDB và WebSocket API.<br>- Điều chỉnh các flow backend để frontend vẫn tiếp tục tích hợp được sau migration. | Hoàn thành |

### 3. Kết quả đạt được

* Backend đã được đưa về kiến trúc AWS-centric rõ ràng hơn.
* Luồng dữ liệu từ local prototype sang DynamoDB/S3 có cơ sở triển khai thực tế.
* Hạ tầng triển khai đã có template IaC đủ phản ánh các thành phần chính của hệ thống.

### 4. Vấn đề & Giải pháp

* **Vấn đề:** Migration đòi hỏi chuyển đổi đồng thời mô hình runtime, storage và cách truy xuất dữ liệu.
* **Giải pháp:** Giữ API surface ở mức hợp lý trong khi thay lớp persistence và deployment phía dưới.

### 5. Bước tiếp theo

* Kiểm thử tích hợp end-to-end giữa frontend và backend trên AWS.
* Tiếp tục ổn định các API và xử lý các lỗi phát sinh sau migration.
