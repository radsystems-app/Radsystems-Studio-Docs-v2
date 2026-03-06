---
title: Database Tables and Views
description: 
published: true
date: 2026-03-04T08:39:04.209Z
tags: 
editor: markdown
dateCreated: 2026-03-04T08:39:00.964Z
---


![rs-database.webp](/assets/manage-database/rs-database.webp)
In RadSystems Studio, the workspace provides a comprehensive overview of your data structure. Once your project is loaded, the Studio automatically scaffolds all your database entities, allowing you to manage your application's foundation directly from the sidebar.

To ensure a seamless experience, you must have your **Localhost Database Engine** (such as MySQL/MariaDB, PostgreSQL, or SQL Server) installed and running in the background. This allows RadSystems Studio to communicate effectively with your data.

# Database Workspace Overview

The sidebar organizes your data into a hierarchical tree view, making it easy to navigate through your tables and views.

![rs-database-toolbar.webp](/assets/manage-database/rs-database-toolbar.webp)
## The Database Toolbar

At the top of the table list, you will find a specialized toolbar containing three essential buttons for managing your data connection and schema:

- **Change Database Connection (Gear Icon)**: This button allows you to modify your database connection settings. You can switch to a different database or update your credentials at any time during the project development phase.
    
- **Internal Database Manager (Database Icon)**: Clicking this opens RadSystems Studio's internal database management window. Here, you can perform administrative tasks such as creating new tables, modifying existing table structures, or managing specific table fields without leaving the Studio.
    
- **Sync Database (Circular Arrow Icon)**: This is a critical tool for maintaining data integrity. If you make changes to your database schema using an external tool (like phpMyAdmin or Navicat), click this button to synchronize those changes. This ensures your RadSystems project stays up-to-date with the actual database structure.
    

## Data Entities

RadSystems Studio categorizes your data into three primary groups:

### Database Tables

This section lists all the physical tables currently residing in your connected database. RadSystems Studio uses these to generate the core CRUD (Create, Read, Update, Delete) functionality of your application. 

If you remove the tickmark of table, RadSystems Studio will skip that table and CRUD pages will not be generated for that table.

### Database Views

These are standard views stored directly within your database engine. They represent saved SQL queries that appear as virtual tables, allowing you to present aggregated or filtered data from multiple tables as a single entity. RadSystems Studio scaffolds these as read-only list pages by default.

### Custom Views

Custom views are unique entities built internally within your RadSystems application. Unlike standard database views, these are specifically designed as **Custom LIST pages**. They allow you to define a custom database query directly in the Studio to list records according to your specific business logic, providing a high degree of flexibility for data presentation.