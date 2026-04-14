---
title: "Week 9: GuardScript - Backend Migration to AWS"
date: 2026-03-16
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### 1. Objectives

* Move GuardScript from the local prototype to an AWS serverless architecture.
* Redesign the backend data and infrastructure layers to fit Lambda, DynamoDB, and S3.
* Stabilize the main business flows after migration.

### 2. Weekly Tasks Breakdown

| Day | Main Task | Details | Status |
|:---:|:---|:---|:---:|
| **Mon** | **Migration Planning** | - Reviewed the old prototype and identified the parts that needed migration.<br>- Clarified changes across runtime, database, storage, and deployment flow. | Completed |
| **Tue** | **Lambda Backend Restructure** | - Reorganized the backend into a Lambda-based modular monolith.<br>- Centralized routing and kept controllers separated by domain for AWS deployment. | Completed |
| **Wed** | **DynamoDB Data Redesign** | - Designed the multi-table model and GSIs for users, workspaces, projects, licenses, invitations, and logs.<br>- Standardized data access paths for the API layer. | Completed |
| **Thu** | **S3 Storage Migration** | - Shifted file and script storage to S3 using content references.<br>- Reduced dependency on the local prototype storage pattern. | Completed |
| **Fri** | **AWS Infrastructure Setup** | - Used SAM/CloudFormation to deploy Lambda, S3, CloudFront, DynamoDB, and WebSocket API.<br>- Adjusted backend flows so frontend integration could continue after migration. | Completed |

### 3. Outcomes

* The backend moved toward a clearer AWS-centric architecture.
* The migration path from local prototype storage to DynamoDB and S3 became technically grounded.
* Infrastructure-as-code now reflected the main deployment components of the system.

### 4. Issues & Solutions

* **Issue:** Migration required changing runtime model, persistence strategy, and data access patterns at the same time.
* **Solution:** Preserved a reasonable API surface while replacing the storage and deployment layers underneath.

### 5. Next Steps

* Run end-to-end integration checks between frontend and backend on AWS.
* Continue stabilizing APIs and resolving migration-related issues.
