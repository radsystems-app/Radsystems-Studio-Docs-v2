---
title: Record Detail Page Property
description: 
published: true
date: 2026-03-05T16:53:23.546Z
tags: 
editor: markdown
dateCreated: 2026-03-05T16:53:21.101Z
---

# Record Detail Page Property

![rs-crud-lvpfields-property-recorddetailpage.webp](/assets/list-view-properties/rs-crud-lvpfields-property-recorddetailpage.webp)

The **Record Detail Page** property is a powerful tool for creating meaningful connections between related data. This property allows you to transform a standard database field (often a foreign key ID) into a descriptive link that navigates the user to a specific details page, such as a **View** or **Edit** page.

For example, instead of displaying a numeric `client_id`, you can configure this property to display the actual `company_name` from the linked table, making the interface much more intuitive for the end-user.

## Configuration Steps

To set up this relationship, you must configure several key settings within the **Update Field Master Detail Page** dialog:

**RelationType**: Defines the database relationship between the tables, such as **OneToOne** or **OneToMany**.

**Detail Table**: Select the related database table that contains the detailed information (e.g., **Clients**).

**Detail Table Field**: Specify the primary key field in the detail table that matches your current field (e.g., **id**).

**DetailPage**: Choose the functional page type to be opened upon clicking, such as the **View** or **Edit** page.

**PageDisplaySettings**: Controls how the detail page is revealed, with options like a **Modal** popup or a **Drawer** or a standard **InPage/Inline** navigation.

**Display Text**: This is where you select the meaningful field to show in the UI. Click to select the desired field from the drop-down showing the list of all fields from the selected Detail Table.

**Icon**: Adds a visual indicator next to the link.