# Customer Management API
A simple customer management system API with a RAML specification for API design and developed with Mule ESB. The underlying system is a MySQL database that contains customer records.

 - [RAML Design](resources/raml)
 - [Mule ESB project](customersapi)

### Instructions to Setup and Run
  - Execute the MySQL script in [here](resources/db) to create the database
  - Add the database connection details in [here](customersapi/src/main/resources/db/db-config.properties)
  - Import the mule project to Anypoint studio and Run the project

### Invoke the API
Following are examples for invoking the API
  - Invoke the get customers with following curl command
```sh
$ curl -i -H "Authorization:Basic 1234567" http://localhost:8081/api/customers
```
  - Invoke the get customers by id with the following curl command
```sh
$ curl -i -H "Authorization:Basic 1234567" http://localhost:8081/api/customers/1
```
