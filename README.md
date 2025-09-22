# Coffee List SQL Project

## Table of Contents
- [Project Overview](#project-overview)  
- [Technology Stack](#technology-stack)  
- [Project Structure](#project-structure)  
- [Installation and Setup](#installation-and-setup)  
- [Features](#features)  
- [Model Implementation](#model-implementation)  
- [Controller Implementation](#controller-implementation)  
- [View Implementation](#view-implementation)  
- [Styling and Design](#styling-and-design)  
- [Running the Application](#running-the-application)  
- [Disclaimer](#disclaimer)  

## Project Overview
This project implements a database for tracking coffees, 
stores, and stock availability. The solution file includes 
creation of tables, insertion of sample data, table alteration, 
updates, and example queries.

## Technology Stack
- Database: Microsoft SQL Server (T-SQL)  
- Tool: SQL Server Management Studio (or comparable)  

## Project Structure
```
coffee-list-sql/
├── solution.sql         # Full SQL implementation (schema, data, queries)
└── README.md            # Project documentation
````

## Installation and Setup
1. Clone the repository:  
```bash
   git clone https://github.com/HChristopherNaoyuki/coffee-list-sql.git
```

2. Open `solution.sql` in SQL Server Management Studio.
3. Execute the script step by step:

   * Create the database and tables.
   * Insert data.
   * Alter tables.
   * Run updates.
   * Execute the queries.

## Features

* Database creation of `COFFEELIST`.
* Tables: **COFFEE**, **STORES**, **AVAILABILITY** with primary and foreign keys.
* Populated with sample data for coffees and stores.
* Alteration of table to add `STOCK_ORDERED` column.
* Update operation setting `STOCK_ORDERED`.
* Queries to find coffees with no availability, total stock per coffee, and which store has most stock for a specific coffee code.

## Model Implementation

The data model includes:

* **COFFEE**: stores coffee codes, names, brands, strength, and price.
* **STORES**: stores store codes, names, addresses, and city.
* **AVAILABILITY**: linking coffees and stores, holds stock and order information.
* Foreign key constraints ensure referential integrity between tables.

## Controller Implementation

SQL statements in `solution.sql` serve as controller logic:

* DDL (CREATE, ALTER) define schema.
* DML (INSERT, UPDATE) manage data.
* Constraints enforce data rules.

## View Implementation

The view-like outputs are produced by queries in `solution.sql`:

* Coffees not available in any store.
* Total available stock per coffee.
* Store that has the highest stock for a particular coffee code.

## Styling and Design

* SQL keywords are uppercase for readability.
* Consistent indentation.
* Clear table and column naming.
* Inline comments for sections (e.g., `-- Question 1.1`, `-- Question 2.2`) to separate logical parts.

## Running the Application

* Use SQL Server Management Studio or any SQL client connected to SQL Server.
* Load `solution.sql`.
* Run in sequence: database creation → table definitions → insert data → alter and update → queries.
* Check results in query output panels.

## Disclaimer

This project is for academic or demonstration purposes. 
It does not include production-level security, performance 
tuning, or error handling. Use with caution in live environments.

---
