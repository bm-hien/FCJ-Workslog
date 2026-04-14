---
title: "Week 11: GuardScript - Security Hardening and Access Control"
date: 2026-03-20
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### 1. Objectives

* Review and strengthen the most important backend security mechanisms in GuardScript.
* Standardize access control flow across workspace, project, and license boundaries.
* Improve system observability through logging, audit trails, and realtime events.

### 2. Weekly Tasks Breakdown

| Day | Main Task | Technical Details | Status |
|:---:|:---|:---|:---:|
| **Mon** | **Loader v2 Review** | - Checked request signatures, timestamp and nonce validation.<br>- Reviewed response signature handling in the execute flow. | Completed |
| **Tue** | **Loader v3 Review** | - Verified the X25519 and AES-GCM handshake flow.<br>- Compared the loader security flow against the current implementation. | Completed |
| **Wed** | **Auth and License Hardening** | - Reviewed auth utilities, PBKDF2 password hashing, password rotation, and rate limiting.<br>- Standardized license active/inactive state, expiration, project binding, and HWID lock/reset behavior. | Completed |
| **Thu** | **Access Control** | - Completed workspace-level access list handling.<br>- Checked whitelist, blacklist, and IP-based restriction logic. | Completed |
| **Fri** | **Logging, Audit, and Realtime** | - Reviewed workspace logs, admin audit, and realtime broadcasts.<br>- Checked workspace, user, and admin event channels. | Completed |

### 3. Outcomes

* Script protection and request verification mechanisms were aligned more closely with the implemented security model in the codebase.
* License, HWID, and access-control flow became more consistent with the loader execution path.
* System observability improved through logs, audit trail support, and realtime events.

### 4. Issues & Solutions

* **Issue:** The hardening phase required balancing stronger security with compatibility for the existing usage flow.
* **Solution:** Preserved the API surface while tightening validation, signatures, permission checks, and event logging.

### 5. Next Steps

* Finalize technical documentation so it accurately reflects the implementation.
* Prepare testing, deployment, and demo checklists.
