---
title: "Week 6: Post-Tet Sync-up and Backend Design for GuardScript"
date: 2026-02-23
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### 1. Objectives

* Sync the team after the Tet holiday and finalize the official project direction.
* Define the business scope of GuardScript from a backend feasibility perspective.
* Design the initial architecture for APIs, data flow, and security mechanisms.

### 2. Weekly Tasks Breakdown

| Day | Main Task | Details | Status |
|:---:|:---|:---|:---:|
| **Mon** | **Post-Tet Team Sync** | - Reconnected with Team TheBois after the Tet holiday.<br>- Reviewed the ideas discussed before the break.<br>- Finalized **GuardScript** as the official project. | Completed |
| **Tue** | **Backend Scope Definition** | - Defined core backend domains: workspace, project/script, file, license, team, and access control.<br>- Clarified business scope to avoid overexpansion in the initial phase. | Completed |
| **Wed** | **Architecture Design** | - Designed the prototype backend around a modular monolith approach.<br>- Drafted domain-based controllers and the API surface for major functional areas. | Completed |
| **Thu** | **Security Research** | - Studied AES-GCM for content encryption.<br>- Explored ECDH/X25519 for secure handshake flow.<br>- Evaluated PBKDF2 and token-based auth for authentication design. | Completed |
| **Fri** | **Development Environment Setup** | - Prepared the Node.js environment for the backend prototype.<br>- Organized the initial code structure for the next implementation phase. | Completed |

### 3. Outcomes

* Finalized a clearer scope for GuardScript with backend-driven script distribution and license management at the center.
* Established an initial design for the most important system domains.
* Built a concrete security direction for password hashing, encryption, and secure loader handshake design.

### 4. Issues & Solutions

* **Issue:** The main challenge was balancing fast prototype delivery with later migration and scalability.
* **Solution:** Kept the first version simple while preserving a module structure that could transition cleanly to AWS.

### 5. Next Steps

* Start implementing the backend core of GuardScript.
* Build foundational features such as auth, workspace, project handling, and data organization.
