User Profile Management Solution Readme
Welcome to the User Profile Management Solution! This repository contains a .NET Core Web API for managing user profiles, including features such as user registration, login, forgotten password recovery, password reset, and South African ID number validation. The solution also includes a .NET Core Web MVC frontend to provide a user interface for interacting with the Web API.
Features
1.	User Registration: Users can create new accounts by providing their necessary details, including email, password, and South African ID number.
2.	Login: Registered users can log in securely using their credentials.
3.	Forgotten Password Recovery: Users who have forgotten their passwords can initiate a recovery process. They will receive instructions on how to reset their password via their registered email.
4.	Password Reset: Once the forgotten password recovery process is initiated, users can reset their password securely.
5.	South African ID Number Validation: The solution provides the ability to validate South African ID numbers. It can determine the user's gender and birthdate based on a valid ID number.
6.	Profile Viewing: Successfully registered and logged-in users can view their profiles, including personal information and possibly additional details retrieved from their ID number.
Solution Structure
Backend: .NET Core Web API
•	Environments: Contains models used across the application.
•	Data: Holds the SQLite database for data persistence.
•	DAL: Contains the database context and related data access logic.
•	Controllers: Houses the RegistrationController, which handles HTTP methods for registration, login, profile, forgotten password, and password reset.
Frontend: .NET Core Web MVC
•	ViewModels: Contains view models for Registration, Login, Forgot Password, and Reset.
•	Controllers: Includes controllers for Registration, Login, and Profile actions.
•	Views: Contains corresponding views for each of the controllers.
•	Validation: Frontend validations for ID Number, password strength, and other input fields.
Getting Started
1.	Clone the Repository: Clone this repository to your local machine.
2.	Backend Setup:
•	Open the .NET Core Web API project in your preferred development environment (e.g., Visual Studio).
•	Update the database connection string in the appsettings.json file to configure your SQLite database.
•	Run the migrations to create the database schema.
•	Run the API project, which will start the backend server on http://localhost:5000.
3.	Frontend Setup:
•	Open the .NET Core Web MVC project in your preferred development environment.
•	Configure the API base URL in the frontend to match the backend URL.
•	Run the MVC project, which will start the frontend server on http://localhost:5001.
4.	Access the Application: Open a web browser and navigate to http://localhost:5001 to access the frontend interface for the User Profile Management Solution.
Contributing
Contributions are welcome! If you find a bug or have an enhancement in mind, please create an issue or a pull request following GitHub's guidelines.

