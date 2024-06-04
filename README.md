Food Delivery App
Overview
This Food Delivery App is a desktop application built using Java Swing for the graphical user interface. The app provides different interfaces for riders, restaurants, and users, allowing each to log in and manage their respective tasks. User credentials are securely stored in a database.

Features
User Interface: Users can log in, browse restaurants, place orders, and track their order status.
Restaurant Interface: Restaurants can log in, manage their menus, and view orders placed by users.
Rider Interface: Riders can log in, view delivery requests, and update the status of deliveries.
Authentication: Secure login for users, restaurants, and riders, with credentials stored in a database.
Prerequisites
Java Development Kit (JDK) 8 or higher
Apache Maven


MySQL or any other relational database
Installation
Setting Up the Database
Install MySQL and create a database named food_delivery.
Create the necessary tables for users, restaurants, and riders. An example SQL script is provided below:
sql
Copy code from the provided database file


Configuring the Application
Clone the repository to your local machine.
bash
Copy code
git clone https://github.com/yourusername/food-delivery-app.git
cd food-delivery-app
Open the project in your favorite IDE (e.g., IntelliJ IDEA, Eclipse).
Update the database configuration in the DatabaseConfig.java file:
java
Copy code
public class DatabaseConfig {
    public static final String URL = "jdbc:mysql://localhost:3306/food_delivery";
    public static final String USERNAME = "your_db_username";
    public static final String PASSWORD = "your_db_password";
}
Build the project using Maven:
bash
Copy code
mvn clean install
Running the Application
After building the project, run the main class FoodDeliveryApp.java to start the application.
You will be presented with the login screen. Choose your role (User, Restaurant, Rider) and enter the corresponding credentials to log in.
Project Structure
src/main/java/com/fooddelivery/ - Contains all Java source files.
config/ - Database configuration.
dao/ - Data Access Objects for interacting with the database.
models/ - Java classes representing the data model.
ui/ - User interface classes for different roles.
util/ - Utility classes for common operations.
src/main/resources/ - Contains any static resources like images and configuration files.
pom.xml - Maven configuration file for dependencies and build configuration.
Usage
User: After logging in, users can browse available restaurants, view menus, place orders, and track order status.
Restaurant: Restaurants can log in to manage their menu items, view incoming orders, and update the status of orders.
Rider: Riders can log in to see available delivery requests and update the status of deliveries.
Contributing
Fork the repository.
Create a new branch (git checkout -b feature/your-feature-name).
Commit your changes (git commit -am 'Add new feature').
Push to the branch (git push origin feature/your-feature-name).
Create a new Pull Request.
License
This project is licensed under the MIT License. See the LICENSE file for more details.

Contact
For any questions or suggestions, feel free to open an issue in the repository or contact the project maintainers.

Thank you for using the Food Delivery App! We hope it meets your needs and simplifies the food ordering and delivery process.
