E-Ticket Booking System

Overview:
The E-Ticket Booking System is a web-based application designed for bus ticket reservations. It allows users to register, log in, view schedules, book tickets, and manage their bookings. The system is built using PHP for the backend and MySQL for the database.


Features:
User Registration & Login: Secure user authentication system.
Bus Schedule Management: View available bus schedules.
Ticket Booking: Select buses and book tickets.
Admin Panel: Manage users and bookings.


Requirements:
Web Server: Apache or Nginx
PHP: Version 7.4 or higher
Database: MySQL
PHP Extensions: mysqli, session_start


Installation:
1. Clone the Repository
git clone https://github.com/Sam24280/E-Ticket-Booking-System.git

2. Set Up the Database
Create a new database in MySQL.
Import the provided SQL file (if available) to set up the necessary tables.

3. Configure Database Connection
Navigate to includes/db.php.
Update the database connection details:

  <?php
  $servername = "localhost";
  $username = "root";
  $password = "";
  $dbname = "bus_ticket_system"; // Replace with your database name

  // Create connection
  $conn = new mysqli($servername, $username, $password, $dbname);

  // Check connection
  if ($conn->connect_error) {
      die("Connection failed: " . $conn->connect_error);
  }
  ?>

4. Set Up the Web Server
Place the project files in the web server's root directory.
Ensure that the server is configured to handle PHP files.

5. Access the Application
Open your web browser and navigate to http://localhost/bus_ticket_system.
