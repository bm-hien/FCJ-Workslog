---
title: "Week 9: GuardScript — AWS Migration & Comprehensive UI Improvements"
date: 2026-03-16
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### 1. Objectives

* **AWS Migration:** Team migrates GuardScript from local prototype to AWS.
* **Infrastructure (Team):** Set up AWS services (Lambda, DynamoDB, S3, CloudFront).
* **Comprehensive UI Improvements:** Upgrade visual design, fix theme system, and complete missing frontend features.

### 2. Weekly Tasks Breakdown

| Day | Main Task | Details | Status |
|:---:|:---|:---|:---:|
| **Mon** | **Migration Planning** | - Reviewed prototype, identified AWS services needed.<br>- Distributed migration tasks among team members. | Completed |
| **Tue** | **Infrastructure (Team) & UI** | - Team deployed AWS infrastructure (Lambda, S3, CloudFront, DynamoDB).<br>- Enhanced overall UI: spacing, colors, logos, shield icons.<br>- Fixed light theme — multiple components displayed incorrectly in light mode. | Completed |
| **Wed** | **Workspace & License** | - Added toggle option for workspace.<br>- Fixed license key status update and workspace creation flow.<br>- Fixed execution summary display. | Completed |
| **Thu** | **Auth Pages & Landing** | - Fixed login/register page layouts for better responsive behavior.<br>- Added blur effect to landing page. | Completed |
| **Fri** | **Sidebar Fix & PR Review** | - Fixed toggle sidebar in workspace.<br>- Reviewed and merged PR#14 → PR#21 (enhance_UI, License_status, workspace_Overview, login_register). | Completed |

### 3. Key Results

#### Infrastructure (Team Effort):
* Deployed AWS services: Lambda, S3, CloudFront, DynamoDB.
* Migrated data from SQLite to DynamoDB.

#### Frontend (Personal Contribution):
* UI upgrade: spacing, typography, color palette, new logos.
* Finalized dark/light theme toggle.
* Fixed workspace toggle, license status, execution summary, auth page layouts.
* Added blur effect to landing page.
* Merged 8 PRs (PR#14 → PR#21).

### 4. Issues & Solutions
* **Issue:** Light theme caused display issues since components were initially designed only for dark theme.
* **Solution:** Audited all CSS, replaced hardcoded colors with CSS custom properties.

### 5. Next Steps
* Conduct end-to-end integration testing.
* Complete the system architecture diagram.
* Prepare documentation and worklog reports.
