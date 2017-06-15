# Java-Web-Component-Dev-Guide

This repository features basic guide to Java Web Component Development using Apache Tomcat Ver8 and Eclipse

===============================================SETUP==========================================================================
Steps(for Mac/Linux Users):

i)    Download JDK of appropriate version and set up Java Environment
ii)   Download latest version of Eclipse (Code Editor)
iii)  Download Apache Tomcat. Here, Apache is the server and Tomcat is server container
iv)   Go to the downloaded Tomcat folder -> conf -> tomcat-users.xml -> add user using "<user username="--any--"                    
      password="--any--" roles="manager-gui" />" within <tomcat-users> tag
v)    Go to Terminal and using "cd" command move to Tomcat folder and then to bin directory
vi)   Using "./" command run startup.sh which will start your server 
vii)  Type localhost:8080 on your web browser, if this doesn't work then go to:
      Tomcat folder -> conf -> server.xml -> Change the port no. to "9090"(for eg.) under the "<Connector>" tag with protocol
      "HTTP/1.1" which finally looks like:
      " <Connector port="9090" protocol="HTTP/1.1" connectionTimeout="20000 redirectPort="8443" /> "
viii) Restart the server and type localhost:9090 on the browser
ix)   Go to Manager app and login
x)    If you successfully login, then you are done with your set up...

=======================================Basic folder Structure=================================================================

bin :     imp files : startup.sh and shutdown.sh 
          use : to start up and shutdown server manually
      
conf :    imp files : tomcat-users.xml server.xml and web.xml
          use : configuration related files
          
lib :     imp files : servlet.jar and jsp.jar
          use : jars(Java Archive similar to zip files) to be used in our webapps
          
webapps : Place where all webapps are deployed manually

=====================================Using Eclipse for Java WCD===============================================================

i)   Configure your server on Eclipse : Eclipse -> Preferneces -> Server -> Run Time Envr. -> Add 
ii)  File -> New -> Dynamic Web Project -> Name It and Click Ok
iii) Go to the Project created and Go to properties -> In Java Build Path 

      
