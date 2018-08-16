# matrix
Final Project Top 25 Collaboration Matrix RIN (Add File Config)  

Minimum Requirement :
- Glassfish 4
- Java JDK 8

### Test Deploying an Application From the Command Line

1.	To download a copy of the 'matrix.war' application.
2.	Save the matrix.war file in the directory of your choice. This directory is referred to as *sample-dir*.
3.	Start Glassfish Server domain before deploy the application. To Start the Default Domain. Run the asadmin start-domain command without an operand: 

    **as-install/bin/asadmin start-domain**

    The command starts the default domain, domain1.

4.	Use the asadmin deploy command. General command is: 

    **as-install/bin/asadmin deploy war-name**

    To deploy the matrix.war sample, the command is:

    **as-install/bin/asadmin deploy sample-dir/matrix.war**

5.	Access the matrix application by typing the following URL in your browser:

    **http://localhost:8080/matrix**
    
6.	The application's start page is displayed.

See Full Documentation Glassfish : [Doc Glassfish 4](https://javaee.github.io/glassfish/doc/4.0/quick-start-guide.pdf).



### Config Database
Configure Script To Connect Database Server in File "config.json" at */matrix/resources/data/config.json*

Example Default Config :

![2018-08-16_00h42_36](https://user-images.githubusercontent.com/42184550/44163344-521b1500-a0ed-11e8-8fe4-0da3583b3b94.png)

- host = "IP database PostgreSQL server"
- port = "port database"
- dbname = "the name of database"
- username = "username to access database"
- password = "password to access database"
- pathjsonfile = "folder location where json file is stored" *(normally it doesn't need to be changed)*
