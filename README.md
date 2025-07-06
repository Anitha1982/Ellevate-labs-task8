Stored Procedure and Function in SQL Server:

This project uses the EmployeeDB database containing an Employees table.

A stored procedure GetEmployeesByDept retrieves employees by department using a parameter @DeptId.

Execute the procedure using: EXEC GetEmployeesByDept @DeptId = 102;.

A scalar user-defined function GetPerformanceLevel calculates performance based on salary.

The function uses conditional logic (IF...ELSE) to return: 'Excellent', 'Good', or 'Needs Improvement'.

Create it with CREATE FUNCTION dbo.GetPerformanceLevel(@Salary DECIMAL(10,2)) RETURNS VARCHAR(50).

Use it in a query like: SELECT Employee_Name, dbo.GetPerformanceLevel(Salary) FROM Employees;.

Procedures are used for actions (DML/queries), functions are used for reusable computations.

Both objects accept parameters and can include conditional logic.

Use USE EmployeeDB; before creating or executing any stored procedure or function.
