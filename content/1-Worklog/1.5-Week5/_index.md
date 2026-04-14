---
title: "Week 5: Learning Serverless and Forming the Backend Idea for GuardScript"
date: 2026-02-02
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### 1. Objectives

* Study serverless architecture on AWS in more depth.
* Evaluate how Lambda, API Gateway, and DynamoDB can be combined into a real backend system.
* Brainstorm project ideas and identify a direction that matches the team’s implementation capacity.

### 2. Weekly Tasks Breakdown

| Day | Main Task | Details | Status |
|:---:|:---|:---|:---:|
| **Mon** | **Lambda Deep Dive** | - Studied the Lambda execution model, statelessness, cold starts, and Function URL.<br>- Evaluated how Lambda could serve as the backend runtime foundation. | Completed |
| **Tue** | **API Gateway and DynamoDB** | - Explored API Gateway and DynamoDB from a query-pattern perspective.<br>- Studied partition keys, GSIs, and API-oriented data design. | Completed |
| **Wed** | **Hands-on Serverless API** | - Built a simple CRUD API in a serverless style.<br>- Validated backend feasibility without a traditional server model. | Completed |
| **Thu** | **Project Brainstorming** | - Joined team brainstorming around secure code distribution, licensing, and script management.<br>- Helped shape the initial idea of **GuardScript**. | Completed |
| **Fri** | **Pre-Tet Review** | - Consolidated the technical lessons learned from weeks 1-5.<br>- Prepared the thinking needed for scope finalization and backend design after the Tet break. | Completed |

### 3. Outcomes

* Built a solid technical basis for choosing a serverless direction for later deployment.
* Validated how backend APIs can be implemented with Lambda and DynamoDB.
* Formed a clearer product idea for GuardScript with identifiable backend core components.

### 4. Issues & Solutions

* **Issue:** DynamoDB required a different design mindset compared to relational databases.
* **Solution:** Approached schema design through expected query patterns first, then derived tables and indexes from those needs.

### 5. Next Steps

* After the Tet break, return to finalize the scope of GuardScript.
* Begin detailed backend architecture, API surface planning, and security flow design.
