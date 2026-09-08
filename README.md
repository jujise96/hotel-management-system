# 🏨 Hotel Management System

Desktop application for internal hotel management.

## 📋 Description

The **Hotel Management System** is a desktop application designed for hotel staff or small chains. It replaces spreadsheets and notebooks for booking control, providing a centralized and validated solution.

Unlike an online booking engine, this application **has no public face**. All reservations are entered by an employee (by phone or email), ensuring that availability management and invoicing are accurate and always up to date.

## ✨ Key Features

- **Hotels & Rooms Management**: Create, edit, and deactivate hotels, room types, and individual rooms with their bed and extra bed counts.
- **Booking Engine**: Create and modify reservations with automatic availability validation (prevents overbooking). Supports multiple rooms per reservation with independent check‑in/check‑out dates.
- **Check‑in / Check‑out**: Register arrivals and departures, with automatic room status updates (Occupied, Available, Cleaning).
- **Guest Management**: Guest profile with search by name, ID, or reservation number. Register companions per booking line.
- **Invoicing**: Generate invoices from a reservation with a breakdown by nights and concepts, exportable to PDF.
- **Excel Export**: Export reservations, guests, and occupancy reports.
- **Users & Roles**: Access control with "Reception" and "Administrator" roles.
- **Suggestions & Incidents**: Suggestion box for staff and an incident tracking system (cleaning, maintenance, complaints).

## 🛠️ Technologies

- **Language**: C# (.NET)
- **UI Framework**: WPF (Windows Presentation Foundation)
- **Architectural Pattern**: MVVM (Model‑View‑ViewModel)
- **Data Access**: Entity Framework Core
- **Database**: SQLite (local)
- **Additional Libraries**:
  - ClosedXML (Excel export)
  - (Pending) PDF generation library (e.g., iTextSharp or QuestPDF)

## 🏗️ Project Architecture

The solution follows a layered architecture with clear separation of concerns:

- **Hotel.Core**: Domain entities and business logic (availability validation, business rules). Independent of UI and data access.
- **Hotel.Data**: Data access using Entity Framework Core and SQLite. Implements the Repository pattern.
- **Hotel.App**: WPF user interface with MVVM (Views and ViewModels). Depends on Core and Data via dependency injection.
- **Hotel.Tests**: Unit tests (xUnit) for the business logic in Hotel.Core.

## 📅 Planning & Methodology

The project follows the **SCRUM** agile methodology, adapted for a single developer, with two‑week sprints. The planning is divided into the following milestones, starting on **September 8, 2026**:

| Milestone | Description | Dates |
| :-------- | :---------- | :---- |
| **M0 – Preparation** | Environment setup and technology review | 08 – 13 Sep 2026 |
| **M1 – Core & Data Model** | Solution creation, domain entities, and Core layer | 14 Sep – 04 Oct 2026 |
| **M2 – Users & Roles Management** | User creation, role assignment, authentication, and basic login UI | 05 – 25 Oct 2026 |
| **M3 – Hotels & Rooms CRUD** | Screens for hotels, room types, and rooms (with role‑based access) | 26 Oct – 15 Nov 2026 |
| **M4 – Booking Engine & Calendar** | Availability validation, booking creation/modification, occupancy calendar view | 16 Nov – 06 Dec 2026 |
| **M5 – Guests, Check‑in/out** | Guest and companion management, check‑in/out actions | 07 – 27 Dec 2026 |
| **M6 – Invoicing & Excel Export** | PDF invoice generation and Excel data export | 28 Dec 2026 – 17 Jan 2027 |
| **M7 – Polish & Unit Testing** | Unit tests (xUnit), bug fixing, and UI polish | 18 Jan – 07 Feb 2027 |
| **M8 – Integration & Packaging** | Integration tests, deployment package, and final review | 08 – 21 Feb 2027 |
| **M9 – Finalisation** | Final documentation, portfolio delivery, and project closure | 22 Feb – 07 Mar 2027 |

## 🚀 Getting Started

### Prerequisites

- [Visual Studio 2026](https://visualstudio.microsoft.com/) (or later; Community edition is sufficient)
- [.NET SDK 6.0](https://dotnet.microsoft.com/download) or later
- Basic knowledge of C# and WPF (for contributions)

### Clone the repository

```bash
git clone https://github.com/your-username/HotelManagementSystem.git
cd HotelManagementSystem
```


## 👥 Team

- **Juan Jiménez Serrano** – [@jujise96](https://github.com/jujise96)
- **Ismael Da Palma Fernandez** – [@Conardium](https://github.com/Conardium)
- **Victoria C. García Serrano** – [@Vicky5-5](https://github.com/Vicky5-5)

---
