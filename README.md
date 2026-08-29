# 🏥 Smart Healthcare Appointment & Patient Management System

> A modular **SOA-based microservices platform** for managing patients, doctors, appointments, availability, and notifications.

<p align="center">

![Project Status](https://img.shields.io/badge/Status-In%20Development-blue)
![Academic Year](https://img.shields.io/badge/Academic%20Year-2026--2027-green)
![Course](https://img.shields.io/badge/Course-24SDCS03-orange)
![Architecture](https://img.shields.io/badge/Architecture-SOA%20%7C%20Microservices-purple)

</p>

---

## 📌 Overview

The **Smart Healthcare Appointment & Patient Management System** is a proposed healthcare platform designed to simplify appointment scheduling and patient management.

The system brings together:

- Patient management
- Doctor management
- Doctor availability
- Appointment scheduling
- Appointment notifications
- Authentication
- Independent microservices

The project follows a **Service-Oriented Architecture (SOA)** approach, allowing healthcare functions to be separated into independent services.

---

## 🎯 Objectives

| Objective | Description |
|---|---|
| 📅 **Appointment Management** | Book, reschedule, and cancel appointments |
| 👤 **Patient Management** | Maintain patient profiles and appointment history |
| 👨‍⚕️ **Doctor Management** | Manage doctor profiles and availability |
| 🕐 **Smart Scheduling** | Allocate suitable appointment slots |
| 🔔 **Notifications** | Provide appointment confirmations and reminders |
| ⚙️ **SOA Integration** | Separate major functions into independent services |

---

## ✨ Key Features

### 👤 Patient Management
- Patient registration
- Patient profile management
- Appointment history
- Patient information management

### 👨‍⚕️ Doctor Management
- Doctor profiles
- Availability management
- Schedule management

### 📅 Appointment Management
- Appointment booking
- Appointment rescheduling
- Appointment cancellation
- Doctor availability checking

### 🔔 Notification Management
- Appointment confirmation
- Appointment reminders
- Appointment updates

### 🔐 Authentication
- User authentication
- Role-based access
- Secure service access

---

# 🏗️ System Architecture

The proposed system follows a **layered SOA/microservices architecture**.

Workflow

Patient → Appointment Request → Doctor Availability → Appointment Scheduling → Confirmation → Notification

🧩 Microservices
Service	Responsibility
Authentication Service	Authentication and access control
Patient Service	Patient profiles and information
Doctor Service	Doctor profiles and availability
Appointment Service	Booking, rescheduling and cancellation
Notification Service	Appointment confirmations and reminders
Medical Records Service	Patient medical information and history
⚙️ Proposed Technology Architecture

The project is designed around the following technical concepts:

Client
   │
   ▼
API Gateway
   │
   ├── Authentication Service
   ├── Patient Service
   ├── Doctor Service
   ├── Appointment Service
   ├── Notification Service
   └── Medical Records Service
           │
           ▼
     Database per Service
Core Concepts
REST APIs
Microservices
API Gateway
Authentication
Service-to-Service Communication
Database-per-Service
Containerized Deployment

Technologies may be adjusted during implementation according to project requirements.

📂 Project Structure
smart-healthcare-appointment/
│
├── api-gateway/
│
├── auth-service/
│
├── patient-service/
│
├── doctor-service/
│
├── appointment-service/
│
├── notification-service/
│
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
