# Student Directory Table

## Introduction
- This is a simple exercise in Makers Module 3 - Databases
- I used this project to learn how to design and create a schema with a single table.
- `student_directory_recipe.md` documents my design of the student_directory table
  
## Objectives
- [x] Design a single table schema from these user stories.
  - [x] As a coach  
        So I can get to know all students  
        I want to see a list of students' names.
  - [x] As a coach  
        So I can get to know all students  
        I want to see a list of students' cohorts.

## Setup
This project was made with postgreSQL database software. Here's how to install it:
```shell
# Install postgresql (use latest version)
$ brew install postgresql@15

# Make sure the installation directory is on your PATH environment variable
echo 'export PATH="/opt/homebrew/opt/postgresql@15/bin:$PATH"' >> ~/.zshrc
```
Here's how to run this project:
```shell
# Clone the repository to your local machine
; git clone https://github.com/NatalieJClark/student-directory-table.git YOUR_PROJECT_NAME

# Create the database
createdb student_directory;

# Create the table by running the SQL table file with psql.
psql -h 127.0.0.1 student_directory < students_table.sql

# Navigate to the student_directory database with psql
psql -h 127.0.0.1 student_directory

# View the created table with psql
SELECT * FROM students;
```
