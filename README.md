# project-bank-management-system
A Python-based Bank Management System that demonstrates the core pillars of Object-Oriented Programming (OOP). The project utilizes abstraction, encapsulation, inheritance, and polymorphism to simulate banking operations for different types of bank accounts.
##  Core OOP Features Implemented

*   **Abstraction**: Utilizes the `abc` module (`ABC` and `@abstractmethod`) to create an abstract base class `Account` with a mandatory abstract `withdraw` method.
*   **Encapsulation**: Demonstrates strict access control modifiers:
    *   **Public**: `acc_no` (accessible anywhere).
    *   **Protected**: `_acc_name` (intended for internal/subclass use).
    *   **Private**: `__balance` (hidden from direct outside access, managed securely via Getter `get_balance()` and Setter `set_balance()` methods).
*   **Inheritance**: Subclasses `SavingAccount` and `CurrentAccount` inherit core functionalities from the base `Account` class.
*   **Polymorphism (Method Overriding)**: The `withdraw` method is customized independently in both subclasses to apply specific banking rules.


## Account Types & Rules

1.  **Saving Account (`SavingAccount`)**:
    *   Standard withdrawal rule.
    *   Ensures the withdrawal amount does not exceed the available current balance (`amount <= balance`).
2.  **Current Account (`CurrentAccount`)**:
    *   Includes a flexible financial buffer.
    *   Supports an **Overdraft Limit of 700 Tk**, allowing users to withdraw slightly more than their active balance.
  
    *   ## How to Run
You can run this project in any Python environment, such as **Google Colab**, **Jupyter Notebook**, or any local IDE (like VS Code or PyCharm). Just copy the code and run the cells!
