# Evolent Code Test
This project is devided into to different applications.

Evolent WEB API - An WEB API, developed in ASP.NET Web API 2.0, to perform CRUD operation for contact data. The project evolent.webapi.Tests project under WEB API project has Unit Test for API methods. It has two test cases.

Evolent Web - And application, developed in ASP.NET MVC 5, which consumed the above WEB API which provide an User Interface to perform Create, Update, Delete & List contacts.

Create database as "evolent" and run "Evolent_DBScript.sql" which is located in "DB" folder.

Run these application,

First run the Evolent WEB API project.

Please make sure to change the sql server data source in the below connection string used in the following application,
evolent.data
evolent.webapi
evolent.webapi.Tests
Second run the Evolent Web application project.

As this project internally communicate with above WEB API project, make sure the port number of the above WEB API application running is same as the following app settings in web.config file
For error logging ELMAH is used. To see the logs regarding the WEP API, you can browse the URL "http://localhost:63124/elmah.axd". If the web api project is running on the port 63124. Otherwise adjust the port number accordingly.

For error logging ELMAH is used. To see the logs regarding the MVC application, you can browse the URL "http://localhost:49588/elmah.axd". If the MVC project is running on the port 63124. Otherwise adjust the port number accordingly.
