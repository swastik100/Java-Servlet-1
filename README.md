# Java-Servlet File

This repository demonstrate how to run Apache Tomcat Server on linux:

Steps are:

1. Download Apache Tomcat from https://tomcat.apache.org/download-80.cgi
2. Make xyz folder in apache-tomcat/webapps
3. Change permission on bin of sh files to allow execting program.
4. Open terminal and start server by running sh startup.sh in terminal. Check in web-browser
   by visiting localhost:8080, which starts the Apache-TomCat Server.  
5. From bin extract servlet.tar file  to location where you put your java file (in xyz folder).
6. Compile java file and paste it's class file in webapps/examples/web-inf/classes.
7. Update xml file(/webapps/examples/web-inf) by adding:
     ``` <servlet>
      <servlet-name>balia</servlet-name>
      <servlet-class>myClass</servlet-class> 
      
    </servlet>
    <servlet-mapping>
      <servlet-name>balia</servlet-name>
      <url-pattern>/bc</url-pattern> <!-- add the url pattern to form action--->
    </servlet-mapping> ``` 
    
8. Restart the server if reqired.
9. Enter http://localhost:8080/xyz/add.html to run the servlet.

