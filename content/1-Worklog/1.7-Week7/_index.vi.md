---
title: "Tuần 7: GuardScript - Phát triển backend cốt lõi"
date: 2026-03-02
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### 1. Mục tiêu

* Khởi động giai đoạn phát triển chính thức của GuardScript.
* Thiết lập backend prototype và các domain nền tảng của hệ thống.
* Xây dựng các API đầu tiên để frontend có thể bắt đầu tích hợp.

### 2. Chi tiết công việc trong tuần

| Thứ | Công việc chính | Chi tiết | Trạng thái |
|:---:|:---|:---|:---:|
| **Hai** | **Rà soát kiến trúc** | - Rà soát lại kiến trúc tổng thể sau khi chốt scope.<br>- Xác định các phần backend cần ưu tiên triển khai trước. | Hoàn thành |
| **Ba** | **Thiết lập backend prototype** | - Thiết lập backend theo hướng Node.js/Express.<br>- Chuẩn bị cấu trúc controller, utils và lớp dữ liệu cho các domain chính. | Hoàn thành |
| **Tư** | **Xây dựng auth cơ bản** | - Triển khai luồng đăng ký, đăng nhập, quản lý hồ sơ người dùng và cơ chế token.<br>- Chuẩn bị nền tảng cho các màn hình login/register tích hợp với backend. | Hoàn thành |
| **Năm** | **Khởi tạo workspace/project** | - Khởi tạo xử lý workspace và project ở mức nền tảng.<br>- Tạo khung cho các tính năng quản lý dữ liệu ở các tuần tiếp theo. | Hoàn thành |
| **Sáu** | **Phối hợp tích hợp ban đầu** | - Thống nhất API contract cơ bản với frontend cho login/register và truy cập dữ liệu ban đầu.<br>- Rà lại response để thuận lợi cho tích hợp sớm. | Hoàn thành |

### 3. Kết quả đạt được

* Backend đã có cấu trúc ban đầu đủ rõ để mở rộng tiếp các module nghiệp vụ.
* Luồng auth cơ bản được hình thành, tạo nền cho các trang login/register và dashboard tích hợp.
* Việc phân tách controller theo domain giúp nhóm dễ song song hóa phát triển hơn.

### 4. Vấn đề & Giải pháp

* **Vấn đề:** Giai đoạn đầu cần vừa chốt cấu trúc backend vừa đảm bảo đủ đầu ra để frontend tích hợp sớm.
* **Giải pháp:** Ưu tiên triển khai các API nền tảng trước, sau đó mới mở rộng các module phức tạp hơn.

### 5. Bước tiếp theo

* Mở rộng các API cho project, file, license và team.
* Bắt đầu hiện thực hóa luồng bảo vệ script và quản lý nội dung thực thi.
