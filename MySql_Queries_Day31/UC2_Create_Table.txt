CREATE database Payroll_Service;
show databases;
use Payroll_Service;
CREATE table Employee_Payroll (
ID          int NOT Null auto_increment,
Name        varchar(45) Not Null,
Salary      double Not Null,
Start_Date  date Not Null,
Primary key(ID) );
Select * From employee_payroll;