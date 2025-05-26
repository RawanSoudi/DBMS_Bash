# DBMS_Bash
# Overview
This project implements a simple Database Management System (DBMS) using Bash scripting. It provides basic database operations including creating, listing, connecting to, and dropping databases, as well as table operations within each database.

# Features
Database Operations
  Create Database
  
  Validates database name according to strict rules
  
  Creates a new directory for the database

List Databases

  Shows all available databases
  
  Handles cases when no databases exist
  
  Connect to Database
  
  Changes context to the selected database
  
  Presents table operations menu

Drop Database

  Removes a database directory and all its contents
  
  Includes permission validation

# Table Operations (after connecting to a database)
  Create Table
  
  Validates table name and structure
  
  Creates metadata and data files
  
  List Tables
  
  Displays all tables in the current database
  
  Drop Table
  
  Removes a table and its data
  
  Insert into Table
  
  Adds new records with data validation

Select From Table

  Retrieves data with optional conditions
  
  Supports basic filtering
  
  Delete From Table
  
  Removes records with optional conditions

Update Table

  Modifies existing records with validation

# Validations Implemented

Database Validations

  Name cannot be empty
  
  No spaces allowed in name
  
  Only letters, numbers, and underscores allowed
  
  Cannot start with a number
  
  Avoids reserved SQL keywords
  
  Ensures unique name
  
  Validates name length

Table Validations

  Similar naming rules as databases
  
  Column definition validation
  
  Data type checking
  
  Primary key constraints

  Null/Not null constraints

# Data Validations

  Type checking for inserts/updates
  
  Constraint enforcement
  
  Conditional operation validation

# File Structure

Each database is represented as a directory

Tables is stored as:

Separate files (one for data, one for metadata)

Uses relative paths for portability
