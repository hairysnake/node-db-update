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
* Asynchronous scripts execution
  * long running data migrations
  * big index creation
* Data loading from files (bulk loading where available)
* Migration files verification (before final execution)
  * Errors
  * Advices - no primary key, possbile foreign key (one can apply advices automatically)
* Schema and environments management
* Different formats of scripts : json/xml/plain text
* Statistics - execution time for all scripts and their commands
* Logging - execution logging to standard io / log files
* It prevents concurrent migration execution (optymistic locking on the level of database)
* Custom attributes (ex. service or monolith app version)
* Script execution avoiding on selected environments
* Execution chain / changeset (few scripts that should be treat and execute toogether - ex. from one feature branch) 

### Technology stack

* Typescript
* Nodejs
