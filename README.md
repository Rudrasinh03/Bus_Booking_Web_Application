**NAME:THAKOR RUDRASINH PRAGNESHSINH


CLASS/DIV: 5-D


EN.NO:202303103510355**

🚌 Bus Booking Web Application

A complete **Bus Ticket Booking System** built using **ASP.NET Core MVC (.NET 9)** and **SQLite (Entity Framework Core)**.
This project allows users to **search buses, book tickets, manage bookings**, and provides admin-level management of routes, buses, and schedules.

---

🚀 Features

🧑‍💻 Authentication & User Roles

* Secure **Login / Logout / Registration**
* Role-based access:

  * **Admin:** Manage routes, buses, and users
  * **User:** Search and book buses

🚌 Core Functionality

* Search buses by route, date, and time
* View bus details and availability
* Book and cancel tickets
* Generate and view booking confirmation

⚙️ Admin Features

* Add / Edit / Delete Buses
* Manage Routes and Schedules
* View all bookings and users

🎯 Additional Features

* SQLite local database (portable, file-based)
* Entity Framework Core (ORM)
* Razor Views for responsive UI
* Bootstrap & jQuery for front-end styling and interactivity

---

🧰 Technology Stack

| Layer        | Technology                         |
| ------------ | ---------------------------------- |
| **Frontend** | HTML5, CSS3, Bootstrap, jQuery     |
| **Backend**  | ASP.NET Core MVC (.NET 9)          |
| **Database** | SQLite (via Entity Framework Core) |
| **ORM**      | Entity Framework Core              |
| **IDE**      | Visual Studio 2022 or VS Code      |

---

📦 Prerequisites

Before running the project, ensure you have installed:

* [.NET 9 SDK](https://dotnet.microsoft.com/en-us/download)
* [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or VS Code
* Git (to clone the repository)

---

⚙️ Installation & Setup

1️⃣ Clone the Repository

```bash
git clone https://github.com/Rudrasinh03/Bus_Booking_Web_Application.git
cd Bus_Booking_Web_Application
```
2️⃣ Open the Project

* Open the solution in **Visual Studio 2022** or **VS Code**.

3️⃣ Check Database Connection

In your **`appsettings.json`**, ensure this connection string exists:

```json
"ConnectionStrings": {
  "DefaultConnection": "Data Source=busapp.db"
}
```

 4️⃣ Run the Application

```bash
dotnet run
```

 5️⃣ Access in Browser

Open your browser and go to:

```
https://localhost:5001
```



📂 Project Structure


BusBookingWebApp/
├── Controllers/         # MVC Controllers
├── Models/              # Data models (Bus, Booking, User, etc.)
├── Views/               # Razor Views (.cshtml files)
├── Data/                # Database context & migrations
├── Migrations/          # EF Core migration files
├── wwwroot/             # Static files (CSS, JS, images)
├── appsettings.json     # Configuration file
├── Program.cs           # Application entry point
└── busapp.db            # SQLite database file


For demo purposes, you may add default users via the database or EF seeding.

---

## 🧩 Key Models

| Model       | Description                                         |
| ----------- | --------------------------------------------------- |
| **Bus**     | Stores bus details such as name, type, and capacity |
| **Route**   | Defines source and destination locations            |
| **Booking** | Stores user booking details                         |
| **User**    | Represents registered users (Admin / Customer)      |
