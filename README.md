Employee Management System – OOP Wrapper

📌 Project Overview

The Employee Management System is a Python-based console application created using Object-Oriented Programming (OOP) concepts.

This project demonstrates important OOP concepts such as:

- Classes and Objects
- Inheritance
- Encapsulation
- Method Overriding
- Getters and Setters
- "super()"
- Dictionaries
- Loops and Conditional Statements
- Built-in functions such as "issubclass()"

🎯 Project Objective

The main objective of this project is to understand how OOP concepts can be combined to create a simple Employee Management System.

The system allows users to:

1. Create Person details
2. Add Employee details
3. Add Manager details
4. Display individual details
5. Display all employees
6. Display all managers
7. Exit the program

🏗️ Class Structure

Person
   │
   └── Employee
          │
          └── Manager

1. Person Class

The "Person" class is the parent/base class.

It contains:

- Name
- Age
- "display()" method

2. Employee Class

The "Employee" class inherits from "Person".

It contains:

- Employee ID
- Salary
- Getters and setters
- Employee details display

Private attributes are used for encapsulation:

self.__employee_id
self.__salary

3. Manager Class

The "Manager" class inherits from "Employee".

It contains:

- Manager ID
- Salary
- Department
- Manager-specific "display()" method

The "display()" method is overridden to demonstrate method overriding.

🔐 Encapsulation

Encapsulation is implemented using private attributes:

self.__employee_id
self.__salary

Access to these attributes is controlled using getter and setter methods.

Example:

def get_salary(self):
    return self.__salary

def set_salary(self, salary):
    if salary >= 0:
        self.__salary = salary

The salary setter also prevents negative salary values.

🧬 Inheritance

The project demonstrates multilevel inheritance:

Person → Employee → Manager

For example:

class Employee(Person):

and:

class Manager(Employee):

This allows child classes to reuse properties and methods from their parent classes.

🔄 Method Overriding

The "Manager" class overrides the "display()" method of the "Employee" class.

def display(self):
    print("\nManager Details:")

This demonstrates polymorphism through method overriding.

📚 Data Storage

Dictionaries are used to store multiple employee and manager records.

employees = {}
managers = {}

Employee records are stored using the Employee ID as the dictionary key.

Manager records are stored using the Manager ID as the dictionary key.


🖥️ Menu Options

========== Employee Management System ==========

1. Person Details
2. Employee Details
3. Manager Details
4. Show Details
5. Display All Employees
6. Display All Managers
7. Exit

Option 1 – Person Details

Creates and displays a Person object.

Option 2 – Employee Details

Creates an Employee object and stores the employee information.

Option 3 – Manager Details

Creates a Manager object and stores the manager information.

Option 4 – Show Details

Displays the details of the selected Person, Employee, or Manager.

Option 5 – Display All Employees

Displays all employee records stored in the dictionary.

Option 6 – Display All Managers

Displays all manager records stored in the dictionary.

Option 7 – Exit

Exits the program and demonstrates inheritance using "issubclass()".

🔎 OOP Concepts Demonstrated

OOP Concept| Implementation
Class| "Person", "Employee", "Manager"
Object| "person", "employee", "manager"
Inheritance| "Employee(Person)", "Manager(Employee)"
Encapsulation| Private ID and salary
Getter| "get_salary()", "get_employee_id()"
Setter| "set_salary()", "set_employee_id()"
Method Overriding| "Manager.display()"
"super()"| Used in child class constructors
Polymorphism| Overridden "display()" method

▶️ How to Run

Step 1: Install Python

Make sure Python is installed on your system.

Step 2: Save the File

Save the Python code as:

main.py

Step 3: Run the Program

Open the terminal in the project folder and run:

python main.py

💡 Example

========== Employee Management System ==========
1. Person Details
2. Employee Details
3. Manager Details
4. Show Details
5. Display All Employees
6. Display All Managers
7. Exit

Enter your choice: 2

Enter Employee Name: Digna
Enter Age: 17
Enter Employee ID: E101
Enter Salary: 25000

Employee added successfully.

Employee Details:
Name: Digna
Age: 17
Employee ID: E101
Salary: 25000.0

🛠️ Technologies Used

- Python
- Object-Oriented Programming
- Dictionaries
- Console / CLI

🎓 Learning Outcome

Through this project, I learned how to implement OOP concepts in Python and how different classes can work together in a real-world application.

This project helped me understand Inheritance, Encapsulation, Polymorphism, Classes, Objects, Getters, Setters, and Method Overriding in a practical way.

👩‍💻 Author

Digna Vora

B.Sc. IT – AI & ML

⭐ If you found this project useful, feel free to explore the code and learn from it.

🎥 Explanation Video:

https://drive.google.com/file/d/1vavxF9pyszrAHmWF1irAa3ziXuP2d9PX/view?usp=sharing

## ⭐ Conclusion

This project is a practical implementation of **Object-Oriented Programming in Python**. It demonstrates how OOP concepts can be combined to create a simple and organized **Employee Management System**

📞 Contact Me:

📧 Email: dignavora8233@gmail.com

💼 LinkedIn: www.linkedin.com/in/digna-vora-b135a3416
