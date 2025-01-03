Open the Project in your IDE
Open your IDE ( NetBeans).
Import or open the project as a Maven Project (if using Maven).
Check the src/main/java/com/ecommerce/config/DatabaseConnection.java file to configure your database connection.
3. Configure the Database Connection
In DatabaseConnection.java, update the following properties with your own MySQL configuration:

Database Setup
Create the Database: Open MySQL and create a new database named ecommerce (or a name of your choice). You can use the following command:
sql
Copy code
CREATE DATABASE ecommerce;
Create Tables: Run the SQL script found at src/resources/db/schema.sql to create the required tables. You can execute the script using a MySQL client like SQLYog, MySQL Workbench, or directly in the MySQL command line:
bash
Verify Tables: Ensure that tables like User, Product, Order, CartItem, and Category are created correctly.

Running the Application
Start the Tomcat Server:

In your IDE, configure and start the Apache Tomcat server.
Set the context path to /ecommerce-platform or a path of your choice.
Deploy the application on the server.
Access the Application:

Open a web browser and go to http://localhost:8080/ecommerce-platform to access the application.
Logging In / Creating an Account:

Go to the registration page to create a new user account.
Once registered, log in to browse products, add items to the cart, and place orders.
