---
title: Join Tables Property
description: 
published: true
date: 2026-03-05T06:17:49.669Z
tags: 
editor: markdown
dateCreated: 2026-03-05T06:17:46.878Z
---

# Join Tables Configuration

![rs-crud-listpage-join.webp](/assets/list-view-properties/rs-crud-listpage-join.webp)

In RadSystems Studio, the **Join Tables** configuration is an essential tool for creating comprehensive data views by linking multiple database tables. This interface allows you to define relationships so that your **List** or **View** pages can display data from related records simultaneously.

The Join Tables interface is accessed by clicking the **(Collection)** button next to the **Join Tables** property in the List Page Properties panel. The interface is organized into three distinct columns to streamline the process of building complex SQL JOIN statements.

## 1. List of Tables (First Column)

This column displays every table available in your currently connected database.

- **Adding a Table**: To include a table in your query, select its name and click the **Join Table** button, or simply **double-click** the table name. The table will then move into the second column for further configuration.
    

## 2. Selected Tables (Second Column)

This workspace manages the tables you have chosen to include in your join operation.

- **Remove Table Join**: If you decide a table is no longer needed for this specific page, select it in this column and click the **Remove Table Join** button.
    
- **Table Alias**: If you need to use a shorter or more descriptive name for the table within your SQL queries, enter the name in the **Table Alias** text box and click **Change**. This is particularly useful when joining the same table multiple times or dealing with very long database names.
    

## 3. JOIN Settings (Third Column)

The third column is where you define the specific logic for the relationship between the master table and the joined table.

- **Left Field**: Use this dropdown to select the linking field from the primary (master) table (e.g., `invoices.client_id`).
    
- **Right Field**: Use this dropdown to select the corresponding field from the joined table (e.g., `clients.id`).
    
- **Join Type**: Select the mathematical logic for the join:
    
    - **INNER JOIN**: Returns only records that have matching values in both tables.
        
    - **LEFT JOIN**: Returns all records from the left table and matched records from the right table.
        
    - **RIGHT JOIN**: Returns all records from the right table and matched records from the left table.
        
- **Sample SQL Statement Structure**: As you configure these settings, this area provides a live preview of the generated SQL code (e.g., `SELECT * FROM Invoices INNER JOIN Clients ON invoices.client_id=clients.id`). This helps verify that your logic matches your intended database query.
    
## Finalizing the Joins

- **Okay**: Once all relationships are defined, click **Okay** to save the collection. These joined fields will now be available for selection in your **Page Fields** list, allowing you to display them on your application pages.
