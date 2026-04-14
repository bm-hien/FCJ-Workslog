---
title: "Tuần 8: GuardScript - Phát triển tính năng backend và module bảo vệ script"
date: 2026-03-09
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### 1. Mục tiêu

* Mở rộng backend sang các nhóm chức năng chính của GuardScript.
* Hoàn thiện luồng quản lý project, file, license, team và access control.
* Triển khai module bảo vệ script và chuẩn bị cho việc migrate lên AWS.

### 2. Chi tiết công việc trong tuần

| Thứ | Công việc chính | Chi tiết | Trạng thái |
|:---:|:---|:---|:---:|
| **Hai** | **Phát triển project/file flow** | - Xây dựng API tạo script, cập nhật nội dung, tổ chức file tree và đặt entry point.<br>- Chuẩn bị nền tảng cho bundle và protected content flow. | Hoàn thành |
| **Ba** | **Hoàn thiện license management** | - Triển khai tạo license đơn lẻ và hàng loạt.<br>- Hỗ trợ export license, toggle trạng thái, HWID lock và reset HWID. | Hoàn thành |
| **Tư** | **Team và phân quyền workspace** | - Xây dựng invitation flow và role-based team management trong workspace.<br>- Chuẩn hóa xử lý member/invitation theo backend logic. | Hoàn thành |
| **Năm** | **Access control và protection module** | - Xây dựng access list theo whitelist/blacklist.<br>- Tích hợp mã hóa nội dung và chuẩn bị loader cho các ngôn ngữ được hỗ trợ. | Hoàn thành |
| **Sáu** | **Hỗ trợ tích hợp frontend** | - Kiểm tra hành vi API với frontend workspace.<br>- Điều chỉnh response data để thuận lợi cho việc hiển thị và tích hợp ở giao diện. | Hoàn thành |

### 3. Kết quả đạt được

* Các module backend trọng tâm của GuardScript đã được hình thành tương đối đầy đủ.
* Luồng quản lý dữ liệu theo workspace/project/license rõ ràng hơn và có thể tích hợp với frontend.
* Module bảo vệ script bắt đầu có đầu ra kỹ thuật cụ thể thay vì chỉ dừng ở mức thiết kế.

### 4. Vấn đề & Giải pháp

* **Vấn đề:** Khối lượng chức năng backend tăng nhanh, đòi hỏi giữ sự nhất quán giữa quyền truy cập, dữ liệu và response format.
* **Giải pháp:** Gom logic theo domain và ưu tiên chuẩn hóa flow trước khi tiếp tục mở rộng thêm tính năng.

### 5. Bước tiếp theo

* Bắt đầu migration GuardScript sang kiến trúc AWS serverless.
* Chuyển trọng tâm sang tổ chức dữ liệu DynamoDB, storage trên S3 và deploy backend trên Lambda.
