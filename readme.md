PRE-REQUISITES
-----------------
- netbeans IDE 8.2
- visual studio 2015
- Glass fish server 4.1.1
- mysql

# Please install above software if not available in desktop

************************************************************************************************************************
- Install Mysql
- Create database schema called soa and make it as a default schema 
- Execute the given sql scripts to create table and insert the test data

************************************************************************************************************************

PROCEDURE - STEPS TO IMPORT JAVA PROJECT
----------------------------------------

- Do Datasource connection from netbeans to soa schema with full user priveleges
- Download the project zip folder and Unzip it
- Create a web application project
- Import the project folder in netbeans
- Right click clean & build, start the glassfish server and then right click to deploy
- In the output window of Glassfish server - you can view the message as 'Project deployed successfully'
- In the project folder - you should be able to see the folder webservices; Under webservices you can see the folder truck catalogue and inside that you can see all the webservices.
- Right click on the Truck Catalogue and click on test service --> to test the web services
- Right click generate and copy wsdl to get the wsdl 
- copy the wsdl

***************************************************************************************************************************

PROCEDURE - STEPS TO SETUP THE CLIENT
--------------------------------------

- Open the Asp.net folder provided -> Unzip the TruckWebApp file
- In Visual Studio, On the File menu, point to Open, and then click Project/Solution -> The Open Project dialog box is displayed
- Click Add to Solution 
- Go to the folder that contains the solution file for the solution you want to open. Solution files have the extension .sln. Select this file and then click Open.
- Right click on the reference and click Add service reference --> paste the wsdl in the address bar and click on GO
- It will show you all the webservices - OK
- Under the connected services - you can find TruckWebService (which is part of object part creation)
- Use the code under the .Net folder
- Copy the code along with other ASPX files
- Right click on the project and say build - you will receive a message as build succeeded
- Right click on the project and set as startup project --> Again Right click on the login.ASPX and set as start page
- Use login.ASPX and right click to select weavin browser --> set the browser to internet explorer
- download the attached mysqldate.dll - make sure to verify under bin folder that mysql data dll is present - if not copy from the project folder and paste it in bin folder
- Now you can run the .Net project from internet explorer and from visual studio, you can launch the application

***********************************************************************************************************************************

- Before launching application in the visual studio -- make sure the glassfish server is running and application deployed in netbeans.
- Stop other webservers running on the same port as Glassfish server.

TESTING
--------

- Give the login credentials for testing.
- Give the customer login credentials
	- user name - C101
	- password - 123
	- Use SignUp form for new user creation
	- For existing User, use above credentials to login.
	- Customer landing page -> All customers related services are present. 
	- Click on each link and test. Use Cancel or Home button to get back to previous page.
	- Once testing done, logout

- Admin credentials
	- Username - admin
	- password - admin
	
	- SignUp is not for admin.
	- Login with above details and you can see the admin landing page.
	- Click on each link and test. Use Cancel or Home button to get back to previous page.
	- Once testing done, logout

- Application is running fine in our local servers
- Get back to us for any concerns

**********************************************************************************************************************************
