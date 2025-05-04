🌟 Project Overview
A comprehensive management system for Quran education centers, 
handling student attendance, teacher assignments, group management, 
and progress tracking. Designed to streamline operations for Islamic education institutions.

Key Objectives:

Digitalize attendance tracking

Manage teacher-group assignments

Track student progress

Generate reports for administration

Provide mobile-friendly interfaces

🚀 Features
Frontend
📱 Responsive dashboard for admins, teachers, and students

📅 Interactive attendance calendar

📊 Real-time analytics and reporting

👥 Student/Teacher profile management


Backend
🔐 JWT Authentication & Role-Based Access Control

📝 Attendance recording with validation

🔄 CRUD operations for all entities

📈 Advanced reporting endpoints

🚦 Request validation and error handling

📄 PDF report generation


🛠 Tech Stack
Frontend
Technology	Purpose
Angular 17	Frontend framework
NgRx	State management
Tailwind CSS	Styling
PrimeNG	UI Component library
Chart.js	Data visualization
Date-fns	Date handling
Backend
Technology	Purpose
.NET 7	Backend framework
Entity Framework Core	ORM
SQL Server	Database
MediatR	CQRS pattern
FluentValidation	Request validation

🏛 Architecture
High-Level Design
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│   Angular       │    │   ASP.NET       │    │   SQL Server    │
│   Frontend      │ ◀─▶│   Web API       │ ◀─▶│   Database      │
└─────────────────┘    └─────────────────┘    └─────────────────┘

Backend Architecture (Clean Architecture)
Presentation Layer (API)
│
Application Layer (CQRS with MediatR)
│
Domain Layer (Core Business Logic)
│
Infrastructure Layer (Persistence, External Services)
📚 API Documentation
Full API documentation available via Swagger UI at /swagger when running the project.

View API Docs

Key Endpoints:

POST /api/attendance - Record attendance

GET /api/groups/{id}/attendance - Get group attendance

POST /api/groups/{id}/teachers - Assign teacher to group

GET /api/reports/attendance - Generate attendance reports


