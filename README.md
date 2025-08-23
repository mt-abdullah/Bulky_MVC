# 📚 Bulky_MVC - Book Store Management System

A modern ASP.NET Core MVC application for managing book inventory, categories, and online store operations built with .NET 8.0.

## 🚀 Features

- **Book Management** - CRUD operations for books
- **Category Management** - Organize books by categories
- **Razor Pages** - Modern UI with Razor syntax
- **Entity Framework Core 9.0** - Data access with ORM
- **SQL Server Integration** - Robust database management
- **Responsive Design** - Mobile-friendly interface
- **Git Version Control** - Proper source control management

## 🛠️ Technology Stack

- **Framework**: .NET 8.0
- **Backend**: ASP.NET Core MVC
- **Frontend**: Razor Pages, HTML5, CSS3, JavaScript
- **Database**: SQL Server with Entity Framework Core 9.0.8
- **ORM**: Entity Framework Core
- **Tools**: Entity Framework Core Tools 9.0.8
- **Version Control**: Git & GitHub

## 📦 Project Structure

```
Bulky_MVC/
├── Controllers/
├── Models/
├── Views/
├── Data/
├── wwwroot/
├── Services/
├── Repository/
└── Bulky_MVC.csproj
```

## ⚙️ Prerequisites

- [.NET 8.0 SDK](https://dotnet.microsoft.com/download/dotnet/8.0)
- [Visual Studio 2022](https://visualstudio.microsoft.com/) (v17.8 or later) or [VS Code](https://code.visualstudio.com/)
- [SQL Server](https://www.microsoft.com/en-us/sql-server/sql-server-downloads) or SQL Server Express
- [Entity Framework Core Tools](https://docs.microsoft.com/ef/core/cli/)

## 🏃‍♂️ Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/mt-abdullah/Bulky_MVC.git
   cd Bulky_MVC
   ```

2. **Restore dependencies**
   ```bash
   dotnet restore
   ```

3. **Database setup**
   - Update connection string in `appsettings.json`
   - Create database migrations:
     ```bash
     dotnet ef migrations add InitialCreate
     ```
   - Apply migrations:
     ```bash
     dotnet ef database update
     ```

4. **Run the application**
   ```bash
   dotnet run
   ```
   or for development with hot reload:
   ```bash
   dotnet watch run
   ```

5. **Open in browser**
   Navigate to `https://localhost:7000` or `http://localhost:5000`

## 🔧 Configuration

Update `appsettings.json` with your database connection:

```json
{
  "ConnectionStrings": {
    "DefaultConnection": "Server=.;Database=Bulky;Trusted_Connection=True;TrustServerCertificate=True;"
  },
  "Logging": {
    "LogLevel": {
      "Default": "Information",
      "Microsoft.AspNetCore": "Warning"
    }
  }
}
```

## 🗃️ Entity Framework Commands

```bash
# Add new migration
dotnet ef migrations add MigrationName

# Update database
dotnet ef database update

# Remove last migration
dotnet ef migrations remove

# List migrations
dotnet ef migrations list
```

## 📋 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/Books` | Get all books |
| GET | `/Books/{id}` | Get book by ID |
| POST | `/Books` | Create new book |
| PUT | `/Books/{id}` | Update book |
| DELETE | `/Books/{id}` | Delete book |

## 🧪 Testing

Run the application:
```bash
dotnet run
```

Run with watch mode (auto-restart on changes):
```bash
dotnet watch run
```

## 📦 Dependencies

- Microsoft.EntityFrameworkCore (9.0.8)
- Microsoft.EntityFrameworkCore.SqlServer (9.0.8)
- Microsoft.EntityFrameworkCore.Tools (9.0.8)
- Microsoft.VisualStudio.Web.CodeGeneration.Design (9.0.0)

## 🤝 Contributing

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request
   
## 👨‍💻 Author

**Abdullah**  
- GitHub: [@mt-abdullah](https://github.com/mt-abdullah)
- Email: iammtabdullah@gmail.com

## 🤝 Acknowledgments

- ASP.NET Core 8.0 documentation
- Entity Framework Core 9.0 team
- Microsoft Learn resources
