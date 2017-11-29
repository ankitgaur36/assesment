REST API Spring-hibernate based crud opertaion
================================================
CRUD operations using the Spring MVC RESTful web service with Spring security and Hibernate ORM framework.

	
Tools and technologies used for this application are-
**Front-end**
HTML
CSS/JavaScript
Angular Js -  v1.4
Bootstrap v3.3.2

**Java Back-end**
Spring-Security v4.1.1.
Spring MVC v4 - REST
Jackson API v2.7.5
Hibernate v5.2.5
hsqldb v2.3.4    
Java  1.8
log4j v1.2
Maven v3.3.9
Apache Tomcat v9.0



After you have cloned this repository you need to follow the below steps in order to deploy this app,

1) Update the maven dependencies.
2) Clean and install the application using maven and verify test results.
mvn command - mvn clean install 
                   or 
              mvn clean install eclipse:eclipse -Dwtpversion=2.0

3) Launch the HSQLDB server 
4) Find the datasource and details in application.properties
5) Set up Tomcat Server.
6) Deploy the application on server
7) Enjoy it.


 
**USER API Operations & EndPoints**
Basic-Auth credentials you can find the configuration in 
UserName & Password -  admin & admin123 (Admin Role)
                    - uxpsuser & user123 (User Role)


GET	- Retrieve a resource ( equivalent to sql SELECT statement)
EndPoints - http://localhost:8080/assignment/api/user



POST	Create	Create a new resource ( equivalent to sql INSERT statement)
EndPoints - http://localhost:8080/assignment/api/user

Input =>
 {
        "userName": "Joey",
        "password": "Joey123",
        "status": "Activated"
    }

PUT/PATCH	Update	Update or modify a resource ( equivalent to sql UPDATE statement)
EndPoints - http://localhost:8080/assignment/api/user
Input =>
{        "id" : 5,
        "userName": "Joey",
        "password": "Joey123",
        "status": "Deactivated"
    }


DELETE	Delete	Delete a resource ( equivalent to sql DELETE statement)
EndPoints - http://localhost:8080/assignment/api/user/5

Output id - 5 





Regards,
Ankit Gaur.
