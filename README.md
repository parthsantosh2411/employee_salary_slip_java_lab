# Payroll System

This Java program implements a simple payroll system for managing employee salaries.

## Classes:
1. **Employee**: An abstract class representing common attributes and methods for all employees.
2. **NormalEmployee**: A subclass of `Employee` representing employees without bonus eligibility.
3. **BonusEmployee**: A subclass of `Employee` representing employees eligible for bonuses.
4. **Main**: Contains the main method to run the program and interact with users.

## Function:
1. **Employee**: An abstract class representing common attributes and methods for all employees.

   - `Employee(String empName, String empAddress, int basicWage)`: Constructor method that initializes an Employee object with the provided name, address, and basic wage.
   
   - `abstract void salaryCalculation()`: Abstract method to be implemented by subclasses for calculating the salary of an employee.
   
   - `void getEmployeeDetails()`: Method to input employee details such as employee ID, department, date of joining, etc.
   
   - Getter and setter methods for various attributes like employee ID, department, date of joining, etc.

2. **NormalEmployee**: A subclass of `Employee` representing employees without bonus eligibility.

   - `NormalEmployee(String name, String address, int basicSalary, double bonusPercentage)`: Constructor method to initialize a NormalEmployee object with the provided name, address, basic salary, and bonus percentage.
   
   - `NormalEmployee()`: Default constructor method that initializes a NormalEmployee object with default values and prompts the user to input bonus eligibility.
   
   - `@Override void salaryCalculation()`: Overridden method to calculate the salary of a normal employee based on the provided or default values.

3. **BonusEmployee**: A subclass of `Employee` representing employees eligible for bonuses.

   - `BonusEmployee(String name, String address, int basicSalary, double bonusPercentage)`: Constructor method to initialize a BonusEmployee object with the provided name, address, basic salary, and bonus percentage.
   
   - `BonusEmployee()`: Default constructor method that initializes a BonusEmployee object with default values and prompts the user to input bonus eligibility and percentage.
   
   - `@Override void salaryCalculation()`: Overridden method to calculate the salary of a bonus employee, including the bonus amount based on the provided or default percentage.

4. **Main**: Contains the main method to run the program and interact with users.

   - `public static void main(String[] args)`: The main method where the program starts execution. It prompts the user to choose the type of employee, gets employee details, and calculates the salary accordingly.

## Features

- Allows input of employee details such as name, address, basic wage, etc.
- Calculates salary based on provided or default values and deductions like EPF and ESI.
- Handles both normal employees and those eligible for bonuses.

## Usage

To use the program:

1. Run the `Main` class.
2. Choose whether the employee is a bonus employee or not.
3. Provide employee details when prompted.
4. The program will calculate and display the employee's salary.

## Requirements

- Java Development Kit (JDK) installed on your system.

