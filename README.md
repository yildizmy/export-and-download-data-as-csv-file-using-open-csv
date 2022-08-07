# Export Data as CSV using OpenCSV
Project used for exporting data as csv file using OpenCSV.


## Description

Employee list can be populated by using `employees_request.json` file and corresponding endpoint.

## Getting Started

### Dependencies

* Spring Web
* Spring Boot
* Spring Data JPA
* OpenCSV
* H2 Database

### Installing

* Database connection url for DBeaver, etc.

```
jdbc:h2:tcp://localhost:9092/mem:employee-db
```

### API Endpoints

All URIs are relative to *http://localhost:8080/api/v1*

Class | Method                                                                  | HTTP request                  | Description
------------ |-------------------------------------------------------------------------|-------------------------------| -------------
*EmployeeController* | [**create**](http://localhost:8080/api/v1/employees)                    | **POST** /employees           | Create an employee
*EmployeeController* | [**createFromFile**](http://localhost:8080/api/v1/employees/{fileName}) | **POST** /employees/{fileName} | Create employees from given JSON file
*EmployeeController* | [**findByEmail**](http://localhost:8080/api/v1/employees/{email})       | **GET** /employees/{email}    | Get employee by email
*EmployeeController* | [**findAll**](http://localhost:8080/api/v1/employees)                   | **GET** /employees            | Get all employees
*EmployeeController* | [**export**](http://localhost:8080/api/v1/employees/export)             | **GET** /employees/export     | Export employee list to CSV file
*EmployeeController* | [**deleteById**](http://localhost:8080/api/v1/employees/{id})           | **DELETE** /employees/{id}   | Delete employee by id
*EmployeeController* | [**deleteAll**](http://localhost:8080/api/v1/employees)                 | **DELETE** /employees   | Delete all employees


## Documentation
[Access a File from the Classpath in a Spring Application](https://www.baeldung.com/spring-classpath-file-access#3-using-resourceloader)<br/>


## Authors
Murat Yıldız


## Version History

* 0.2
  * Various bug fixes and optimizations
  * See [commit change]() or See [release history]()
* 0.1
  * Initial Release


## License

...


## Acknowledgments
...