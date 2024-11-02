# Library-Management-System

# Overview
This Library Management System is a database-driven application designed to streamline and automate the operations of a library. Built using SQL and PL/SQL, this project includes modules for handling book issuance, returns, fine calculation, and transaction history, offering a comprehensive solution for managing a library’s records with accuracy and efficiency.

# Key Features
Member Management: Supports multiple types of library memberships (monthly, yearly, lifetime), each with specific borrowing limits.
Book Issuance and Return Tracking: Ensures books are issued only if membership and book availability criteria are met, and accurately records due dates and return dates.
Fine Calculation: Calculates late fees based on the difference between the due date and the actual return date, with customizable rates.
Automatic Updates: Uses triggers to automatically adjust book stock and member records upon issuance and return.
Transaction History: Archives completed transactions for auditing and record-keeping purposes.

# Modules
Issue Book Section
Validates member and book IDs.
Checks membership status and borrowing limits.
Ensures no duplicate borrowing of the same book.
Restricts operations on weekends.

2 Return Book Section
Verifies if the member has borrowed the book.
Updates return dates and calculates fines.
Transfers transaction data to a history table upon return.
Restricts operations on weekends.


# Database Structure
Member Table: Stores member information, including membership type and total fines.
Book Table: Contains book details, such as author, price, and availability.
Transaction Table: Logs active book borrowings with due dates and return dates.
Transaction History Table: Records completed transactions.


# Core SQL Features
Procedures and Functions: Implemented for book issuing and returning workflows.
Triggers: Automatically update book counts and move data to the transaction history.
Exception Handling: Manages errors such as borrowing limits, invalid member IDs, and unavailable books.


# Getting Started
To set up the Library Management System:

# Clone the repository:
git clone https://github.com/yourusername/library-management-system
cd library-management-system

Run SQL scripts to create tables and insert initial data in your database.



