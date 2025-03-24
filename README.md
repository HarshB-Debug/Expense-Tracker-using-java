# Expense-Tracker-using-java
# Expense Service

## Overview
The **Expense Service** is a simple Java-based application that manages expense records. It allows users to **add, edit, delete, and retrieve** expenses using an in-memory data structure.

## Features
- Add a new expense with **description, amount, and date**.
- Edit an existing expense by **ID**.
- Delete an expense by **ID**.
- Retrieve all expenses.
- Get a specific expense by **ID**.

## Technologies Used
- **Java** (Core Java concepts including OOP, Collections, and Streams)
- **ArrayList** for in-memory storage

## Installation & Setup
### Prerequisites
- Install **Java 8+**
- Use a Java IDE such as **IntelliJ IDEA**, **Eclipse**, or **VS Code**

### Installation Steps
1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/ExpenseService.git
   ```
2. Open the project in your preferred Java IDE.
3. Compile and run the Java files.

## Usage
### Adding an Expense
```java
ExpenseService expenseService = new ExpenseService();
expenseService.addExpense("Groceries", 1500.50, "2024-03-24");
```

### Editing an Expense
```java
expenseService.editExpense(1, "Groceries - Supermarket", 1600.00, "2024-03-25");
```

### Deleting an Expense
```java
expenseService.deleteExpense(1);
```

### Retrieving All Expenses
```java
List<ExpenseItem> expenses = expenseService.getAllExpenses();
```

### Retrieving an Expense by ID
```java
ExpenseItem expense = expenseService.getExpenseById(1);
```

## Project Structure
```
📂 ExpenseServiceProject
 ┣ 📜 ExpenseService.java   # Main service to manage expenses
 ┣ 📜 ExpenseItem.java      # Model class for expense details
 ┗ 📜 README.md             # Project documentation

```
![Screenshot 2025-03-24 121045](https://github.com/user-attachments/assets/eb550a04-709f-4722-aafa-3ff6d96d3e5d)


## Future Enhancements
- Implement **database storage** (MySQL, PostgreSQL).
- Create a **REST API** using Spring Boot.
- Develop a **web-based UI** for better user interaction.

## License
This project is licensed under the **MIT License**.

