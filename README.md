# COMP3005 Template Code (ver 1.1)
This is the template code for the COMP3005 Database Project.

## Updates (04/03/2024)
Ver 1.0 -> Ver 1.1
- Added some more comments for accurate guidance
- Changed time collection - no longer using the overhead of Python but the SQL "EXPLAIN ANALYZE" computations.

## Contains:
- queries.py
  - This will be the file you will write your queries in **AND** submit.
- dbexport.sql
  - This is an **example** of an exported database.

## Modules and Dependencies:
This code primairly uses the psycopg3 module, installation and documentation is listed in this [hyperlink.](https://www.psycopg.org/psycopg3/docs/)
This also only works on a Ubuntu Linux environment, I'd suggest getting a [Virtual Machine](https://carleton.ca/scs/tech-support/virtual-machines/) to accomplish this. Aim for a Ubuntu 22.04 Linux Environment.

## How Does This Work?
Your task is to ONLY write your SQL queries within the prompted space within each Q_# method (where # is the question number).

## How to Test for Yourself:
This script will first connect to an initial database, named by the global variable "initial_database" - please do **NOT** change this name. You should create a database named "project_database" for testing, with the password, user, port and host are also the same as the ones listed in the code.
Throughout running the script, the connection is dropped from the initial database, named as variable "initial_database" and then reconnected to an exported database, named as variable "export_database_name". 

After you set these up and write your queries for each question, you can run the script which will both print the time taken (secs) and create your .csv files. 

The other prints before the execution times are printed are from the dump files, which can be ignored.

### Warnings
For the initial database, please create your own database with the same name. Otherwise, your submission will be **void**.
For the exported database, it is recommended to leave as is but you can rename with no issue. Although it would be easier to leave it unmodified.

## What to Submit?
Your source code file(s) that maps and loads the existing JSON dataset from the JSON files into your database. This code must be stored in a directory named "json_loader".
Therefore, in your submission repository, you are ***only*** submitting the template script "queries.py", *your* dbexport.sql, and this directory. Any additional submissions will ***void*** the ***entire submission.***

  - What will VOID your submission?
    - Any additional submissions in your repository.
    - OTHER Print statements.
    - Changing the name of the databases names, passwords, users, ports, etc.
    - Other alterations to code other than the query executions (please view ACADEMIC INTEGRITY below).

## Bugs or Issues?
If you run into any issues or bugs, please notify me in the [Repository Issues Tab.](https://github.com/gabrielmartell/COMP3305-Project-Template/issues)

# ACADEMIC INTEGRITY
Any alterations to the code, such as modifying the time, will be flagged for suspicion of cheating - and thus will be reviewed by the staff and, if need be, the Dean.
To review the Integrity Violation Attributes of Carleton University, please view https://carleton.ca/registrar/academic-integrity/ 
