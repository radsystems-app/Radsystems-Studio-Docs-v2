---
title: Built-in Database Manager
description: 
published: true
date: 2026-03-04T08:52:17.981Z
tags: 
editor: markdown
dateCreated: 2026-03-04T08:52:15.378Z
---


# Internal Database Manager

![rs-database-managedb.webp](/assets/manage-database/rs-database-managedb.webp)

While RadSystems Studio works seamlessly with existing databases, it also features a built-in **Internal Database Manager**. This tool provides a streamlined environment for performing essential schema modifications directly within the application, eliminating the need to switch to external management tools for routine tasks.

The interface is designed for rapid prototyping and schema adjustments, organized into a sidebar for table selection and a primary workspace for field configuration.

## Table Management Toolbar

Located at the top left of the window, these controls allow you to manage the high-level entities in your database:

- **Add Table**: Click this to initialize a brand-new table in your database.
    
- **Duplicate Table**: This feature allows you to clone an existing table structure, which is useful when creating audit tables or similar data entities.
    
- **Drop Table**: Use this to permanently delete a table from your database.
    
- **Table Name Editor**: When a table is selected, you can modify its name directly in the "Table Name" input field.
    

## Field Configuration Workspace

The central grid is where you define the specific attributes for each column in your selected table.

### Column Definition Attributes

- **FieldName**: Define the name of the database column (e.g., **userid**, **first_name**).
    
- **FieldType**: A dropdown menu to select the data format, such as **INT**, **VARCHAR**, **TEXT**, or **TIMESTAMP**.
    
- **DefaultValue**: Specify a standard value if none is provided during record creation (e.g., **1** or **CURRENT_TIMESTAMP**).
    
- **Size**: Set the character limit or numerical precision for the field (e.g., **11** for standard integers or **255** for emails).
    
- **Null**: Check this box if the field should be allowed to contain empty (NULL) values.
    
- **AutoInc**: Enabling this allows the database to automatically increment the numerical value for every new record, which is standard for primary keys.
    
- **KeyType**: Define the index level for the field, such as **PRIMARY** for unique identifiers or **UNIQUE** to prevent duplicate entries in fields like usernames or emails.
    

### Field Modification Tools

- **Add Field**: Click the icon above the grid to insert a new column into the current table.
    
- **Drop Field**: Use this to remove a selected column from the table structure.
    

## Finalizing Schema Changes

- **Save Changes**: Once you have finished modifying your tables or fields, click the **Save Changes** button. RadSystems Studio will execute the necessary SQL commands (CREATE, ALTER, or DROP) to update your physical database schema.
    
- **Close**: Exits the manager without saving any pending modifications.
    

> [!TIP]
> 
> **Pro Tip**: While this tool is excellent for quick adjustments, it is recommended to use advanced tools like **PHPMyAdmin**, **DBeaver**, or **Navicat** for complex database operations like managing foreign key constraints or advanced indexing.
