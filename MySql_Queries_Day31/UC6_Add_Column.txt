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
Insert into employee_payroll ( Name, Salary, Start_Date) values ( 'Jack Parker', '45000.0', '2020-01-15'),
                                                                ( 'Riyan Smith', '50000.0', '2020-02-01'),
								( 'Rachel Brown', '65000.0', '2020-01-01'),
								( 'Nick Jonas', '49000.0', '2020-03-10'),
								( 'Alex Paul', '38000.0', '2020-03-15'),
								( 'Nia Patrik', '57000.0', '2020-03-20'),
								( 'Carol Tyler', '75000.0', '2020-04-05');
Select * From employee_payroll;   
Select salary from employee_payroll where Name = 'Alex Paul'; 
Select Name from employee_payroll where Start_Date between Cast( '2020-03-10' as date) and date(now());     
Alter table employee_payroll  add Gender varchar(1) after Name;   
Update employee_payroll set Gender = 'M' where Name = 'Jack Parker' or Name = 'Riyan Smith' or Name = 'Nick Jonas' or Name = 'Alex Paul';   
Update employee_payroll set Gender = 'F' where Name = 'Rachel Brown' or Name = 'Nia Patrik' or Name = 'Carol Tyler';            
                                                                