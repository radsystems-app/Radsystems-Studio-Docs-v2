---
title: Add Page - Properties Overview
description: 
published: true
date: 2026-03-06T08:19:50.010Z
tags: 
editor: markdown
dateCreated: 2026-03-06T08:19:45.151Z
---

# Add Page - Properties Overview

While the List and View pages are designed for data consumption, the **Add** and **Edit** pages are the engine of your application's data entry. A well-designed entry form is significant because it ensures ease of use for the end-user while maintaining data integrity. RadSystems Studio offers a comprehensive set of properties that allow you to configure these forms to handle everything from simple inputs to complex multi-table transactions.

## Accessing Add and Edit Page Properties

![rs-crud-addpage-properties.webp](/assets/add-edit-properties/rs-crud-addpage-properties.webp)

The workflow for configuring your data entry forms follows the standard RadSystems Studio navigation pattern as shown in the interface:

1. **Select Table**: Click on the database table in the first column for which you want to create or modify an entry form.
    
2. **Select Page**: In the **List of Pages** (second column), click on **Add Page** or **Edit Page**.
    
3. **Page Properties**: The specific properties for the selected form page will automatically load in the panel below.
    

---

## Add Page Properties

![rs-crud-addpage-properties-list.webp](/assets/add-edit-properties/rs-crud-addpage-properties-list.webp)

The **Add Page** properties allow you to define the behavior, validation, and layout of your new record forms. Note that these settings apply UI classes and logic based on the **Frontend Framework** whilst the Server-side custom code based on the **Backend Framework** selected at the time of project creation.

### Page Design

**PageTitle**: The heading that appears at the top of the form (e.g., **Add Invoice**).

**SubmitButtonText**: Customizes the label on the primary action button (e.g., **Submit** or **Save**).

**PageCustomValidation**: This property allows you to inject custom validation logic to ensure data meets specific business rules before being sent to the server.

**Master Detail Form**: A powerful property that enables the creation of complex forms where a master record and multiple child records (like an invoice and its items) are saved simultaneously in a single transaction.

**FormLayoutType**: The **FormLayoutType** property is a key design setting that determines how your input fields and their corresponding labels are positioned on the screen. Choosing the right layout is essential for creating a user-friendly data entry experience that matches the complexity of your form.

The following options are available to structure your **Add** and **Edit** pages:

- **Horizontal**: This classic layout places the field label to the left and the input control to the right on the same row. It is ideal for desktop views where horizontal space is abundant and helps keep the form height compact.

- **Vertical**: This is the default modern layout where the field label is placed directly above the input control. It is highly recommended for mobile-responsive designs as it ensures that input fields span the full width of the container, making them easier to tap and type in.

- **VerticalNoLabel**: Similar to the Vertical layout, but the field labels are completely hidden. This creates a very clean, minimalist interface. When using this, it is important to provide **Placeholders** within the input fields so users still know what data is required.

- **Inline**: In this mode, multiple fields are placed side-by-side in a single row until the row width is filled. This is perfect for short forms, such as a "Subscribe" or "Quick Search" bar, where you want to minimize the vertical footprint of the page.

- **InlineNoLabel**: This combines the compact nature of the Inline layout with the minimalist look of hidden labels. It is typically used for very simple one-line forms like login or newsletter signups.

- **DynamicTableRow**: This specialized layout renders the form fields as cells within a table row. It is specifically designed for use within **Master Detail Forms** (such as adding multiple items to an invoice), allowing users to add, edit, or remove multiple rows of data dynamically before submitting.
  
  ![rs-crud-addpage-properties-dynamiclayout.webp](/assets/add-edit-properties/rs-crud-addpage-properties-dynamiclayout.webp)
  
  For Dynamic Table Row, two more properties can be set to control how many entries User can add in one go. The **Max Table Row** sets the upper limit whereas the **Min Table Row** sets how many rows to present up front when the dynamic form section is presented to the user.
  
### General

**MessageBeforeAdd**: Allows you to display a custom instruction or notification to the user before they begin filling out the form.

**MessageAfterAdd**: Sets the success message shown to the user after the record is successfully saved (e.g., **Record added successfully**).

### Record Events

**Redirect To After Add**: Defines which page the user should be sent to once the form is submitted (e.g., returning to the **invoices** list page).

**Mail Action Settings**: Opens a separate configuration interface to trigger automated emails (such as notifications or confirmations) immediately after a new record is added.
