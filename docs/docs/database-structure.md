# NimbleShift – Database Structure

## 1. Overview

NimbleShift uses Bubble's built-in database to store business, employee, leave, shift, and planning information.

The database is organized around seven main data types.

## 2. Main Data Types

### İşletmeler
Stores business-level information and subscription-related data.

### Kullanıcılar
Stores application user information and role-related data.

### Personel
Stores employee records and their business association.

### İzinler
Stores employee leave requests and their approval status.

### Vardiyalar
Stores shift records, including planned shifts and draft suggestions.

### Kurallar
Stores rules used in shift planning.

### Personel İhtiyaçları
Stores staffing requirements used when creating shift suggestions.

## 3. Option Sets

The application currently uses the following Option Sets:

- Abonelik Paketi
- Görev Unvanı
- İzin Durumu
- İzin Kaydı
- İzin Türü
- Kullanıcı Rolü
- Müsaitlik
- Vardiya Durumu
- Çalışma Türü

## 4. Data Relationships

The application is designed to associate operational records with their relevant business.

Employee, leave, shift, rule, and staffing requirement records use business-related relationships to support business-level data separation.

## 5. Access Control

Bubble Privacy Rules and workflow conditions are used to restrict access to business data.

Users should only be able to access records permitted by their business association and application role.

## 6. Data Integrity

Workflow conditions are used to protect important operations, including shift approval, leave decisions, and employee management.

Detailed field definitions and relationship validation should be maintained as the Bubble database evolves.

## 7. Current Scope

This document describes the known high-level database structure. It does not claim that every field, relationship, or privacy rule has been independently verified.
