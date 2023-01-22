
# BlackCoffer - EMS

BlackCoffer Internship Assesment task: Employee Management System uisng Rest-API, SpringBoot, Thymeleaf, SpringSecurity, SQL


## API Reference

#### Get All uers 

```http
  GET http://localhost:8080/
```



#### To Create User

```http
  POST http://localhost:8080/registration
```

| Parameter | Type     | 
| :-------- | :------- | 
| `email`      | `string` |
| `first_name`      | `string` | 
| `last_name`      | `string` |
| `password`      | `string` |



1.Pass following JSON format in Body of API
```yaml
{ 
  "email":"chetasraulkar774@gmail.com", 
  "first_name":"Chetas",
  "last_name":"Raulkar",
  "password":"Chetas@11"
}
```
#### To create Employee
```http
  POST http://localhost:8080/showNewEmployeeForm
```
1.Authenticate User 
```yaml
{
    email:"chetasraulkar774@gmail.com",
    password:"Chetas@11"
}
```
2.Pass following JSON format in Body of API
```yaml
{ 
  "email":"chetasraulkar774@gmail.com", 
  "first_name":"Chetas",
  "last_name":"Raulkar",
  "password":"Chetas@11"
}
```
#### To Update Employee
```http
  PUT http://localhost:8080/showFormForUpdate/{id}
```

1.Pass following JSON format in Body of API
```yaml
{ 
  "email":"updated-info", 
  "first_name":"updated-info",
  "last_name":"updated-info",
  "password":"updated-info"
}
```

#### To Delete Employee
```http
  DELETE http://localhost:8080//deleteEmployee/{id}
```







## Run Locally

Clone the project

```bash
  git clone https://github.com/chetas1105/BlackCoffer-EMS.git
```

Go to the project directory

```bash
  cd BlackCoffer-EMS/src/main/java/net/javaguides/springboot
```

Run Application

```bash
  mvn spring-boot:run
```

Open Browser

```bash
    lochalhost:8080/
``` 

