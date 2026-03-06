---
title: Managing Page Fields
description: 
published: true
date: 2026-03-05T16:42:48.051Z
tags: 
editor: markdown
dateCreated: 2026-03-04T10:40:24.914Z
---

# Managing Page Fields

![rs-crud-pagefields.webp](/assets/manage-page-fields/rs-crud-pagefields.webp)

The true flexibility of RadSystems Studio is found in its ability to fine-tune data at the field level. Once you select a specific page from the Page List (such as a List Page or Add Page), the **Page Fields** column dynamically populates with every available field from your primary database table and any joined tables.

This interface acts as the control center for your data's visibility and behavior. Selecting a field from this list will load its specific attributes into the **Field Properties** panel on the right. It is important to note that these properties are context-aware; for example, the properties available for a field on a **List or View Page** will differ significantly from those on an **Add or Edit Page**.

> [!TIP]
> 
> For a deep dive into specific configurations, please refer to the **Page Field Properties** section later in this document.

## User Interface Layout

The Page Fields column is designed for rapid configuration with global toggles and individual record controls.

### Navigation and Side Toolbar

![rs-crud-toolbar.webp](/assets/manage-page-fields/rs-crud-toolbar.webp)

To the left of the field list, a vertical toolbar provides essential management tools:

The vertical toolbar contains several buttons to manage both native database fields and user-defined custom fields:

- **Reorder Arrows (Up/Down)**: Use these to physically change the display order of the fields on your page. This determines the sequence of columns in a list or the order of inputs in a form.
    
- **Add Custom Field (Green Plus Button)**: This allows you to insert a new, non-database field into **List** or **View** pages. You can choose between two types:
    
    - **SQL**: Used for performing server-side calculations or subqueries.
        
    - **Template**: Used for adding custom HTML, buttons, or display logic (like the "Archive" button example). _Please refer to the **List/View Page Custom Field** section for more details on these types._
        
- **Edit Custom Field (Blue Pen Button)**: Select a previously created custom field and click this button to modify its SQL logic or HTML template.
    
- **Delete Custom Field (Red Cross Button)**: Permanently removes the selected custom field from the page.
    

### Global Header Controls

![rs-crud-pagefields-header.webp](/assets/manage-page-fields/rs-crud-pagefields-header.webp)

The header row allows you to apply settings to the entire page at once:

- **Output Toggle (First Checkbox)**: Clicking this top-left checkbox allows you to globally check or uncheck the "Output" state for all fields in the list.
    
- **Search Checkbox**: This master setting determines whether the **Search** functionality is enabled for this specific page.
    
## Field List Columns

![rs-crud-pagefields-listconfig.webp](/assets/manage-page-fields/rs-crud-pagefields-listconfig.webp)

Each field in the list features two primary checkboxes that define its role in the application:

- **Output Checkbox**: This determines whether the field is included in the generated SQL `SELECT` query.
    
    - **Note**: You may choose to include a field in the query (keep it checked) but still hide it from the user interface. This is done by modifying the **Display Type** in the Field Properties panel. Refer to the specific page field properties section for more details on hiding fields.
        
- **Searchable Checkbox**: This column specifies whether a particular field should be included in the application's search logic. If checked, the system will look for user-provided keywords within this database column.