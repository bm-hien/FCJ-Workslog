---
title: "Week 4: Identity, Authorization, and System Security Direction"
date: 2026-01-26
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### 1. Objectives

* Master IAM and least-privilege thinking to prepare for secure backend operations.
* Understand how users, groups, roles, and policies should be organized in AWS.
* Evaluate technology directions that could support the backend architecture of the project.

### 2. Weekly Tasks Breakdown

| Day | Main Task | Details | Status |
|:---:|:---|:---|:---:|
| **Mon** | **IAM Structure** | - Studied how IAM Users, Groups, and Roles can be organized for a team environment.<br>- Related these concepts to backend resource access control. | Completed |
| **Tue** | **Least-Privilege Policies** | - Practiced drafting and reviewing policies with limited resource scope.<br>- Avoided broad access grants across AWS resources. | Completed |
| **Wed** | **MFA and Account Security** | - Applied MFA and secure account management practices.<br>- Reduced dependency on the root account in daily work. | Completed |
| **Thu** | **Technology Update** | - Attended the AWS re:Invent recap activity.<br>- Expanded my view of services that could support backend architecture. | Completed |
| **Fri** | **Architecture Relevance Review** | - Evaluated directions such as Cognito and newer data services for auth, data flow, and logging use cases.<br>- Summarized what could be relevant to the project. | Completed |

### 3. Outcomes

* Developed a clearer understanding of AWS resource access control at the user and role level.
* Built a stronger foundation for later decisions around authentication, authorization, and backend security.
* Reinforced a least-privilege mindset for every system component.

### 4. Issues & Solutions

* **Issue:** Fine-grained policy writing with ARNs was error-prone at first.
* **Solution:** Generated draft policies with support tools, then refined them manually to match actual resources.

### 5. Next Steps

* Move into serverless architecture and backend design with Lambda, API Gateway, and DynamoDB.
* Start connecting infrastructure knowledge with the actual product direction of the team.
