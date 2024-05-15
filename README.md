# ASP.NET MVC CRUD Operations 🌐

Welcome to the **ASP.NET MVC CRUD Operations** project! This project demonstrates how to perform basic Create, Read, Update, and Delete (CRUD) operations on tables specified in SQL assignments. The tables used in this project are `t_Employee` and `t_Salary`.

## ✨ Features

- **Create**: Add new records to the database.
- **Read**: View details of existing records.
- **Update**: Modify existing records.
- **Delete**: Remove records from the database.

## 💻 Technologies Used

- **ASP.NET MVC**: Framework for building web applications.
- **C#**: Language used for server-side programming.
- **SQL Server**: Database management system.
- **Entity Framework**: ORM used for database operations.
- **HTML/CSS**: Frontend design and styling.
- **Bootstrap**: Frontend framework for responsive UI.

## 🛠️ Getting Started

To run this project locally, follow these steps:

1. **Clone the Repository**

   ```bash
     https://github.com/Mustafabharmal/Crud-Dotnet.git
   ```

2. **Set up Database**

   - Open SQL Server Management Studio.
   - Create the necessary database and tables (`t_Employee` and `t_Salary`) using the provided SQL scripts.

3. **Open Project in Visual Studio**

   - Launch Visual Studio and open the project.
   - Ensure all required dependencies for ASP.NET MVC are installed.

4. **Configure Connection String**

   - Update the database connection string in `Web.config` to match your SQL Server instance.

     ```xml
     <connectionStrings>
       <add name="DefaultConnection" connectionString="Data Source=YOUR_SERVER;Initial Catalog=AssignmentDB;Integrated Security=True" providerName="System.Data.SqlClient" />
     </connectionStrings>
     ```

5. **Build and Run**

   - Build the solution and start the application.
   - Access the application in your web browser (`http://localhost:{port}/Home/Index`).

## 📂 Project Structure

### Controllers

- **HomeController.cs**: Manages CRUD operations for the `t_Employee` table.
  - `Index()`: Lists all employees.
  - `Details(int id)`: Shows details of a specific employee.
  - `Create()`: Displays the create form.
  - `Create(t_Employee employee)`: Handles form submission to add a new employee.
  - `Edit(int id)`: Displays the edit form for a specific employee.
  - `Edit(int id, t_Employee employee)`: Handles form submission to update an employee.
  - `Delete(int id)`: Displays the delete confirmation for a specific employee.
  - `Delete(int id, t_Employee employee)`: Handles deletion of an employee.

- **SalaryController.cs**: Manages CRUD operations for the `t_Salary` table.
  - `Index()`: Lists all salary records.
  - `Details(int id)`: Shows details of a specific salary record.
  - `Create()`: Displays the create form.
  - `Create(t_Salary salary)`: Handles form submission to add a new salary record.
  - `Edit(int id)`: Displays the edit form for a specific salary record.
  - `Edit(int id, t_Salary salary)`: Handles form submission to update a salary record.
  - `Delete(int id)`: Displays the delete confirmation for a specific salary record.
  - `Delete(int id, FormCollection collection)`: Handles deletion of a salary record.

### Models

- **t_Employee**: Represents the employee entity with properties such as `EmployeeId`, `EmpName`, and `Age`.
- **t_Salary**: Represents the salary entity with properties such as `Id`, `EmpId`, `MonthName`, and `SALARY`.

### Views

- **Home Views**: Views for managing `t_Employee` records (Index, Create, Edit, Delete, Details).
- **Salary Views**: Views for managing `t_Salary` records (Index, Create, Edit, Delete, Details).

## 🤝 Contributing

Contributions to enhance this project are welcomed! Feel free to fork the repository and submit pull requests.

## 📝 License

This project is licensed under the [MIT License](LICENSE).

---
