# _BugLister_

#### _C# ASP.NET MCV w/ MySQL Project for Epicodus, October 7th, 2020_

#### By _**Mike Manchee, Daniel Schaaf, and William Donovan-Seid**_

## Description



<!-- Brainstorming

 -->
### Specs
| Spec | Input | Output |
| :-------------     | :------------- | :------------- |
|  1.  Create Issues and Language Classes | ... | ... |
|  1.  Build Issue Controllers for Index, Create, Delete, Details, Edit, and Search | ... | ... |
|  1.  Build Language Controllers for Index, Create, Delete, Details, and Edit | ... | ... |
|  1.  Build Home Controllers for Index | ... | ... |
|  1.  Build Home Views for Index | ... | ... |
|  1.  Build Issue Views for Index, Create, Delete, Details, Edit, and Search | ... | ... |
|  1.  Build Language Views for Index, Create, Delete, Details, and Edit | ... | ... |
|  1.  Create Issues and Language Classes | ... | ... |


## Setup/Installation Requirements

### Project from GitHub
* Download option
  * Download files from GitHub repository by click Code and Download Zip
  * Extract files into a single directory 
  * Run GitBASH in directory
  * Type "dotnet restore" to get bin and obj files
  * Type "dotnet run" in GitBash to run the program
  * Have fun with BugLister <!-- TITLE HERE -->

* Cloning options
  * For cloning please use the following GitHub [tutorial](https://docs.github.com/en/enterprise/2.16/user/github/creating-cloning-and-archiving-repositories/cloning-a-repository)
  * Place files into a single directory 
  * Run GitBASH in directory
  * Type "dotnet restore" to get bin and obj files
  * Type "dotnet run" in GitBash to run the program
  * Have fun with BugLister <!-- TITLE HERE -->

### Database Setup
* Setup with SQL statements 
  * Enter the following code into your SQL database and run.
    ``` SQL
      CREATE DATABASE `buglister` /*!40100 DEFAULT CHARACTER SET utf8mb4 COLLATE utf8mb4_0900_ai_ci */ /*!80016 DEFAULT ENCRYPTION='N' */;
      USE 'buglister';
      CREATE TABLE `issues` (
        `IssueId` int NOT NULL AUTO_INCREMENT,
        `Title` varchar(255) DEFAULT NULL,
        `Type` varchar(255) DEFAULT NULL,
        `Description` varchar(255) DEFAULT NULL,
        `Solution` varchar(255) DEFAULT NULL,
        `LanguageId` int DEFAULT '0',
        `Link1` varchar(255) DEFAULT NULL,
        `Link2` varchar(255) DEFAULT NULL,
        `Link3` varchar(255) DEFAULT NULL,
        `ProjectId` int DEFAULT '0',
        PRIMARY KEY (`IssueId`)
      ) ENGINE=InnoDB AUTO_INCREMENT=11 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;
      CREATE TABLE `languages` (
        `LanguageId` int NOT NULL AUTO_INCREMENT,
        `LanguageName` varchar(255) DEFAULT NULL,
        `DocLink` varchar(255) DEFAULT NULL,
        PRIMARY KEY (`LanguageId`)
      ) ENGINE=InnoDB AUTO_INCREMENT=13 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;
      CREATE TABLE `projects` (
        `ProjectId` int NOT NULL AUTO_INCREMENT,
        `ProjectName` varchar(255) DEFAULT NULL,
        `Description` varchar(255) DEFAULT NULL,
        `Link` varchar(255) DEFAULT NULL,
        PRIMARY KEY (`ProjectId`)
      ) ENGINE=InnoDB AUTO_INCREMENT=2 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;
      ```
  * Go to appsettings.json and change the password if needed.

* Setup with SQL Import
  * MySQL
    * In the Navigator > Administration window, select Data Import/Restore.
    * In Import Options select Import from Self-Contained File.
    * Navigate to the file.
    * Under Default Schema to be Imported To, select the New button.
      * Enter 'buglister' as the name of your database.
      * Click Ok.
    * Click Start Import.
  * Go to appsettings.json and change the password if needed.

## Known Bugs

No Known Bugs

## Technologies Used

Main Programs
* MySQL
* C# / ASP.NET
* MCV
* MSTest
* CSS
  * Bootstrap


### Other Links
[Mike's GitHub](https://github.com/mmanchee)
[Will's GitHub](https://github.com/wdonovanseid)

### License

Copyright (c) 2020 **_{Mike Manchee, Daniel Schaaf, and William Donovan-Seid}_**
Licensed under MIT

co-authored-by: William Donovan-Seid <wdstwo@live.com>
Co-authored-by: Daniel Schaaf <daniel.schaaf@outlook.com>"