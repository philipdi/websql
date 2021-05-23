# websql (https://websql.diouri.de/)

## SUPPORTED PLATTFORMS
Congratulations! If you see this page, the hardest part is already done!! Because all you need is a computer, internetaccess and a webbrowser to use this tool. Ok... there is some more requirements you can see below.

If you face any problems during the installation, then please make sure, that your system supports these features:

Because of the possibility to customize nearly everything, I´d to make a decision, what to support, and what not.

#### MongoDB
* MongoDB is supported from Version 4 and above.
* It´s only possible to use the default port (27017)
* Ensure your MongoDB is published to the internet and reachable by the ip address of this service.
#### MySQL

* In this Documentation and in this tool MySQL means MySQL and supported plattforms (e.g. MariaDB is also supported)
* Make sure your MySQL Instance is reachable from the ip address of this service.
* There are no known limitations to ports
#### MSSQL (Microsoft SQL Server)
* Supported SQL Servers are 2014, 2016, 2017 and 2019
* This tool supports on premise installations and azure sql
* A valid certificate is not required
* Only Default Port is supported (1433)
* Make sure the Server is reachable from the ip of this service

If you´re running in any problems, you can open an issue on github.

## Connecting to a MongoDB Server

For connecting to a MongoDB Server choose MongoDB from the Dropdown on Home-Page or "MongoDB Client" on the navigation above.

#### Requirements:
* Enter a valid Hostname or IP - "mongodb://" before or a Portspecification after the Hostname/IP is unsupported!
* If needed you can specify the credentials for the MongoDB Host
* Click on the "Discover" Button at Databases. It will fill the dropdown with all available databases of your MongoDB Host (if you specified the url and credentials correctly)
* Choose a Database from the Dropdown
* Click on the "Discover" Button at Collections. It will fill the dropdown with all collections in the choosen database.
* Now you can enter a query. It had to be in Object-Format - e.g. {"name":"max"}
* Choose what kind of operation you want to perform (e.g. insert, find, delete)
* If check the checkbox the response (if there is one) will displayed in a table. if unchecked it will displayed in JSON Format.
* Finally hit "Send Request"
* See the results below (if there is a response)


## Connecting to a MySQL/MariaDB Server

For connecting to a MySQL or MariaDB Server choose mysql from the Dropdown on Home-Page or "MySQL Client" on the navigation above.

#### Requirements:
* Enter a valid Hostname or IP - if needed you can speficy a port by adding ":%PortNumber%" to the Hostname/IP
* If needed you can specify the credentials for the MySQL/MariaDB Host
* Click on the "Discover" Button at Databases. It will fill the dropdown with all available databases of your MySQL/MariaDB Host (if you specified the url and credentials correctly)
* Choose a Database from the Dropdown
* Now you can enter a query. You can use the default MYSQL Language - e.g. SELECT * FROM Cities WHERE postalcode = "2432"
* If check the checkbox the response (if there is one) will displayed in a table. if unchecked it will displayed in JSON Format.
* Finally hit "Send Request"
* See the results below (if there is a response)

## Connecting to a MSSQL Server

For connecting to a MSSQL or Azure SQL Server choose mssql from the Dropdown on Home-Page or "MSSQL Client" on the navigation above.

#### Requirements:
* Enter a valid Hostname or IP - Specify a custom port is not supported
* If needed you can specify the credentials for the MSSQL Host
* Click on the "Discover" Button at Databases. It will fill the dropdown with all available databases of your MSSQL Host (if you specified the url and credentials correctly)
* Choose a Database from the Dropdown
* Now you can enter a query. You can use the default MSSQL Language
* If check the checkbox the response (if there is one) will displayed in a table. if unchecked it will displayed in JSON Format.
* Finally hit "Send Request"
* See the results below (if there is a response)


## Upcomming Features:
* "Any DB" to AWS S3 Backup
* OracleDB Client
* PostgreSQL Client
* Linking to another Webservice for Remote Scripting (Powershell/SSH/SFTP/etc. from Browser)
