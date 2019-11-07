In this tutorial, we are going to see an example program to learn how to do database CRUD operations using Golang and MySQL. CRUD is an acronym for Create, Read, Update, and Delete. CRUD operations are basic data manipulation for database.

In this example, we are going to create an interface as database front end to handle these operations. We have Employee table containing Employee information like id, name and city. With this table, we have to perform CRUD using MySQL. 

Step 1:Prepare and Import MySQL driver into your project
       sudo go get -u github.com/go-sql-driver/mysql

Step 2: Creating the Employee Table
        //DROP TABLE IF EXISTS `employee`;
	CREATE TABLE `employee` (
  		`id` int(6) unsigned NOT NULL AUTO_INCREMENT,
  		`name` varchar(30) NOT NULL,
  		`city` varchar(30) NOT NULL,
  		PRIMARY KEY (`id`)
	);

Step 3: some change in crud.go 
        1. replace mysql username
        2. replace mysql password
        3. replace database name
        4. if you are created same table name , don't chnage otherwise replace 
           table name according to your table name

Step 4: run Application two diffrent way 
        1. go run crud.go
        
	2. sudo +x crud.go
           ./crud 
         
