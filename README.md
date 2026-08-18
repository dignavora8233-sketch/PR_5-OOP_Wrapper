# OOP Wrapper - Employee Management System

## 📌 Project Overview

**OOP Wrapper - Employee Management System** is a Python-based project created to demonstrate the core concepts of **Object-Oriented Programming (OOP)**.

The project manages details of **Persons, Employees, and Managers** using classes, inheritance, encapsulation, method overriding, and dictionaries.

## 🎯 Objectives

The main objectives of this project are:

* Understand the basics of Object-Oriented Programming.
* Implement classes and objects in Python.
* Demonstrate **Inheritance**.
* Demonstrate **Encapsulation** using private attributes.
* Demonstrate **Method Overriding**.
* Use **Getters and Setters**.
* Store and display multiple employee and manager records.
* Create a menu-driven Employee Management System.

## 🛠️ Technologies Used

* **Programming Language:** Python
* **Concept:** Object-Oriented Programming
* **Data Structure:** Dictionary
* **Interface:** Command Line Interface (CLI)

## 🧩 OOP Concepts Used

### 1. Class and Object

The project contains different classes:

* `Person`
* `Employee`
* `Manager`

Objects are created from these classes to store and manage information.

### 2. Inheritance

`Employee` inherits from `Person`.

```python
class Employee(Person):
```

`Manager` inherits from `Employee`.

```python
class Manager(Employee):
```

This demonstrates **multilevel inheritance**.

### 3. Encapsulation

Employee ID and salary are stored using private attributes:

```python
self.__employee_id
self.__salary
```

They are accessed through getter and setter methods.

### 4. Getter and Setter

Getter methods are used to retrieve private data:

```python
def get_salary(self):
    return self.__salary
```

Setter methods are used to update data safely:

```python
def set_salary(self, salary):
    if salary >= 0:
        self.__salary = salary

### 5. Method Overriding

The `Manager` class overrides the `display()` method of the parent class.

def display(self):

This demonstrates **polymorphism through method overriding**.

### 6. `super()`

The `super()` function is used to call the constructor of the parent class.

```python
super().__init__(name, age)

## 📋 Features

The program provides the following menu options:

1. **Person Details**
2. **Employee Details**
3. **Manager Details**
4. **Show Details**
5. **Display All Employees**
6. **Display All Managers**
7. **Exit**

## 👤 Person

The `Person` class stores:

* Name
* Age

Example:

Person Details:
Name: Digna
Age: 17

## 👨‍💼 Employee

The `Employee` class stores:

* Name
* Age
* Employee ID
* Salary
* Role

Employee records are stored in the `employees` dictionary.

Example:

Employee Details:
Name: Digna
Age: 17
Employee ID: E101
Salary: 25000

## 👨‍💼 Manager

The `Manager` class extends the `Employee` class and additionally stores:

* Department

Manager records are stored in the `managers` dictionary.

Example:

Manager Details:
Name: Rahul
Age: 30
Employee ID: M101
Salary: 50000
Department: IT

## 💻 Sample Menu

========== Employee Management System ==========
1. Person Details
2. Employee Details
3. Manager Details
4. Show Details
5. Display All Employees
6. Display All Managers
7. Exit

Enter your choice:

## 📚 Learning Outcomes

After completing this project, you can understand:

* Classes and Objects
* Constructors
* Inheritance
* Multilevel Inheritance
* Encapsulation
* Private Attributes
* Getters and Setters
* Method Overriding
* `super()` function
* Dictionaries
* Menu-driven programs
* Basic Employee Management System design

## 🔮 Future Improvements

The project can be extended with:

* Developer class
* Delete employee/manager functionality
* Update employee information
* Search employee by ID
* Save data into a file
* Database connectivity
* Login system
* GUI using Tkinter

## 👩‍💻 Author

**Digna Vora**

B.Sc. IT – AI & ML

🎥 Explanation Video:

https://drive.google.com/file/d/1vavxF9pyszrAHmWF1irAa3ziXuP2d9PX/view?usp=sharing

## ⭐ Conclusion

This project is a practical implementation of **Object-Oriented Programming in Python**. It demonstrates how OOP concepts can be combined to create a simple and organized **Employee Management System**

📞 Contact Me:

📧 Email: dignavora8233@gmail.com
💼 LinkedIn: www.linkedin.com/in/digna-vora-b135a3416
