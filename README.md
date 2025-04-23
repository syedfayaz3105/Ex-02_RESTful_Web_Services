# Ex-05_RESTful_Web_Services

## Aim:
To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
Step 1: Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.
![image](https://github.com/AfzaraThagsin/Ex-04_RESTful_Web_Services/assets/127172501/3b2c53b8-0dd5-45f3-a9e4-dd22488e6efd)

Step 2: Right-click on the project name and select New->RESTful Web Services from Patterns.

Step 3: A new window will appear. Select “Simple Root Resource” and click Next.
![image](https://github.com/AfzaraThagsin/Ex-04_RESTful_Web_Services/assets/127172501/8b9ef62c-82a7-4733-b94c-25f3dc5a9081)

Step 4: In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.
![image](https://github.com/AfzaraThagsin/Ex-04_RESTful_Web_Services/assets/127172501/aab0aa19-096e-44f2-997b-2bb9a46bec1d)

Step 5: Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.
![image](https://github.com/AfzaraThagsin/Ex-04_RESTful_Web_Services/assets/127172501/d8c3c728-3d2b-4991-91ee-664fe2a7257c)

Step 6: Alter getHtml() method as shown below.

Step 7: Save your project, clean and build it. Deploy your project.
 
Step 8: To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).
![image](https://github.com/AfzaraThagsin/Ex-04_RESTful_Web_Services/assets/127172501/cf60de3c-6fc9-4310-9186-2f7e9d79585c)

### Client-Side:

Step 1: Create a new Java Web Project. Follow steps 1-5 as in section 1.1.

Step 2: Right-click on the project and select New->RESTful Java Client.

Step 3: A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse. Step 4: Carefully select your RESTful resource (web service) and click OK.
 
 ![image](https://github.com/AfzaraThagsin/Ex-04_RESTful_Web_Services/assets/127172501/69392b1c-9c4d-445a-880b-fe97a780640c)

Step 5: Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.
![image](https://github.com/AfzaraThagsin/Ex-04_RESTful_Web_Services/assets/127172501/01d622d3-12f7-403d-8b50-377cfec58176)

Step 6: An editing tab will open. Alter getHtml() method with the following.
![image](https://github.com/AfzaraThagsin/Ex-04_RESTful_Web_Services/assets/127172501/100a668b-4f71-47c2-bb5e-a454671e4efd)
 
Step 7: Right-click on the Libraries folder under your project and select “Add JAR/Folder”.
![image](https://github.com/AfzaraThagsin/Ex-04_RESTful_Web_Services/assets/127172501/66462b76-62a4-42a3-9db0-237a605aec6a)

Step 8: A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.
 ![image](https://github.com/AfzaraThagsin/Ex-04_RESTful_Web_Services/assets/127172501/a74cb20f-a6e4-43d0-b1e8-7176be82ae16)

Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.

Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.
![image](https://github.com/AfzaraThagsin/Ex-04_RESTful_Web_Services/assets/127172501/e28d0aee-751b-4c96-a007-575b768e48e5)

Step 11: Save the project and build it.
![image](https://github.com/AfzaraThagsin/Ex-04_RESTful_Web_Services/assets/127172501/9876177d-c4ef-46f9-a459-1087d92d30b6)

Step 12: Run the JSP file and you should see the output in a new browser window.

### Client-Side Remote Invocation:

Step 1: Follow steps 1-5 as in Section 2.2

Step 2: In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";

Step 3: Follow steps 6-12 as in Section 2.2

## Result:
 Thus, the RESTful web service program has been successfully created and executed.
