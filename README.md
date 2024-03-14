# SLIATE-Assignment_Draft

# Java CRUD Application with MySQL Database

This is a simple Java application developed using Netbeans IDE that connects to a MySQL database and performs CRUD (Create, Read, Update, Delete) operations on a table named `student`. The application provides a graphical user interface (GUI) for interacting with the database.

## Functionality

### Create
- Allows users to add new student records to the database.
- When the user fills out the required information (Name, Department, Year, Email, Contact No) and clicks on the "Add" button, the data is inserted into the `student` table in the MySQL database.

### Read/View
- Displays existing student records from the `student` table in a table format on the GUI.
- When the application starts, it fetches all existing records from the `student` table and displays them in the table.

### Update
- Allows users to update existing student records in the database.
- Users can select a record from the displayed table, and its details will be populated in the input fields on the GUI. They can then modify any information and click on the "Update" button to save the changes to the database.

### Delete
- Enables users to delete existing student records from the database.
- Users can select a record from the displayed table and click on the "Delete" button. A confirmation dialog will prompt the user to confirm the deletion. If confirmed, the selected record will be removed from the `student` table.

## Usage

To use this application:

1. Ensure you have Netbeans IDE installed on your system.
2. Set up a MySQL database with a table named `student`. You can use the provided SQL script to create the table.
3. Open the project in Netbeans IDE.
4. Modify the `db.java` file in the `database` package to provide your MySQL database connection details.
5. Run the project.
6. Use the GUI to perform CRUD operations on the `student` table.

## Database Schema

The `student` table schema consists of the following columns:

- `s_id` (Student ID, Primary Key)
- `name` (Student Name)
- `department` (Student Department)
- `year` (Year of Study)
- `email` (Student Email)
- `contact` (Student Contact Number)

## SQL Script for Database Table Creation

```sql
CREATE TABLE `student` (
  `s_id` int(11) NOT NULL AUTO_INCREMENT,
  `name` varchar(255) NOT NULL,
  `department` varchar(255) NOT NULL,
  `year` int(11) NOT NULL,
  `email` varchar(255) NOT NULL,
  `contact` varchar(15) NOT NULL,
  PRIMARY KEY (`s_id`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4;
```

## Dependencies

This project utilizes the following dependencies:

- MySQL Connector/J: JDBC driver for connecting Java applications to MySQL databases.
- Swing Framework: Java's GUI toolkit for creating graphical user interfaces.

## Author

This project was developed by [@M-Samly](https://github.com/M-Samly)
