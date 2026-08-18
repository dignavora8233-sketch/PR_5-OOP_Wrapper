# ============================================================
#      OOP Wrapper - Employee Management System
# ============================================================


# -------------------- Person Class --------------------

class Person:

    def __init__(self, name, age):
        self.name = name
        self.age = age

    def display(self):
        print("\nPerson Details:")
        print("Name:", self.name)
        print("Age:", self.age)


# -------------------- Employee Class --------------------

class Employee(Person):

    def __init__(self, name, age, employee_id, salary=0):
        super().__init__(name, age)

        # Encapsulation
        self.__employee_id = employee_id
        self.__salary = salary

    # Getter
    def get_employee_id(self):
        return self.__employee_id

    # Setter
    def set_employee_id(self, employee_id):
        self.__employee_id = employee_id

    # Getter
    def get_salary(self):
        return self.__salary

    # Setter
    def set_salary(self, salary):
        if salary >= 0:
            self.__salary = salary
        else:
            print("Salary cannot be negative.")

    # Display method
    def display(self):
        print("\nEmployee Details:")
        print("Name:", self.name)
        print("Age:", self.age)
        print("Employee ID:", self.get_employee_id())
        print("Salary:", self.get_salary())


# -------------------- Manager Class --------------------

class Manager(Employee):

    def __init__(self, name, age, manager_id, salary, department):
        super().__init__(name, age, manager_id, salary)

        self.department = department

    # Method Overriding
    def display(self):
        print("\nManager Details:")
        print("Name:", self.name)
        print("Age:", self.age)
        print("Manager ID:", self.get_employee_id())
        print("Salary:", self.get_salary())
        print("Department:", self.department)


# -------------------- Main Program --------------------

person = None
employee = None
manager = None


# Dictionaries to store multiple details
employees = {}
managers = {}


while True:

    print("\n========== Employee Management System ==========")
    print("1. Person Details")
    print("2. Employee Details")
    print("3. Manager Details")
    print("4. Show Details")
    print("5. Display All Employees")
    print("6. Display All Managers")
    print("7. Exit")

    choice = input("Enter your choice: ")


    # -------------------- Person --------------------

    if choice == "1":

        name = input("Enter Person Name: ")
        age = int(input("Enter Age: "))

        person = Person(name, age)

        print("\nPerson created successfully.")

        person.display()


    # -------------------- Employee --------------------

    elif choice == "2":

        name = input("Enter Employee Name: ")
        age = int(input("Enter Age: "))
        employee_id = input("Enter Employee ID: ")
        salary = float(input("Enter Salary: "))

        employee = Employee(
            name,
            age,
            employee_id,
            salary
        )

        # Store employee details
        employees[employee_id] = {
            "Name": name,
            "Age": age,
            "Employee ID": employee_id,
            "Salary": salary,
         }

        print("\nEmployee added successfully.")

        employee.display()


    # -------------------- Manager --------------------

    elif choice == "3":

        name = input("Enter Manager Name: ")
        age = int(input("Enter Age: "))
        manager_id = input("Enter Manager ID: ")
        salary = float(input("Enter Salary: "))
        department = input("Enter Department: ")

        manager = Manager(
            name,
            age,
            manager_id,
            salary,
            department
        )

        # Store manager details
        managers[manager_id] = {
            "Name": name,
            "Age": age,
            "Manager ID": manager_id,
            "Salary": salary,
            "Department": department,
            "Role": "Manager"
        }

        print("\nManager added successfully.")

        manager.display()


    # -------------------- Show Details --------------------

    elif choice == "4":

        print("\nChoose details to show:")
        print("1. Person")
        print("2. Employee")
        print("3. Manager")

        detail_choice = input("\nEnter your choice: ")

        if detail_choice == "1":

            if person is not None:
                person.display()
            else:
                print("\nPerson has not been created yet.")

        elif detail_choice == "2":

            if employee is not None:
                employee.display()
            else:
                print("\nEmployee has not been created yet.")

        elif detail_choice == "3":

            if manager is not None:
                manager.display()
            else:
                print("\nManager has not been created yet.")

        else:
            print("\nInvalid detail choice!")


    # -------------------- Display All Employees --------------------

    elif choice == "5":

        print("\n========== All Employees ==========")

        if employees:

            for employee_id, details in employees.items():

                print("\nEmployee ID:", employee_id)

                for key, value in details.items():
                    print(key + ":", value)

        else:
            print("No employee data available.")


    # -------------------- Display All Managers --------------------

    elif choice == "6":

        print("\n========== All Managers ==========")

        if managers:

            for manager_id, details in managers.items():

                print("\nManager ID:", manager_id)

                for key, value in details.items():
                    print(key + ":", value)

        else:
            print("No manager data available.")


    # -------------------- Exit --------------------

    elif choice == "7":

        print("\nThank you for using Employee Management System.")
        print("Goodbye!!")

        print(
            "\nIs Employee a subclass of Person?",
            issubclass(Employee, Person)
        )

        print(
            "Is Manager a subclass of Employee?",
            issubclass(Manager, Employee)
        )

        break


    # -------------------- Invalid Choice --------------------

    else:

        print("\nInvalid choice. Please try again.")
