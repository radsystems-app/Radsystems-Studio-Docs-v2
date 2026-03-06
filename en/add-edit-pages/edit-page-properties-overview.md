---
title: Edit Page - Properties Overview
description: 
published: true
date: 2026-03-06T08:25:06.356Z
tags: 
editor: markdown
dateCreated: 2026-03-06T08:25:03.233Z
---

# Edit Page - Properties Overview

The **Edit Page** serves as the primary interface for modifying existing records within your application. While it shares many structural similarities with the Add Page, its primary focus is on updating specific data points while maintaining the integrity of the original record. RadSystems Studio provides a specialized set of properties to manage the update lifecycle, ensuring that users can revise information efficiently and accurately.

## Accessing Edit Page Properties

![rs-crud-addpage-properties.webp](/assets/add-edit-properties/rs-crud-addpage-properties.webp)

To configure the behavior and layout of your update forms, follow these steps:

1. **Select Table**: Click on the specific database table in the first column.
    
2. **Select Page**: In the **List of Pages** (second column), click on **Edit Page**.
    
3. **Page Properties**: The configuration panel for the Edit Page will appear in the section below the page list.
    

---

## Edit Page Properties

![rs-crud-editpage-properties.webp](/assets/add-edit-properties/rs-crud-editpage-properties.webp)

The properties for the Edit Page allow you to control the routing, visual structure, and automated responses triggered during a record update.

### 01. Page Design

**RoutePath**: Defines the unique URL endpoint for editing a specific record, typically including a parameter for the record ID (e.g., `invoiceitems/edit`).

**PageTitle**: The heading displayed at the top of the update form, such as **Edit Invoice Item**.

**SubmitButtonText**: Customizes the label on the primary action button to reflect an update action, such as **Update** or **Save Changes**.

**PageCustomValidation**: Provides access to the server-side code editor where you can write custom business logic to validate updated data before it is committed to the database.

**FormLayoutType**: Determines the alignment of labels and inputs. As seen in the configuration, this is often set to **Horizontal** for edit pages to maintain a compact, professional look.

**MessageBeforeUpdate**: An optional text field to display instructions or warnings to the user before they perform the update.

**MessageAfterUpdate**: The success notification shown to the user after the changes are saved (e.g., **Record updated successfully**).

**Master Detail Display**: This toggle determines if related child records should be visible within this specific context.

### 02. Record Events

**Redirect To After Update**: Specifies the destination page the user is sent to once the update is complete, such as returning to the main **invoiceitems** list.

**Mail Action Settings**: Allows you to configure automated email notifications that trigger specifically after an existing record has been modified.