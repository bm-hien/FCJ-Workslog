---
title: "Tuần 3: Mạng, bảo mật hạ tầng và chuẩn bị môi trường triển khai"
date: 2026-01-19
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### 1. Mục tiêu

* Hiểu sâu hơn về networking trên AWS để phục vụ tư duy triển khai backend an toàn.
* Làm rõ các lớp kiểm soát truy cập ở mức mạng và mức tài nguyên.
* Chuẩn bị nền tảng hạ tầng cho những giai đoạn thiết kế hệ thống về sau.

### 2. Chi tiết công việc trong tuần

| Thứ | Công việc chính | Chi tiết | Trạng thái |
|:---:|:---|:---|:---:|
| **Hai** | **AWS Networking Fundamentals** | - Nghiên cứu VPC, subnet, route table, Internet Gateway và NAT Gateway.<br>- Xây nền tảng cho việc tổ chức backend network topology. | Hoàn thành |
| **Ba** | **Isolation Strategy** | - Phân tích cách cô lập backend components giữa private/public subnets.<br>- Xem xét các nhu cầu truy cập khác nhau theo từng loại dịch vụ. | Hoàn thành |
| **Tư** | **Network Security Practice** | - Thực hành cấu hình bảo mật mạng.<br>- Làm rõ sự khác nhau giữa Security Groups và NACLs trong kiểm soát lưu lượng. | Hoàn thành |
| **Năm** | **Infra Discussion** | - Thảo luận cùng nhóm về yêu cầu hạ tầng cho hệ thống backend.<br>- Tập trung vào việc giảm bề mặt tấn công khi triển khai. | Hoàn thành |
| **Sáu** | **Review & Consolidation** | - Tổng hợp kiến thức networking và security đã học trong tuần.<br>- Chuẩn bị nền tảng cho giai đoạn IAM và authorization. | Hoàn thành |

### 3. Kết quả đạt được

* Có nền tảng tốt hơn về cách tổ chức mạng cho hệ thống backend trên AWS.
* Hiểu rõ hơn cách kết hợp route, gateway và lớp lọc truy cập để bảo vệ tài nguyên.
* Sẵn sàng chuyển từ kiến thức hạ tầng sang tư duy bảo mật hệ thống và phân quyền truy cập.

### 4. Vấn đề & Giải pháp

* **Vấn đề:** Dễ nhầm lẫn giữa phạm vi áp dụng của Security Groups và NACLs khi mới tiếp cận.
* **Giải pháp:** Kiểm tra lại theo từng luồng truy cập thực tế để gắn khái niệm với hành vi hệ thống.

### 5. Bước tiếp theo

* Chuyển trọng tâm sang IAM, policy và cơ chế phân quyền.
* Chuẩn bị nền tảng cho các quyết định liên quan đến auth, role và security posture của backend.
