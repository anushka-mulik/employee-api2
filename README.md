# employee-api2



Test API
Get All Employees
GET http://localhost:3000/employees

Response:

[
  {
    "id": 1,
    "name": "Rahul",
    "position": "Developer"
  },
  {
    "id": 2,
    "name": "Priya",
    "position": "Manager"
  }
]
Add Employee
POST http://localhost:3000/employees

Body (JSON):

{
  "name": "Amit",
  "position": "Tester"
}

Response:

{
  "message": "Employee added successfully",
  "employee": {
    "id": 3,
    "name": "Amit",
    "position": "Tester"
  }
}
Update Employee
PUT http://localhost:3000/employees/1

Body:

{
  "name": "Rahul Sharma",
  "position": "Senior Developer"
}
Delete Employee
DELETE http://localhost:3000/employees/1

Response:

{
  "message": "Employee deleted successfully"
}
