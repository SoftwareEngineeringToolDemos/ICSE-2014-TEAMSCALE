==================================================
Instructions to Run Teamscale Demo on this VM
==================================================

Assumptions: 
(i) Teamscale has been downloaded and the teamscale.license has been also put in the same folder where teamscale zip folder is extracted.
(ii) Teamscale server is running and localhost:8080 is open on the browser. 
(iii) Java 1.8 and Eclipse Luna are installed.
(iv) The sample project "spring-petclinic" has been cloned from git and is opened on Eclipse

Following steps need to be done in order to run the teamscale demo.

Step 1:

(a) Open Eclipse
(b) Go to Help-> Eclipse MarketPlace
(c) Find https://marketplace.eclipse.org/content/teamscale-eclipse-plugin.
(d) Click Install, confirm and accept the terms of the license agreement. Click Finish.
(e) Restart Eclipse.
(f) In order to make sure that Teamscale is properly installed, one should be able to see a Teamscale menu entry in 
the main menu bar in Eclipse.


Step 2: Create Project on Teamscale server 

(a) On the login page enter the default admin credentials:
	(i)User: admin
	(ii)Password: admin
(b) Once logged in, click on More menu.
(c) Select Projects from the more menu.
(d) Create a new project.
(e) Give any project name eg; "Demo"
(f) Assuming we are working on a java project, select JAVA (Default) from the analysis profile option.
(g) No need to change "Template for initial Dashboard"
(h) Click on Add Source Code Repository
     (i)   Provide the path of the sample spring-petclinic project in the "Input Directory"
     (ii)  Give any name for the "Repository Identifier"
     (iii) Click on "Create Project"
     
Step 3:

(a) The IDE Requires you to use your IDE Access Key for authentication. 
(b) Go to your user profile (located in the top right menu) in http://localhost:8080/dashboard.html
(c) Click on "IDE Access Key" -> "Generate a New Access Key"
(d) This is used in step 9

Step 4:

(a)Open the Eclipse Window -> Preferences menu and select Teamscale from the list.
(b)Use the "Add" button to add a new Teamscale server 
(c)Fill the dialog with the appropriate values. 
	(i)Name : anyname
	(ii)URL:http://localhost:8080
	(iii)Username:admin
	(iv)IDE Access Key : Use the key from Step 8.
(d) Click "Validate" and then "OK" once everything is successful.
(e) Right click on the petclinic project -> Properties and select Teamscale on the left hand side
(f) Check "Enable Teamscale for this project"
(g) The server name and the project name will match the teamscale server configuration.

Step 5:
(a) Installation is complete.
(b) View Teamscale "findings" by hovering on red bars on the left side of the code in eclipse or going to
localhost:8080 and clicking on "Findings"
