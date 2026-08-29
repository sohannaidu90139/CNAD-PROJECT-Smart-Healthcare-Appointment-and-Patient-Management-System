# CNAD-PROJECT-Smart-Healthcare-Appointment-and-Patient-Management-System

Smart Healthcare Appointment and Patient Management System

A Smart Healthcare Appointment and Patient Management System designed to streamline patient management, doctor availability, appointment scheduling, and notifications through a modular SOA-based microservices architecture.

Academic Project: SOA Programming and Microservices – 24SDCS03
Academic Year: 2026–2027

📌 Overview

Healthcare appointment management can involve separate processes for patient registration, doctor availability, appointment booking, and appointment communication. This project proposes an integrated platform that brings these functions together through independent services.

The system focuses on:

👤 Patient management
👨‍⚕️ Doctor management
📅 Appointment scheduling
🕐 Doctor availability
🔔 Appointment notifications
🔐 Authentication
⚙️ SOA-based microservices
🎯 Objectives
Provide efficient appointment booking, rescheduling, and cancellation.
Maintain organized patient information and appointment history.
Manage doctor profiles, schedules, and availability.
Reduce appointment scheduling conflicts.
Automate appointment confirmations and reminders.
Develop a modular and scalable service-oriented architecture.
🏗️ Proposed Architecture
                    ┌─────────────────────┐
                    │   Patient / Doctor  │
                    │       / Admin       │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │    Web / Mobile     │
                    │      Client         │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │     API Gateway     │
                    └──────────┬──────────┘
                               │
             ┌─────────────────┼─────────────────┐
             │                 │                 │
             ▼                 ▼                 ▼
      ┌─────────────┐   ┌─────────────┐   ┌─────────────┐
      │ Auth        │   │ Patient     │   │ Doctor      │
      │ Service     │   │ Service     │   │ Service     │
      └─────────────┘   └─────────────┘   └─────────────┘
             │                 │                 │
             └─────────────────┼─────────────────┘
                               │
             ┌─────────────────┼──────────────────┐
             │                 │                  │
             ▼                 ▼                  ▼
      ┌─────────────┐   ┌─────────────┐   ┌─────────────┐
      │ Appointment │   │ Notification│   │ Medical     │
      │ Service     │   │ Service     │   │ Records     │
      └─────────────┘   └─────────────┘   └─────────────┘
                               │
                               ▼
                       ┌───────────────┐
                       │   Database    │
                       └───────────────┘

The architecture is proposed for this project and follows the project's SOA/microservices objective.

🔄 Appointment Workflow
Patient
   ↓
Appointment Request
   ↓
Check Doctor Availability
   ↓
Select Available Slot
   ↓
Schedule Appointment
   ↓
Confirmation
   ↓
Notification
🧩 Core Services
Service	Responsibility
Authentication Service	User authentication and access control
Patient Service	Patient profiles and information
Doctor Service	Doctor profiles and availability
Appointment Service	Booking, rescheduling and cancellation
Notification Service	Appointment confirmations and reminders
Medical Records Service	Patient medical information and history
⚙️ Proposed Technology Concepts
Microservices Architecture
REST APIs
API Gateway
Authentication
Service-to-Service Communication
Database-per-Service
Containerized Deployment

Technologies can be changed during implementation based on project requirements.

✨ Key Features
Patient Management
Patient registration
Patient profile management
Appointment history
Doctor Management
Doctor profiles
Availability management
Schedule management
Appointment Management
Book appointments
Reschedule appointments
Cancel appointments
Availability checking
Notifications
Appointment confirmation
Appointment reminders
Appointment updates
📂 Suggested Project Structure
smart-healthcare-system/
│
├── api-gateway/
├── auth-service/
├── patient-service/
├── doctor-service/
├── appointment-service/
├── notification-service/
├── medical-record-service/
│
├── frontend/
│
├── docs/
│   ├── architecture/
│   └── project-review/
│
├── docker-compose.yml
├── README.md
└── .gitignore
🚀 Project Development Plan
Phase	Work
W1–W2	Requirement & Domain Analysis
W3–W4	Database & Core Services
W5–W6	Patient & Doctor Services
W7–W8	Appointment & Scheduling
W9–W10	Service Integration
W11–W12	Testing & Validation
W13	Deployment
W14	Demonstration & Documentation
🎯 Expected Outcome

The project aims to provide a modular healthcare platform for efficient appointment scheduling and centralized patient management, with independent services that can be developed and maintained separately.

🔮 Future Scope
AI-based doctor/slot recommendation
Predictive appointment demand
Telemedicine integration
Wearable/IoT integration
Cloud deployment
Personalized healthcare services
👥 Team
Name	University ID
Team Member 1	XXXXX
Team Member 2	XXXXX
Team Member 3	XXXXX
Team Member 4	XXXXX

Guide: Dr. XXXXXXX
Department of Computer Science and Engineering
KLH CSE Bowrampet Campus

📚 Academic Context

This project is developed as part of SOA Programming and Microservices (24SDCS03) for the academic year 2026–2027. The proposed system emphasizes modular service decomposition and integration rather than treating the healthcare application as a single monolithic system. The project-review template likewise emphasizes SOA/microservices-oriented project structure and feasibility planning.

⭐ Project Focus

Smart Appointment Scheduling + Patient Management + Doctor Availability + Automated Notifications + SOA Microservices
