# Event Planner PHP Project

## Project Description

The Event Planner PHP Project is a web-based application developed using PHP, MySQL, HTML, CSS, and JavaScript. It helps users create, organize, and manage events efficiently. The system allows event organizers to schedule events, manage participants, maintain venue details, and track event information through an easy-to-use interface.

The application includes user authentication, event management, participant registration, and an administrator panel for managing all activities. Data is securely stored in a MySQL database, ensuring efficient record management and retrieval.

## Software Requirements

* XAMPP or WAMP Server
* PHP 7.0 or above
* MySQL Database
* Web Browser (Chrome, Firefox, Edge, etc.)

## Installation and Setup

### Step 1: Install XAMPP

1. Download XAMPP from the official website.
2. Run the installer and complete the installation process.
3. Open the XAMPP Control Panel.
4. Start the **Apache** and **MySQL** services.

### Step 2: Install WAMP (Alternative)

1. Download and install WAMP Server.
2. Launch WAMP Server.
3. Ensure Apache and MySQL services are running (green icon in the taskbar).

### Step 3: Copy Project Files

1. Extract the Event Planner project folder.
2. Copy the project folder into:

   * XAMPP: `C:\xampp\htdocs\`
   * WAMP: `C:\wamp64\www\`

Example:

```
C:\xampp\htdocs\Event-Planner-PHP-Project
```

### Step 4: Create Database

1. Open a web browser.
2. Visit:

```
http://localhost/phpmyadmin
```

3. Click **New**.
4. Create a database (for example):

```
event_planner
```

### Step 5: Import Database

1. Select the newly created database.
2. Click the **Import** tab.
3. Browse and select the SQL file provided with the project.
4. Click **Go** to import all tables and data.

### Step 6: Configure Database Connection

Open the database configuration file (such as `config.php` or `db_connect.php`) and update the database credentials:

```php
<?php
$servername = "localhost";
$username = "root";
$password = "";
$database = "event_planner";

$conn = mysqli_connect($servername, $username, $password, $database);

if(!$conn){
    die("Connection Failed: " . mysqli_connect_error());
}
?>
```

### Step 7: Run the Project

1. Start Apache and MySQL services.
2. Open a web browser.
3. Enter the project URL:

```
http://localhost/Event-Planner-PHP-Project/
```

or

```
http://localhost/project-folder-name/
```

4. The Event Planner home page will open.

## Project Modules

### User Module

* User Registration
* User Login
* Create Events
* View Event Details
* Manage Personal Events

### Admin Module

* Admin Login
* Manage Users
* Manage Events
* Update Event Information
* Monitor Registrations
* Generate Reports

## Database Connectivity

The project uses MySQL for storing user and event information. PHP's MySQLi functions are used to establish a connection between the application and the database.

## Conclusion

The Event Planner PHP Project provides an efficient solution for managing events through a web-based platform. It reduces manual work, improves event coordination, and demonstrates the practical implementation of PHP, MySQL, database connectivity, and web application development concepts.
