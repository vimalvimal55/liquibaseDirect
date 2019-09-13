## Welcome to GitHub Pages

1. Download liquibase from  https://download.liquibase.org/ 
2. download zip version of it.
3. install it in D drive
4. unzip the folder 
5. go inside the folder , d:\liquibase-3.8.0-bin
6. place liquibase.properties inside the folder and place my mysql-connector-java-8.0.11.jar inside lib folder.
7. paste following content inside liquibase.properties 

```
    ### Connection Property File For File Based HSQL Database
    ### Example use: ..\..\liquibase --defaultsFile=liquibase.hsql.properties update

    classpath=src
    changeLogFile=src/main/resources/liquibase/changelog/changelog-master.xml
    driver=com.mysql.jdbc.Driver
    username=root
    password=password
    url=jdbc:mysql://localhost:3306/bookdb?useSSL=false
    #logLevel=DEBUG
    #referenceUrl=jdbc:hsqldb:file:tmp/db/hsql/liquibase;shutdown=true
    #referenceUsername=liquibase
    #referencePassword=liquibase
    #contexts=dev,main,prod
   
    
8. If you have access to https://github.com/vimalvimal55/liquibaseTool
9. copy the src folder from there 
10. 9 needs to be done to follow the structures mentioned in changelog path 
11. go to command line mode 
12. run following command 
13. d:\liquibase-3.8.0-bin>liquibase.bat update
14. you will see the result.

# If you want to run against Oracle 
1. you have to change the scripts inside basic folder according to oracle.
2. place oralce jdbc jar inside lib folder 
3. update liquibase properties - url and driver  according to oracle 
4. that's it simple ! .



all above stuffs done with this repository. so , 
download it and run it like  ->  **D:\liquibaseDirect>liquibase.bat update**





