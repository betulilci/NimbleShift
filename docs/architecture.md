# NimbleShift – System Architecture

## 1. Overview

NimbleShift is a SaaS-based workforce and shift management application developed using Bubble.

The application helps businesses manage employees, leave requests, staffing requirements, and shift planning through a centralized platform.

## 2. Technology Stack

- Application Platform: Bubble
- Database: Bubble Database
- Business Logic: Bubble Workflows
- Access Control: Bubble Privacy Rules
- User Authentication: Bubble User Authentication

## 3. Main Data Types

The application currently uses the following data types:

- İşletmeler
- Kullanıcılar
- Personel
- İzinler
- Vardiyalar
- Kurallar
- Personel İhtiyaçları

## 4. User Roles

- Yönetici
- Planlayıcı
- Personel

Access is designed around user roles and business ownership.

## 5. Main Application Modules

- Business Management
- User Management
- Employee Management
- Leave Management
- Shift Management
- Smart Shift Suggestions
- Subscription Management

## 6. Smart Planning Flow

1. The manager defines staffing requirements.
2. The system evaluates available employees and relevant constraints.
3. Eligible employees are selected for shift suggestions.
4. Suggestions are stored as drafts.
5. The manager can regenerate unapproved drafts.
6. Approved suggestions are converted into actual shifts.

## 7. Security

The application uses Bubble Privacy Rules and workflow-level checks to restrict access to business data.

Security and production readiness require further validation before public launch.
