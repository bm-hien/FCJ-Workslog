---
title: "Tuần 4: Định danh, phân quyền và định hướng bảo mật hệ thống"
date: 2026-01-26
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### 1. Mục tiêu

* Nắm vững IAM và nguyên tắc least privilege để chuẩn bị cho việc vận hành backend an toàn.
* Hiểu rõ hơn cách tổ chức users, groups, roles và policy trong môi trường AWS.
* Đánh giá các hướng công nghệ có thể hỗ trợ kiến trúc backend của dự án.

### 2. Chi tiết công việc trong tuần

| Thứ | Công việc chính | Chi tiết | Trạng thái |
|:---:|:---|:---|:---:|
| **Hai** | **IAM Structure** | - Tìm hiểu cách tổ chức IAM User, Group và Role cho môi trường làm việc nhóm.<br>- Liên hệ các khái niệm này với cách kiểm soát truy cập tài nguyên backend. | Hoàn thành |
| **Ba** | **Least-Privilege Policies** | - Thực hành viết và rà soát policy theo hướng giới hạn phạm vi truy cập.<br>- Tránh cấp quyền quá rộng cho tài nguyên AWS. | Hoàn thành |
| **Tư** | **MFA và Account Security** | - Áp dụng tư duy MFA và quản trị tài khoản an toàn.<br>- Giảm phụ thuộc vào root account trong công việc hằng ngày. | Hoàn thành |
| **Năm** | **Technology Update** | - Tham dự hoạt động cập nhật công nghệ từ AWS re:Invent Recap.<br>- Mở rộng góc nhìn về các dịch vụ có thể hỗ trợ backend. | Hoàn thành |
| **Sáu** | **Architecture Relevance Review** | - Đánh giá các hướng như Cognito và dịch vụ dữ liệu mới cho bài toán auth, data flow và logging.<br>- Tổng hợp lại các điểm có thể áp dụng cho dự án. | Hoàn thành |

### 3. Kết quả đạt được

* Hiểu rõ hơn cách kiểm soát truy cập tài nguyên AWS ở mức người dùng và vai trò.
* Có nền tảng tốt cho các quyết định sau này liên quan đến xác thực, phân quyền và bảo mật backend.
* Củng cố tư duy chỉ cấp quyền đúng mức cần thiết cho từng thành phần hệ thống.

### 4. Vấn đề & Giải pháp

* **Vấn đề:** Việc viết policy chi tiết theo ARN tương đối dễ sai khi mới thực hành.
* **Giải pháp:** Dùng công cụ hỗ trợ sinh policy nháp, sau đó kiểm tra và tinh chỉnh thủ công theo tài nguyên thực tế.

### 5. Bước tiếp theo

* Chuyển sang nghiên cứu kiến trúc serverless và cách tổ chức backend trên Lambda, API Gateway và DynamoDB.
* Bắt đầu liên kết kiến thức hạ tầng với ý tưởng sản phẩm thực tế của nhóm.
