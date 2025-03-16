📌 Features
  📊 Real-time tracking of food inventory.
  🔍 Pilferage detection through logging and user activity tracking.
  📅 Reports and analytics on food usage and losses.
  🔑 User roles (Admin, Staff) with different permissions.
  🔄 Integration with inventory management for automated alerts.

🛠️ Installation Guide
Prerequisites
  - Install XAMPP and start Apache and MySQL.
Steps to Install
  - Download and Extract the Project
  - Download the ZIP file of the project.
  - Extract the folder and place it inside C:\xampp\htdocs\.

Import the Database
  - Open phpMyAdmin (http://localhost/phpmyadmin).
  - Click New, create a database named food_pilferage_db.
  - Click Import, then select database/food_pilferage_db.sql.

Configure Database Connection (if needed)
  - Open include/connect_db.php and make sure the database details match:
    <?php
      $hostname = "localhost";
      $username = "root";
      $password = "";
      $db_name = "food_pilferage_db";
      
      $conn = new mysqli($hostname, $username, $password, $db_name);
      
      if($conn->connect_error){
          die("Connection failed: ". $conn->connect_error);
      }
      
      ?>
    
Run The Poject
