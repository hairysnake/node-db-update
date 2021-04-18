# node-db-update
Database migration tool for node projects

### Central tents of the concept :

* Easy to understand and use
* Almost no up-front cost
* General and detailed documentation available describing all the necessary commands 
* Every developer can make changes in the database without deep knowledge of sql commands (json -> sql transformation) and datatypes (types mapping)
* Advanced user is not limited (possibility to write native queries)
* Tools that help to generate files and commands (part of script)

### Main features :

* All types of commands available : DML, DDL, DCL
* Script or scripts reversal
* Asynchronous scripts execution
  * long running data migrations
  * big index creation
* Data loading from files (bulk loading where available)
* Migration files verification (before execution)
  * Errors
  * Advices - no primary key, possbile foreign key
* Schema and environment management
* Different formats of scripts : json/xml/plain text
* Statistics - execution time for all scripts and their commands
* Logging - execution logging to standard io / ?
