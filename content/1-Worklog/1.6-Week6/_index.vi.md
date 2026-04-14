---
title: "Tuần 6: Hội nhập sau Tết và thiết kế backend dự án GuardScript"
date: 2026-02-23
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### 1. Mục tiêu

* Đồng bộ lại tiến độ nhóm sau kỳ nghỉ Tết và chốt dự án chính thức.
* Xác định phạm vi nghiệp vụ của GuardScript theo hướng khả thi về mặt backend.
* Thiết kế kiến trúc ban đầu cho API, dữ liệu và luồng bảo mật của hệ thống.

### 2. Chi tiết công việc trong tuần

| Thứ | Công việc chính | Chi tiết | Trạng thái |
|:---:|:---|:---|:---:|
| **Hai** | **Đồng bộ nhóm sau Tết** | - Kết nối lại với Team TheBois sau kỳ nghỉ Tết.<br>- Rà soát lại các ý tưởng đã có từ trước Tết.<br>- Thống nhất chọn **GuardScript** làm dự án chính thức. | Hoàn thành |
| **Ba** | **Xác định phạm vi backend** | - Chốt các domain backend cốt lõi: workspace, project/script, file, license, team, access control.<br>- Làm rõ phạm vi nghiệp vụ để tránh mở rộng quá mức ở giai đoạn đầu. | Hoàn thành |
| **Tư** | **Thiết kế kiến trúc** | - Thiết kế hướng backend prototype theo mô hình modular monolith.<br>- Lên khung controller theo domain và phác thảo API surface cho các nhóm chức năng chính. | Hoàn thành |
| **Năm** | **Nghiên cứu bảo mật** | - Nghiên cứu AES-GCM cho mã hóa nội dung.<br>- Tìm hiểu ECDH/X25519 cho secure handshake.<br>- Đánh giá PBKDF2 và token-based auth cho cơ chế xác thực. | Hoàn thành |
| **Sáu** | **Chuẩn bị môi trường phát triển** | - Chuẩn bị môi trường Node.js cho backend prototype.<br>- Tổ chức cấu trúc code ban đầu để thuận lợi cho việc phát triển tiếp theo. | Hoàn thành |

### 3. Kết quả đạt được

* Scope của GuardScript đã được chốt tương đối rõ với trọng tâm là backend phân phối script và quản lý license.
* Có thiết kế ban đầu cho các domain quan trọng của hệ thống.
* Có định hướng bảo mật rõ ràng cho password hashing, encryption và secure handshake của loader.

### 4. Vấn đề & Giải pháp

* **Vấn đề:** Cần cân bằng giữa tốc độ làm prototype và khả năng mở rộng cho giai đoạn migrate sau này.
* **Giải pháp:** Chọn hướng prototype đủ gọn ở giai đoạn đầu nhưng vẫn giữ cấu trúc module rõ ràng để thuận lợi khi chuyển sang AWS.

### 5. Bước tiếp theo

* Bắt đầu phát triển backend cốt lõi cho GuardScript.
* Triển khai các chức năng nền tảng như auth, workspace, project và tổ chức dữ liệu.
