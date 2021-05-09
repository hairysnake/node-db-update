# node-db-update
Database migration tool for node projects

### Central tents of the concept :

* Easy to understand and use
* Almost no up-front cost (the simplest case - no configuration needed - DATABASE_URL)
* General and detailed documentation available describing all the necessary commands 
* Every developer can make changes in the database without deep knowledge of sql commands (json -> sql transformation) and datatypes (types mapping)
* Advanced user is not limited (possibility to write native queries)
* Tool that help to generate files and commands (part of script)

### Main features :

* The most used types of SQL databases are supported
* All types of commands available : DML, DDL, DCL
* Script or scripts reversal
* Parallel script execution
  * big migration divided into few pieces to make it faster
  * scripts that can be executed together
  * bulk loading of data from external data source
* Asynchronous scripts execution (in background)
  * big index creation (make sure it won't be needed in next scripts)
* Data loading from files (bulk loading where available)
* Migration files verification (before final execution)
  * Errors
  * Advices - no primary key, possbile foreign key (one can apply advices automatically)
* Schema and environments management
* Different formats of scripts : json/xml/yaml
* Statistics - execution time for all scripts and their commands
* Logging - execution logging to standard io / log files
* It prevents concurrent migration execution (optymistic locking on the database level)
* Custom attributes (ex. service or monolith app version)
* Script execution avoiding on selected environments
* Execution chain / changeset (few scripts that should be treated and executed toogether - ex. from one feature branch)
* Simple configuration in json

### Technology stack

* Typescript
* Nodejs

### High level overview

![High level overview of the system](https://github.com/hairysnake/node-db-update/documentation/images/high_level_view.png)
