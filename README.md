# Kit

# ASP.NET Core MVC Product Search Application

This is a simple ASP.NET Core MVC application that allows users to search for products based on various criteria.

## Prerequisites

- [.NET SDK](https://dotnet.microsoft.com/download) installed
- [Visual Studio](https://visualstudio.microsoft.com/) or [Visual Studio Code](https://code.visualstudio.com/) for development

## Getting Started

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/your-repository.git
    cd your-repository
    ```

2. Open the project in Visual Studio or Visual Studio Code.

3. Configure the Database Connection:

    - Open `AppDbContext.cs` and replace `"your_actual_connection_string"` with your actual database connection string in the `OnConfiguring` method.

4. Apply Database Migrations:

    - Open a terminal and navigate to the project directory.
    - Run the following commands:

        ```bash
        dotnet ef migrations add InitialCreate
        dotnet ef database update
        ```

5. Run the Application:

    - Press F5 or use the command `dotnet run` to start the application.

6. Open a web browser and navigate to `https://localhost:5001` to view the application.

## Features

- Product Search: Users can search for products based on various criteria such as Product Name, Size, Price, Manufacturing Date, and Category.
- Flexible Search Criteria: Users can define search criteria using any combination of fields.
- Conjunction Options: Users can specify the conjunction (AND, OR) between two or more search conditions.
- Clear/Reset: Option to clear/reset the search criteria.
- Search Results: Display search results in a table/grid.

## Technologies Used

- ASP.NET Core MVC
- Entity Framework Core
- SQL Server (or your preferred database)

## Folder Structure

- `Controllers`: Contains MVC controller classes.
- `Models`: Contains data models.
- `Views`: Contains Razor views.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
