# Intelligent Security Analytics and Risk Assessment Platform

An AI-powered enterprise security analytics platform that streamlines security assessment, deterministic risk analysis, AI-assisted documentation, and report generation for enterprise applications.

> **Built using React, FastAPI, Gemini AI, Pandas, JWT Authentication, and SQLite**

---

## Overview

Enterprise security assessments often generate thousands of security observations across multiple departments, applications, and review activities. Managing these observations manually using spreadsheets makes it difficult to perform consistent analytics, identify risk trends, generate reports, and derive meaningful insights.

The Intelligent Security Analytics and Risk Assessment Platform addresses this challenge by providing a centralized web-based platform that transforms structured security assessment data into actionable enterprise analytics.

The platform combines deterministic analytics with AI-assisted documentation to help security analysts monitor application security posture, assess organizational risk, visualize key performance indicators, and automatically generate security recommendations using Google's Gemini AI.

This project was developed as a B.Tech Major Project in Artificial Intelligence & Data Science.

---

## Dashboard Preview

> Replace these screenshots after uploading them to the repository.

### Dashboard

![Dashboard](screenshots/dashboard.png)

### AI Analysis

![AI Module](screenshots/ai-module.png)

---

# Key Features

- Enterprise Security Dashboard
- Application-wise Security Analytics
- Department-wise Analytics
- Enterprise-wide Security Metrics
- Deterministic Risk Assessment
- AI-assisted Security Analysis using Gemini AI
- JWT-based Secure Authentication
- User Login & Registration
- Interactive Charts & Visualizations
- Search and Filter Security Observations
- PDF Report Generation
- DOCX Report Generation
- Structured Observation Repository
- REST API Architecture

---

# Project Architecture

The platform follows a modular client-server architecture.

```
React Frontend
       │
       ▼
REST API Layer
       │
       ▼
FastAPI Backend
       │
 ┌───────────────┐
 │ Analytics     │
 │ AI Engine     │
 │ Authentication│
 └───────────────┘
       │
       ▼
Dataset Management Layer
       │
       ▼
Observation Repository
       │
       ▼
Enterprise Analytics & AI Repository
```

---

## Methodology

The overall workflow of the platform consists of four major stages.

### 1. Security Assessment

Security observations are collected during enterprise application reviews including:

- IT General Controls (ITGC)
- Database Review
- Digital Forensic Readiness Assessment (DFRA)
- Secure Network Architecture (SNA)
- Data Flow Diagram Review (DFD)

---

### 2. Data Engineering

The collected observations are converted into a standardized repository.

The Dataset Management Layer performs:

- Data Loading
- Data Cleaning
- Normalization
- Attribute Mapping
- Filtering
- Grouping
- Aggregation

---

### 3. Analytics Engine

The Analytics Engine computes:

- Observation Statistics
- Severity Distribution
- Department Analytics
- Application Analytics
- Enterprise Analytics
- Deterministic Risk Scores
- Dashboard KPIs

---

### 4. AI Analysis

When a user requests AI analysis:

- Observation context is retrieved.
- Associated control information is collected.
- Risk information is retrieved.
- Recommendations are prepared.
- A structured prompt is generated.
- Gemini API generates detailed enterprise security recommendations.

---

# Technology Stack

| Layer | Technology |
|--------|------------|
| Frontend | React + Vite |
| Backend | FastAPI |
| Programming Language | Python |
| Analytics | Pandas |
| AI | Google Gemini API |
| Authentication | JWT |
| Database | SQLite |
| Charts | Recharts |
| Document Generation | ReportLab, python-docx |

---

# Folder Structure

```
intelligent-security-analytics/

├── backend/
├── frontend/
├── dataset/
├── ml/
├── screenshots/
├── docs/
├── README.md
├── requirements.txt
└── LICENSE
```

---

# Installation

## Clone Repository

```bash
git clone https://github.com/<your-github-username>/intelligent-security-analytics.git

cd intelligent-security-analytics
```

---

## Backend

```bash
cd backend

python -m venv venv

source venv/bin/activate

# Windows
venv\Scripts\activate

pip install -r requirements.txt

uvicorn app.main:app --reload
```

---

## Frontend

```bash
cd frontend

npm install

npm run dev
```

---

# REST API Overview

| Method | Endpoint | Description |
|---------|----------|-------------|
| POST | /login | User Login |
| POST | /register | User Registration |
| GET | /dashboard | Dashboard Analytics |
| GET | /applications | Application Analytics |
| GET | /departments | Department Analytics |
| POST | /generate | AI Security Analysis |
| GET | /reports | Report Generation |

---

# Project Modules

### Authentication Module

- JWT Authentication
- Secure Login
- Protected Routes

---

### Analytics Module

- Enterprise Dashboard
- Risk Analytics
- Severity Analytics
- KPI Generation

---

### AI Module

- Observation Retrieval
- Prompt Engineering
- Gemini Integration
- AI Recommendation Generation

---

### Reporting Module

- PDF Reports
- DOCX Reports
- Enterprise Summary Reports

---

# Future Enhancements

Future versions of this platform may include:

- Role-Based Access Control (RBAC)
- PostgreSQL Database
- Docker Deployment
- Kubernetes Support
- Real-time Monitoring
- Vector Database Integration
- Retrieval-Augmented Generation (RAG)
- Multi-LLM Support
- Predictive Risk Analytics
- Automated Security Compliance Monitoring

---

# Author

**Sandipan Choudhury**

B.Tech – Artificial Intelligence & Data Science

Sikkim Manipal Institute of Technology

GitHub: https://github.com/Sandipan12choudhury

---

# License

This project is licensed under the MIT License.

---

## Acknowledgements

This project was developed as part of the Bachelor of Technology (Artificial Intelligence & Data Science) Major Project.

The platform demonstrates the application of enterprise security analytics, deterministic risk assessment, and generative AI to improve cybersecurity assessment workflows and decision support.
