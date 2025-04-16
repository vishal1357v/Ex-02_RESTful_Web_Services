# Ex-04_RESTful_Web_Services
~~~
Name : VISHAL P
Reg.No : 212224230306
~~~
## Aim:
To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation

## Procedure:

### Server side:
Step 1: Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.

Step 2: Right-click on the project name and select New->RESTful Web Services from Patterns.

![image](https://github.com/Catty12384/Ex-04_RESTful_Web_Services/assets/120629225/97844375-6b29-445e-a6bf-81cb6b1ae863)



Step 3: A new window will appear. Select “Simple Root Resource” and click Next.
 
 
![image](https://github.com/Catty12384/Ex-04_RESTful_Web_Services/assets/120629225/73fe81f7-3551-4730-bfa2-0bc6e6ae3825)


Step 4: In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.

![image](https://github.com/Catty12384/Ex-04_RESTful_Web_Services/assets/120629225/cf1d3c1a-a2f4-43d9-a97d-e6da2bbec095)


Step 5: Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.

Step 6: Alter getHtml() method as shown below.

Step 7: Save your project, clean and build it. Deploy your project.
 

 ![image](https://github.com/Catty12384/Ex-04_RESTful_Web_Services/assets/120629225/ca846318-3767-453f-b6d8-4d1be784e576)



Step 8: To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).



### Client-Side:


Step 1: Create a new Java Web Project. Follow steps 1-5 as in section 1.1.

Step 2: Right-click on the project and select New->RESTful Java Client.

![image](https://github.com/Catty12384/Ex-04_RESTful_Web_Services/assets/120629225/8bcae0e8-da6c-40ce-983c-96e86a1d5be7)



Step 3: A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse. 

Step 4: Carefully select your RESTful resource (web service) and click OK.

![image](https://github.com/Catty12384/Ex-04_RESTful_Web_Services/assets/120629225/a831997b-8440-490c-b152-d9c81354792b)



Step 5: Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.

![image](https://github.com/Catty12384/Ex-04_RESTful_Web_Services/assets/120629225/cc9a2c1e-31b7-4dad-822e-1e045afeb678)


Step 6: An editing tab will open. Alter getHtml() method with the following.
 
![image](https://github.com/Catty12384/Ex-04_RESTful_Web_Services/assets/120629225/45e0eb94-b994-45a9-b623-9b4515ede9c3)
 


Step 7: Right-click on the Libraries folder under your project and select “Add JAR/Folder”.

![image](https://github.com/Catty12384/Ex-04_RESTful_Web_Services/assets/120629225/ecccfccc-0f4c-45a7-8baa-64e8d0e82338)


Step 8: A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.
 
 
![image](https://github.com/Catty12384/Ex-04_RESTful_Web_Services/assets/120629225/f66ca82e-4532-40c4-993c-0d8fcb2eef2a)


Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.

Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.

![image](https://github.com/Catty12384/Ex-04_RESTful_Web_Services/assets/120629225/b9df0d0d-81a4-4342-9402-260e399b0cfd)


Step 11: Save the project and build it.

Step 12: Run the JSP file and you should see the output in a new browser window.
 
![image](https://github.com/Catty12384/Ex-04_RESTful_Web_Services/assets/120629225/0ce14793-daf0-4207-a95e-53534384bac5)
 


### Client-Side Remote Invocation:


Step 1: Follow steps 1-5 as in Section 2.2
Step 2: In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";
Step 3: Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
