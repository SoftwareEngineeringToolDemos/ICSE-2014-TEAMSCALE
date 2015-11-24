This Virtual Box (VM) has all the setup configuration file needed to run and test Eclipse plugin,
Teamscale like (JAVA version 1.8)
Teamscale server requires Oracle Java JDK 1.8 or higher in order to run. 
The Teamscale after being added can be seen on the menu bar on the top of the Eclipse IDE.

Open the project properties (right click project -> Properties). Select the Teamscale menu entry. 
Configure your Teamscale server and project

Should your project's directory structure differ from the structure present on the server, create a mapping:
The Local Prefix is a part of your local directory structure.
The Teamscale Prefix is a part of the project directory structure on the Teamscale server.
Click Add to add a mapping. You can leave one of the entries empty, if you want to remove redundant
parts of the local or server's path.
Press OK

To check if everything is configured correctly, open the Findings View (Window -> Show View -> Other -> Teamscale -> Findings), 
make the Refresh on Selection Changes button is active.

For more details you can visit https://cqse.freshdesk.com/support/solutions/articles/1000063210-installing-the-eclipse-teamscale-plugin

The details about this project, the paper in which the 
plugin was first described and the link to the plugin itself are available at the following github link. 
https://github.com/SoftwareEngineeringToolDemos/ICSE-2014-Teamscale.

Iin order to reinstall the plugin to Eclipse, one can follow the steps that have been provided in 
Installation.txt file present on the Desktop. This plugin has been tested with Eclipse Mars version 
and JAVA 8. If you want to reinstall the entire IDE, please make sure that these requirements are met.
