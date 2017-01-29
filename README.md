This assumes you have both Maven and Tomcat installed
on your machine.

Clone the repo. Change directories into the root directory
where the POM is. Run 

mvn clean install 

to create the war (web archive) file in the target/ directory.
Copy and rename this war file into your Tomcat directory in 
webapps/ROOT/ROOT.war 

Depending on where you have Tomcat installed, this command
may look something like this:
cp target/\*.war /usr/local/Tomcat/webapps/ROOT/ROOT.war

You may have to delete or move any other files in the ROOT
directory prior to moving your code in.

Start Catalina with /usr/local/Tomcat/bin/startup.sh

and then point your browser to localhost:8080 if you're 
running this locally.
