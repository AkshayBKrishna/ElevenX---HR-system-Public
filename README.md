<div align="center">

# ElevenX HR Platform

### Built for Humans. Runs like a Machine.

*Spreadsheets break at 50 people. ElevenX is built for what comes after — a complete HR platform that grows with your company, without the workarounds.*

[![Live Platform](https://img.shields.io/badge/Live%20Platform-elevenx--11x.web.app-teal?style=for-the-badge)](https://elevenx-11x.web.app)
[![Status](https://img.shields.io/badge/Status-Live%20%26%20Deployed-brightgreen?style=for-the-badge)]()
[![Client](https://img.shields.io/badge/Paying%20Client-Uday%20Engineering%20Works-blue?style=for-the-badge)]()

</div>

---

## What is ElevenX?

ElevenX HR is a fully deployed, cloud-native, multi-tenant HR Management SaaS platform built from scratch in under 90 days. It is not a prototype or a mockup — it is a functioning product with real companies onboarded and a paying client confirmed before launch day.

The platform was built as part of HRMM504 at Mittal School of Business, Lovely Professional University. CA1 identified the problems. CA2 built the solution.

---

## The Problem We Solved

Our research across growing Indian organisations found the same five problems everywhere:

| Pain Point | What Was Happening |
|---|---|
| Attendance | Tracked manually in Google Sheets every morning |
| Leave Requests | Sent informally over WhatsApp with no audit trail |
| Onboarding | New employees took 2–3 days to get set up manually |
| Self Service | Employees had to call HR for every routine query |
| Monthly Reports | Compiled by hand — 8 to 10 hours every month |

ElevenX replaces all five with working, deployed features.

---

## Live Platform

🌐 **https://elevenx-11x.web.app**

The platform is live and accessible. Five companies are currently onboarded on the SuperAdmin console.

---

## Four Portals, One Platform

### 🔷 SuperAdmin Portal
For the ElevenX team. Onboard and manage all companies, monitor platform-wide activity, manage support inbox, control which companies are active or suspended.

### 🔷 HR Admin Portal
The core of the platform. Add employees individually or via Excel bulk upload. Manage leave, track attendance, run onboarding, manage documents, view analytics, access audit logs.

### 🔷 Manager Portal
Team-level visibility. View team attendance, approve or reject leave requests, raise helpdesk tickets. Managers see only their own team — enforced at the database level.

### 🔷 Employee Portal
Full self-service. Check in and check out with one button. Apply for leave, view balance in real time, upload documents, raise support tickets. No HR involvement needed for routine queries.

---

## Features

- ✅ Multi-tenant architecture — complete data isolation per company
- ✅ Five user roles — SuperAdmin, Company Admin, HR Staff, Manager, Employee
- ✅ Real-time attendance check-in and check-out with monthly history
- ✅ Leave request and approval workflow with live balance tracking
- ✅ Automated employee onboarding via email invite — live in under 10 minutes
- ✅ Bulk employee upload via Excel with duplicate detection
- ✅ Analytics dashboard with real-time HR metrics
- ✅ Helpdesk and ticket management across all roles
- ✅ Document upload and management
- ✅ Audit log for all HR actions
- ✅ 30-minute inactivity auto-logout with 5-minute warning
- ✅ Forced password reset on first login
- ✅ Scheduled auto-wipe of expired trial company data
- ✅ DPDP 2023 compliant — data stored in asia-south1 Mumbai region

---

## Tech Stack

| Layer | Technology | Why |
|---|---|---|
| Frontend | React 18 + Vite | Component-based UI, fast HMR, industry standard |
| Database | Firebase Firestore (asia-south1) | Real-time, zero infrastructure, Mumbai region |
| Authentication | Firebase Auth | Session management, bcrypt hashing, token refresh |
| Backend | Node.js 20 Cloud Functions | Serverless, auto-scales, zero cold start |
| Email | Resend API | High deliverability transactional email |
| Secrets | Google Cloud Secret Manager | No .env files, keys never exposed |
| Hosting | Firebase Hosting + CDN | Global CDN, auto SSL, 99.95% uptime SLA |

---

## Cloud Functions

| Function | Purpose |
|---|---|
| createCompanyAdmin | Creates new company and first admin atomically |
| createEmployee | Creates employee and sends onboarding email |
| bulkCreateEmployees | Parses Excel, creates multiple employees, skips duplicates |
| sendOnboardingInvite | Sends Resend email with onboarding link |
| completeOnboarding | Public endpoint for employee self-onboarding |
| forceResetPassword | Admin-initiated password reset |
| toggleCompanyStatus | Enable or disable a company account |
| wipeCompanyData | Hard-deletes all data for a company instantly |
| deleteCompany | Removes company from master registry |
| scheduledWipeExpiredCompanies | Daily cron — auto-wipes expired trial companies |

---

## Scale
```
10,250+    Lines of Code
4          User Portals
28+        Screens
10         Deployed Cloud Functions
12         Firestore Collections
5          Companies Onboarded
1          Paying Client
90 days    Build Time
```

---

## Screenshots

### Landing Page
![Landing Page](screenshots/landing.png)

### SuperAdmin Dashboard
![SuperAdmin Dashboard](screenshots/superadmin.png)

### HR Portal
![HR Portal](screenshots/hr.png)

### Manager Portal
![Manager Portal](screenshots/manager.png)

### Employee Portal
![Employee Portal](screenshots/employee.png)

---

## First Client

**M/s Uday Engineering Works, Mumbai**
Industrial infrastructure company — EOT crane erection, structural fabrication, rail infrastructure.
50–100 employees across field and office roles.

3-month pilot confirmed. Rs. 15,000 received via UPI on 9 March 2026.

---

## Roadmap

| Quarter | Milestone |
|---|---|
| Q2 2026 | In-app notifications, mobile responsive improvements |
| Q3 2026 | React Native mobile app — iOS and Android |
| Q4 2026 | Payroll module with salary slips |
| Q1 2027 | SSO, Google Workspace integration |
| Q2 2027 | AI attrition prediction, HR analytics layer |

---

## Built By

| Name | Registration No. |
|---|---|
| Akshay B Krishna | 12501922 |
| Shamna Shari | 12502772 |
| Arya P S | 12502425 |
| Muhammad Shinas K P | 12523581 |

**Mittal School of Business, Lovely Professional University**
HRMM504 — Human Resource Information System — 2026
Academic Supervisor: Dr. Priyanka Chhibber

---

> Source code is maintained in a private repository.
> This repository contains the project overview only.

---

<div align="center">

*Built for Humans. Runs like a Machine.*

</div># ElevenX---HR-system-Public
