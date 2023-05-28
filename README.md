# PROG7311-POE-PART2

Introduction
The MPV Farm Management Web Application is a comprehensive system developed to streamline the interaction between farmers and employees with farm-related data. Built on the robust and scalable ASP.NET Core framework, the application incorporates Razor Pages to deliver a seamless and intuitive user interface. The application leverages Azure SQL Database, providing reliable, cloud-based data storage and management.
Core Components and Functionality
The application is organized into the following pages, each serving a distinct role:
Index Page
Serving as the primary entry point for the application, the Index Page is primarily responsible for user authentication. It prompts users to enter their username and password while also selecting their respective roles – "Employee" or "Farmer". On successful authentication, users are redirected to their corresponding landing page – Employee or Farmer Menu Page.
Menu Page
The Menu Page is an employee-centric page providing a robust navigation bar and an advanced product search form. The latter empowers employees to search for products based on a variety of parameters, the results of which are dynamically populated in a user-friendly table.

Registration Page
The Registration Page, as its name suggests, caters to the creation of new user accounts. Here, users are expected to provide their desired username, password, and select their role, either "Employee" or "Farmer". The form validates the provided inputs and, if satisfactory, creates a new account in the database.
Database Management and Usage
At the heart of the application is the Azure SQL Server database, diligently managing and storing user information and other pertinent data. Interactions with the database are facilitated using the Entity Framework Core, with the connection string for the database sourced from the `appsettings.json` file. A central component of the data management functionality is the dBContext `ST10153108_Selton_PROG7311_POE_PART2Context`, which handles all operations related to the database.
 
Setup and Usage
To set up and run the MPV Farm Management Web Application:
1.	Ensure the .NET Core SDK is installed on your system.
2.	Clone the application repository to your local machine.
3.	Open a terminal and navigate to the application's directory.
4.	Execute `dotnet restore` to restore the necessary NuGet packages.
5.	Run `dotnet run` to initiate the application.
6.	Open a web browser and navigate to `localhost:5000` (or the port specified by your application) to access the web application.
To test the application, use the following login credentials:
-	Username: Selton
o	Password: 1234
o	Role: Employee
-	Username: Jose
o	Password: 1234
o	Role: Farmer
-	Username: Sinatra
o	Password: 1234
o	Role: Farmer
Upon successful login, users are redirected to their designated pages based on their roles. The navigation bar at the top allows easy movement between the different pages.
Future Scope and Notes
This application, while currently catering to fundamental functionalities, is designed as a steppingstone for a larger, more comprehensive farm management system. The present features constitute the base model and will need enhancements, additional security measures, and further robust functionalities to meet production-grade requirements. It's worth noting that the application is part of a programming assessment and serves as a testament to the potential that ASP.NET Core applications can achieve with proper utilization and expansion.
