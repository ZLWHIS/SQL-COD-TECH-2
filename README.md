Name:AYUSH SINGH

Company:CODTECH IT SOLUTIONS

Id:CT08DS6615

Domain:SQL

Duration:August to September

Mentor Name:Muzammil Ahmed

Here’s an overview of the Library Management System you’ve designed using SQL:

1. Database Creation
Database Name: LibraryManagementSystem1
This is the main database for managing all the library-related data.
2. Tables Created
Books:

Stores details of each book in the library.
Columns:
book_id (Primary Key, Auto-increment): Unique identifier for each book.
title: Title of the book.
author: Author of the book.
genre: Genre or category of the book.
published_year: Year the book was published.
available_copies: Number of copies available in the library.
Members:

Stores details of the members of the library.
Columns:
member_id (Primary Key, Auto-increment): Unique identifier for each member.
name: Name of the member.
email (Unique): Email address of the member.
phone: Phone number of the member.
join_date: Date when the member joined the library.
Transactions:

Records borrowing and returning activities.
Columns:
transaction_id (Primary Key, Auto-increment): Unique identifier for each transaction.
book_id (Foreign Key): References book_id in the Books table.
member_id (Foreign Key): References member_id in the Members table.
transaction_type: Type of transaction (either 'borrow' or 'return').
transaction_date: Date when the transaction occurred.
3. Data Insertion
Books:

Sample data for five books has been inserted.
Titles include "The Gatsby," "Machine," "Everything Peace," "Peaceful Thing," and "Politics."
These entries include details like author names, genres, publication years, and available copies.
Members:

Sample data for five members has been inserted.
Names include Aman Sharma, Kunj Mishra, Ankit Choubey, Gurmeet Thakur, and Yash Marwal.
Each entry includes details like name, email, phone number, and join date.
Transactions:

Sample transactions have been recorded, where members have borrowed books on specific dates.
4. Data Manipulation
Update Operations:

The number of available copies of "The Gatsby" was reduced by one after a borrow transaction.
The phone number of the member Aman Sharma was updated.
Delete Operations:

A book with book_id = 1 and a member with member_id = 1 were deleted from their respective tables.
5. Data Retrieval
Books:
Retrieved all book entries with their details.
Members:
Retrieved all member entries with their details.
Transactions:
Retrieved all transactions for a specific member (in this case, member_id = 1).
Available Copies by Genre:
Retrieved available copies of books filtered by the genre "Fiction."
Notes:
The database schema effectively covers the core functionalities of a Library Management System: managing books, members, and their transactions.
Proper foreign key relationships ensure data integrity between Books, Members, and Transactions.
The use of ENUM in the Transactions table for transaction_type helps enforce valid transaction types ('borrow' or 'return').
This system provides a solid foundation for managing a library's data, and it could be expanded with additional features like book reservations, fines for late returns, and more detailed member profiles if needed.



TASK 2:

Here's a simplified explanation of the Employee Management System database setup and operations:

### 1. **Database and Tables Creation:**
   - **Database:** A new database called `employeerecords1` is created.
   - **Tables:** Four tables are created within this database:
     - **Departments:** Stores department details like department ID, name, and location.
     - **JobPositions:** Stores job positions with details like position ID, title, and description.
     - **Employees:** Stores employee information, including their name, birth date, hire date, department ID, and job position ID.
     - **Salaries:** Stores salary details for employees, including salary amount and the effective date.

### 2. **Adding Records:**
   - **Departments:** Departments like Engineering, Management, and IT are added with specific locations.
   - **Job Positions:** Job roles like Software Engineer, HR Manager, and Web Developer are added.
   - **Employees:** Employee records are added, linking them to specific departments and job positions.
   - **Salaries:** Salary records for employees are inserted with specific amounts and dates.

### 3. **Fetching Data:**
   - **All Employees with Department and Position:** A query retrieves all employees, displaying their department name and job position.
   - **Salary History for an Employee:** A query shows the salary history for a specific employee.
   - **Employees in a Specific Department:** A query fetches all employees in a particular department.

### 4. **Updating and Deleting Data:**
   - **Updating Employee’s Department:** You can change an employee's department by updating their department ID.
   - **Deleting a Job Position:** A job position can be deleted if no employees are currently assigned to it.

### 5. **Fetching the Highest Salary:**
   - **Highest Salary in Each Department:** A query shows the highest salary in each department, helping to compare salary distributions across departments.

This system helps manage and organize employee-related data efficiently, including their roles, salaries, and departmental associations.
