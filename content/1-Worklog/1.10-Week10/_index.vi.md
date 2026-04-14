---
title: "Tuần 10: GuardScript - Tích hợp hệ thống, kiểm thử và ổn định backend"
date: 2026-03-23
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### 1. Mục tiêu

* Ổn định backend sau giai đoạn migration lên AWS.
* Kiểm thử luồng tích hợp end-to-end giữa frontend và backend.
* Chuẩn hóa thêm các API, response và cấu hình triển khai để giảm lỗi khi demo.

### 2. Chi tiết công việc trong tuần

| Thứ | Công việc chính | Chi tiết | Trạng thái |
|:---:|:---|:---|:---:|
| **Hai** | **Kiểm thử luồng chính** | - Kiểm tra luồng đăng ký, đăng nhập, tạo workspace, tạo project, thao tác file và license.<br>- Ghi nhận các điểm phát sinh lỗi sau migration. | Hoàn thành |
| **Ba** | **Rà soát API tích hợp** | - Rà lại các API như workspace details, project listing, execution summary và user stats.<br>- Điều chỉnh response cho phù hợp với frontend sau khi chạy trên AWS. | Hoàn thành |
| **Tư** | **Xử lý lỗi integration** | - Phối hợp xử lý các lỗi frontend-backend trên AWS.<br>- Kiểm tra routing, CORS, headers và dữ liệu trả về. | Hoàn thành |
| **Năm** | **Rà deployment flow** | - Kiểm tra Lambda Function URL, CloudFront rewrite behavior, S3 frontend hosting và backend environment variables.<br>- Đảm bảo flow triển khai khớp với hệ thống thực tế. | Hoàn thành |
| **Sáu** | **Cập nhật tài liệu kỹ thuật** | - Hỗ trợ cập nhật README và mô tả kiến trúc.<br>- Đồng bộ mô tả hệ thống với trạng thái backend đã triển khai. | Hoàn thành |

### 3. Kết quả đạt được

* Backend sau migration đã ổn định hơn ở mức tích hợp hệ thống.
* Các API chính phục vụ dashboard/workspace có thể đáp ứng tốt hơn cho frontend.
* Quy trình triển khai và kiểm thử end-to-end được làm rõ hơn trước giai đoạn hardening và hoàn thiện tài liệu.

### 4. Vấn đề & Giải pháp

* **Vấn đề:** Một số lỗi chỉ xuất hiện khi chạy môi trường AWS thật, không lộ rõ ở local prototype.
* **Giải pháp:** Kiểm tra lại toàn bộ flow request/response, header và cấu hình rewrite giữa frontend và backend.

### 5. Bước tiếp theo

* Chuyển trọng tâm sang hardening bảo mật, access control và khả năng quan sát hệ thống.
* Siết chặt các validation liên quan đến loader, license, rate limiting và logging.
