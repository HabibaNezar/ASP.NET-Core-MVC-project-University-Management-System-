# 🎓 University Management System

> A full-featured academic platform built from scratch with **.NET 8** and **ASP.NET Core MVC** — covering the complete web development lifecycle from database design to production deployment.

---

## 📌 Overview

The **University Management System** is a comprehensive web application designed to streamline core university operations — from student enrollment and course registration to grade tracking and department management.

Built entirely from scratch, the project demonstrates end-to-end ownership of the full development lifecycle: requirements analysis, database schema design, backend architecture, UI development, and deployment. It served as a true hands-on experience across real-world .NET 8 patterns and practices.

---

## ✨ Features

| Module | Description |
|---|---|
| 👨‍🎓 **Student Management** | Enrollment, profiles, academic history, and status tracking |
| 📚 **Course Management** | Course catalog, prerequisites, capacity, and scheduling |
| 🧑‍🏫 **Instructor Portal** | Manage courses taught, student rosters, and grade submission |
| 📊 **Grade & GPA Tracking** | Automated GPA calculation, transcript generation, and reports |
| 🏛️ **Department Management** | Departments, faculties, and organizational hierarchy |
| 🔐 **Role-Based Auth** | Admin, Instructor, and Student roles with scoped access via ASP.NET Identity |

---

## 🛠️ Tech Stack

| Layer | Technology | Purpose |
|---|---|---|
| **Backend** | .NET 8 / ASP.NET Core MVC | Web framework, routing, controllers |
| **ORM** | Entity Framework Core | Data modeling, migrations, LINQ queries |
| **Database** | SQL Server | Relational data storage |
| **Authentication** | ASP.NET Core Identity | Auth, roles, claims, password hashing |
| **Frontend** | Razor Views + Bootstrap 5 | Server-side rendering, responsive UI |
| **Architecture** | Repository + Service Layer | Separation of concerns, testability |

---

## 📁 Project Structure

```
UniversityManagementSystem/
│
├── Controllers/          # MVC controllers per domain (Students, Courses, Grades…)
├── Models/               # Domain entities and EF Core data models
├── ViewModels/           # Strongly-typed view models per action
├── Views/                # Razor templates, layouts, and partials
├── Services/             # Business logic layer (GPA calculator, enrollment rules…)
├── Repositories/         # Data access abstractions over EF Core
├── Data/                 # DbContext, migrations, and seed data
├── wwwroot/              # Static assets — CSS, JS, images
├── appsettings.json      # Configuration (connection strings, app settings)
└── Program.cs            # App entry point and DI configuration
```

---

## 🚀 Getting Started

### Prerequisites

- [.NET 8 SDK](https://dotnet.microsoft.com/download/dotnet/8.0)
- [SQL Server](https://www.microsoft.com/en-us/sql-server/sql-server-downloads) (or SQL Server Express)
- [Visual Studio 2022](https://visualstudio.microsoft.com/) or [VS Code](https://code.visualstudio.com/)

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/your-username/UniversityManagementSystem.git
cd UniversityManagementSystem

# 2. Configure your connection string in appsettings.json
#    "DefaultConnection": "Server=.;Database=UniversityDB;Trusted_Connection=True;TrustServerCertificate=True;"

# 3. Apply EF Core migrations and seed the database
dotnet ef database update

# 4. Run the application
dotnet run
```

Then navigate to `https://localhost:5001` in your browser.

---

## 🔑 Default Credentials

> These accounts are seeded automatically on first run.

| Role | Email | Password |
|---|---|---|
| Admin | `admin@university.edu` | `Admin@123` |
| Instructor | `instructor@university.edu` | `Inst@123` |
| Student | `student@university.edu` | `Student@123` |

---

## 📸 Screenshots

> _Coming soon — add screenshots of the dashboard, student list, course registration, and grade report pages here._

---

## 🗺️ Roadmap

- [ ] REST API layer with JWT authentication
- [ ] Email notifications for enrollment confirmation
- [ ] PDF transcript export
- [ ] Student attendance tracking module
- [ ] Dark mode support

---

## 💡 What I Learned

This project was a genuine deep-dive into the full development lifecycle. Key takeaways:

- Designing normalized relational schemas for complex academic data with multiple many-to-many relationships
- Implementing role-based authorization with ASP.NET Core Identity and claims-based policies
- Applying the **Repository** and **Service layer** patterns for a clean separation of concerns
- Managing EF Core migrations safely on an evolving, production-like schema
- Building a responsive multi-role UI with Razor Views and Bootstrap 5
- Structuring a maintainable MVC solution from the ground up with no boilerplate shortcuts

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to open a pull request or file an issue.

1. Fork the repository
2. Create your feature branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m 'Add your feature'`
4. Push to the branch: `git push origin feature/your-feature`
5. Open a Pull Request

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

<div align="center">
  Built with ❤️ using .NET 8 &nbsp;|&nbsp; ASP.NET Core MVC &nbsp;|&nbsp; Entity Framework Core
</div>
