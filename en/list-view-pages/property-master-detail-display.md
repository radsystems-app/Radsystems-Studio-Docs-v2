---
title: Master-Detail Display Property
description: 
published: true
date: 2026-03-05T06:16:36.656Z
tags: 
editor: markdown
dateCreated: 2026-03-05T06:16:33.811Z
---

# Master-Detail Display Settings

![rs-crud-listpage-masterdetaildisplay.webp](/assets/list-view-properties/rs-crud-listpage-masterdetaildisplay.webp)

The **Master-Detail Display** property allows you to integrate child record views directly within your master data list. This feature is essential for providing immediate context to your users, such as showing "Invoice Items" directly inside an "Invoices" list without forcing the user to navigate away from the main page.

> For this feature to function, you must have a valid relationship established in the **Master-Detail Relationship** panel. RadSystems Studio relies on these predefined Primary Key and Foreign Key links to fetch the correct related data.

---

## Configuration Interface

The **Master Detail Display Setting** dialog provides granular control over how these nested records appear and behave.

### 01. Detail Page Display

These settings define the logic and visual appearance of the embedded child records.

- **IncludeDetailPage**: Set this to **True** to activate the nested detail view on your list page.
    
- **PageDisplayMode**: Defines how the detail content is revealed. Options include:
    
    - **InPage**: Expands the detail records directly below the master record section.
        
    - **Modal**: Opens the detail records in a centered pop-up window.
        
    - **Drawer**: Slides the detail records out from the side of the screen.
        
- **DetailButtonPosition**: Determines where the toggle button to show details appears in the table row (**OnLeft**, **OnRight**, or **None**).
    
- **ButtonText**: Allows you to add a text label to the detail toggle button.
    
- **ButtonIcon**: Defines the visual icon used for the detail toggle (default is `icon[more_vert]icon`).
    
- **MasterColumnSize**: Sets the layout width for the master record area.
    
- **DetailColumnSize**: Sets the layout width for the detail record area.
    
- **WrapInCard**: When set to **True**, encapsulates the detail view within a distinct card container for better visual separation.
    
- **WrapperClass**: Allows you to apply custom CSS classes to the detail container. Note that these classes and the column size settings automatically adapt to the **Frontend Framework** (Bootstrap or Quasar) selected for your project.
    

---

## Usage Tip

If you select **InPage** for the `PageDisplayMode`, it is recommended to keep `WrapInCard` enabled. This helps users distinguish between the master row and the nested detail records, especially in complex data sets.
