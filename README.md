Introduction
========
**WhiteRabbit-IRIS** is a application that can be used to analyse the structure and contents of a database as preparation for designing an ETL. It provides IRIS connection support and comes with **RabbitInAHat**, an application for interactive design of an ETL to the OMOP Common Data Model with the help of the scan report generated by White Rabbit. 

Original Source: This project is derived from [WhiteRabbit](https://github.com/OHDSI/WhiteRabbit) by OHDSI, available on GitHub.

Features
========
- Can scan databases in **InterSystems IRIS**, SQL Server, Oracle, PostgreSQL, MySQL, MS Access, Amazon RedShift, Google BigQuery, SAS files and CSV files
- The scan report contains information on tables, fields, and frequency distributions of values
- Cutoff on the minimum frequency of values to protect patient privacy
- WhiteRabbit can be run with a graphical user interface or from the command prompt
- Interactive tool (Rabbit in a Hat) for designing the ETL using the scan report as basis
- Rabbit in a Hat generates ETL specification document according to OMOP template

Screenshots
===========
![image](https://github.com/user-attachments/assets/efbd3c8e-0ebc-4564-a289-7aaa9de340b6)

![image](https://github.com/user-attachments/assets/3de311eb-502d-42ba-a8b0-80722e3d69cc)


Technology
============
White Rabbit and Rabbit in a Hat are pure Java applications. Both applications use [Apache's POI Java libraries](http://poi.apache.org/) to read and write Word and Excel files. 
White Rabbit uses JDBC to connect to the respective databases.

Intended use
============
Whte Rabbit and Rabbit In A hat were designed and implemented for use within a secure and trusted environment. No efforts have been made to
encrypt or otherwise protect the passwords, parameters and results. This should be kept in mind when deploying these tools.

System Requirements
============
Requires Java 1.8 or higher for running, and read access to the database to be scanned. Java can be downloaded from
<a href="http://www.java.com" target="_blank">http://www.java.com</a>.

Dependencies
============
For the distributable packages, the only requirement is Java 8. For building the package, Java 17+ and Maven are needed.

Getting Started
===============
WhiteRabbit-IRIS

1. Download `WhiteRabbit*.zip` 
2. Unzip the download
3. Double-click on `bin/whiteRabbit.bat` on Windows to start White Rabbit, and `bin/whiteRabbit` on macOS and Linux.

(See [the documentation](http://ohdsi.github.io/WhiteRabbit/WhiteRabbit.html#running-from-the-command-line) for details on how to run from the command prompt instead)

Rabbit-In-A-Hat

1. Using the files downloaded for WhiteRabbit, double-click on `bin/rabbitInAHat.bat` to start Rabbit-In-A-Hat on Windows, and `bin/rabbitInAHat` on macOS and Linux.


License
=======
WhiteRabbit is licensed under Apache License 2.0

