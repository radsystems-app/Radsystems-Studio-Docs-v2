---
title: Add Custom Field
description: 
published: true
date: 2026-03-05T16:41:56.742Z
tags: 
editor: markdown
dateCreated: 2026-03-05T16:41:52.183Z
---

# Add Custom Field

![rs-crud-listpage-customfield.webp](/assets/list-view-properties/rs-crud-listpage-customfield.webp)

When you need to display information that doesn't exist as a single column in your database, the **Custom Field Editor** allows you to create virtual fields for your **List** and **View** pages. This interface provides a flexible way to concatenate strings, perform calculations, or inject custom HTML layouts directly into your data grids.

The Custom Field interface is a modal dialog that appears when you click the **Green Plus (+)** button in the Page Fields toolbar. It is designed to bridge the gap between raw database data and a polished user interface.

## User Interface Overview

The editor is divided into a source panel and a configuration panel:

- **List of Fields**: The left-most panel displays all available fields from your current table and any joined tables. Double-clicking a field name will automatically insert its correct reference variable into the code editor.
    
- **Field Type Selectors**: At the top, you choose the fundamental logic of your custom field by selecting either **Custom SQL Field** or **Template Field**.
    
- **Code Editor**: The central area features a syntax-highlighted editor with **Undo** and **Redo** capabilities. This is where you write your logic or HTML.
    
- **Finalization**: The **Okay** button saves your custom field, which will then appear in your Page Fields list, allowing you to position it anywhere in your UI.
    

---

## 1. Custom SQL Field

![rs-crud-listpage-customfield-sql.webp](/assets/list-view-properties/rs-crud-listpage-customfield-sql.webp)

The **Custom SQL Field** type allows you to write raw SQL expressions that are executed on the database server. This is the most efficient way to perform data manipulation, such as combining names or calculating totals.

- **Field SQL Expression**: In this mode, you write standard SQL functions.
    
    - _Example_: `CONCAT(clients.company_name, ' (', clients.phone, ')')`
        
    - This logic takes two separate database columns and merges them into a single string for display, such as "ProDesk (555-0123)".
        
- **Field Name Alias**: Since this field doesn't exist in the database, you must provide a unique internal name (e.g., `company_details`).
    
- **Display Label**: Enter the text that will appear as the column header on your List page (e.g., `Company Details`).
    

---

## 2. Template Field

![rs-crud-listpage-customfield-template.webp](/assets/list-view-properties/rs-crud-listpage-customfield-template.webp)

The **Template Field** is a powerful UI-centric option. Instead of database logic, it allows you to write the code specific to the Frontend Framework you've selected for your project and use framework-specific placeholders to create complex, multi-line layouts within a single table cell.

- **Edit Field Code**: You can combine HTML tags with data variables.
    
    - _Example_:
        
        HTML
        
        ```
        <strong>{{ props.row.clients_company_name }}</strong>
        <br>
        {{ props.row.clients_email }}
        <br>
        {{ props.row.clients_phone }}
        ```
        
    - This template renders the company name in bold, followed by the email and phone number on new lines, all within the same column.
        
- **Usage**: This is ideal for creating "Summary" columns, adding custom action buttons, or displaying formatted contact information.
    
- **Display Label**: Just like SQL fields, define the header title that users will see (e.g., `Company Info`).
    
