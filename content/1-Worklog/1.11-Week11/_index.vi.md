---
title: "Tuần 11: GuardScript - Hardening bảo mật và kiểm soát truy cập"
date: 2026-03-20
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### 1. Mục tiêu

* Rà soát và tăng cường các cơ chế bảo mật trọng yếu của backend GuardScript.
* Chuẩn hóa luồng kiểm soát truy cập theo workspace, project và license.
* Tăng khả năng quan sát hệ thống thông qua logging, audit và realtime events.

### 2. Chi tiết công việc trong tuần

| Thứ | Công việc chính | Chi tiết kỹ thuật | Trạng thái |
|:---:|:---|:---|:---:|
| **Hai** | **Rà soát Loader v2** | - Kiểm tra request signature, timestamp/nonce validation.<br>- Rà lại response signature trong execute flow. | Hoàn thành |
| **Ba** | **Rà soát Loader v3** | - Kiểm tra handshake X25519 và AES-GCM.<br>- Đối chiếu luồng bảo mật loader với implementation hiện tại. | Hoàn thành |
| **Tư** | **Hardening Auth và License** | - Rà auth utility, PBKDF2 password hashing, password rotation, rate limiting.<br>- Chuẩn hóa điều kiện license active/inactive, expiration, project binding, HWID lock/reset. | Hoàn thành |
| **Năm** | **Access Control** | - Hoàn thiện access list theo workspace.<br>- Kiểm tra whitelist/blacklist và giới hạn truy cập theo IP. | Hoàn thành |
| **Sáu** | **Logging, Audit và Realtime** | - Rà log theo workspace, admin audit và realtime broadcasts.<br>- Kiểm tra các channel workspace/user/admin trong luồng sự kiện. | Hoàn thành |

### 3. Kết quả đạt được

* Các cơ chế bảo vệ script và xác thực request đã bám sát mô hình bảo mật hiện có trong codebase.
* Luồng license/HWID/access control hoạt động nhất quán hơn với execution flow của loader.
* Hệ thống có khả năng quan sát tốt hơn thông qua logs, audit trail và realtime events.

### 4. Vấn đề & Giải pháp

* **Vấn đề:** Giai đoạn hardening yêu cầu cân bằng giữa mức độ bảo mật và tính tương thích với luồng sử dụng hiện tại.
* **Giải pháp:** Giữ nguyên API surface nhưng siết chặt phần validation, signature, permission check và log sự kiện.

### 5. Bước tiếp theo

* Hoàn thiện tài liệu kỹ thuật để phản ánh đúng implementation.
* Chuẩn bị checklist kiểm thử, deploy và demo dự án.
