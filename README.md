# E-Commerce Platform

## Project Overview
This repository contains the source code for a fully functional e-commerce platform developed using Java and other necessary tools. The platform includes features like user authentication, product management, shopping cart functionality, and admin dashboards.

## Features
- User authentication with secure login and registration.
- Role-based access control for buyers and administrators.
- Product catalog with search and filter functionality.
- Shopping cart with real-time updates.
- Order management and tracking.
- Responsive design for all devices.
- Admin dashboard for inventory and sales analytics.

## Tech Stack
- *Backend:* Java, JDBC, Servlet JSP, Hibernate
- *Frontend:* HTML, CSS, JavaScript, Bootstrap
- *Database:* MySQL
- *Server:* Apache Tomcat
- *IDE:* NetBeans

## Prerequisites
1. *Java Development Kit (JDK):* Ensure JDK 8 or higher is installed.
2. *Apache Tomcat:* Install Apache Tomcat server (version 9 or higher recommended).
3. *MySQL Database:* Install MySQL and set up the database.
4. *SQLYog:* (Optional) Use SQLYog for database management.

## Installation Instructions

### Step 1: Clone the Repository
bash
git clone <your-github-repo-link>
cd <repository-name>


### Step 2: Database Setup
1. Open MySQL or SQLYog.
2. Create a new database (e.g., ecommerce_db).
3. Import the SQL dump file provided in the database/ directory:
   sql
   source database/ecommerce_db.sql;
   

### Step 3: Configure Database Connection
1. Open the dbconfig.properties file in the src/ directory.
2. Update the following properties with your MySQL credentials:
   properties
   db.url=jdbc:mysql://localhost:3306/ecommerce_db
   db.username=<your-mysql-username>
   db.password=<your-mysql-password>
   

### Step 4: Deploy on Apache Tomcat
1. Open the project in NetBeans.
2. Clean and build the project to generate a .war file.
3. Copy the .war file to the webapps directory of Apache Tomcat.
4. Start the Apache Tomcat server.

### Step 5: Access the Application
1. Open your web browser.
2. Navigate to:
   
   http://localhost:8080/<your-project-name>
   

## Usage
### Buyer
- Register or log in to the platform.
- Browse products, add them to the cart, and place an order.
- View order history and track current orders.

### Administrator
- Log in using admin credentials.
- Add, update, or delete products.
- Monitor orders and analyze sales data.

## Troubleshooting
- *Issue:* Unable to connect to the database.
  - *Solution:* Verify the database credentials in dbconfig.properties.
- *Issue:* Tomcat server not starting.
  - *Solution:* Check if another process is using port 8080, or update the port in server.xml.
- *Issue:* Missing dependencies.
  - *Solution:* Ensure all required libraries are included in the lib/ folder.

## Future Enhancements
- Integration with real-world payment gateways.
- AI-driven product recommendations.
- Advanced security features like two-factor authentication.
- Mobile application development.

## Contributors
- Toffek Usmani
- Viwek Raj Anand


For any issues or questions, please contact toffekusmani786@gmail.com
