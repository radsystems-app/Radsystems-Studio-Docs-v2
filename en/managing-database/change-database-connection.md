---
title: Change Database Connection
description: 
published: true
date: 2026-03-04T08:45:15.533Z
tags: 
editor: markdown
dateCreated: 2026-03-04T08:43:39.337Z
---


# Change Database Connection

![rs-database-connection.webp](/assets/manage-database/rs-database-connection.webp)

The **Change Database Connection** window provides the flexibility to switch your project's data source at any point during development. This is particularly useful when moving from a development database to a staging environment or when your project requirements shift to a new data schema.

## Switching Your Database Connection

When you initiate a change in the database connection, RadSystems Studio establishes a fresh link to the new server or database you specify.

> 
> **Schema Replacement**: Once you successfully switch to a new database, all tables, views, and relationships from the **currently connected** database are removed from the workspace. RadSystems Studio will then automatically load all the tables, views, and structural data from the **newly selected** database into your project.

## Database Server Configuration

To point your project to a new data source, provide the following connection details in the configuration window:

- **Server**: Enter the hostname or IP address of the new database server. For local environments, this remains **localhost**.
    
- **Port**: Specify the communication port for the database engine.
    
    - **Tip**: If your server uses a non-standard port, click the **If Different** link to manually enter the port number.
        
- **User**: Enter the username authorized to access the new database (e.g., **root**).
    
- **Password**: Provide the password for the specified database user.
    
- **Database**: Select the specific database name from the dropdown menu. This list is populated based on the server, user, and password provided above.
    

## Finalizing the Switch

- **Okay**: Click this button to confirm the new connection. RadSystems Studio will validate the credentials, drop the old schema from the workspace, and re-scaffold your project using the entities found in the new database.
