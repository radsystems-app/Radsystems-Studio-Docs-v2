---
title: WHERE Condition Property
description: 
published: true
date: 2026-03-05T06:18:54.805Z
tags: 
editor: markdown
dateCreated: 2026-03-05T06:18:52.100Z
---

# Where Condition Configuration

![rs-crud-listpage-where.webp](/assets/list-view-properties/rs-crud-listpage-where.webp)

The **Where** property configuration panel allows you to define custom filtering logic for your page's data set. This interface is crucial for implementing business rules, such as restricting a list to show only "Pending" invoices or filtering records based on the currently logged-in user.

The **Query Condition Statement** dialog provides a code-centric environment to override the default SQL data retrieval logic.

It is vital to understand that the code written in this window is not raw SQL; rather, it depends entirely on the **Backend Framework** (e.g., PHP Laravel, Node.js etc) selected during your project creation. The interface provides a **Sample Statement** at the top to guide you with the correct syntax for your specific framework.

## 01. Field Selection (Right Column)

The right-hand column displays a comprehensive list of all available table fields, including any **Custom Fields** you have added to the page.

- **Double-Click to Insert**: Simply double-click any field in this list, and RadSystems Studio will automatically generate a standard `where` clause for that specific field in the code editor.
    
- **Ease of Use**: This feature ensures you are using the exact field names (aliased or native) that the application expects.
    

## 02. Writing Custom Business Logic

The central code editor allows for complex logical implementations:

- **Multi-Line Code**: You can add any number of code lines or variables above your final condition to prepare data for filtering.
    
- **The "Last Line" Rule**: Ensure that the **last line** of your code block is the actual `where` clause, following the exact syntax demonstrated in the Sample Statement.
    
- **Example (Laravel)**:
    
    PHP
    
    ```
    $user_id = auth()->user()->id;
    where['user_id'] = $user_id;
    ```
    

## 04. System Impact and Safety

Because the code written here **overrides the default SQL query condition**, accuracy is paramount:

- **Syntactical Correctness**: You must ensure your code is bug-free and follows the framework's rules.
    
- **Breakage Warning**: Incorrect syntax or logic in this panel will break the page layout and prevent data from loading in your published application.
    

> Always verify that your variables are defined and your logic accounts for empty or null states to prevent runtime errors on the generated pages.
