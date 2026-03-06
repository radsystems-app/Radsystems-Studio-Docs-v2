---
title: Master Detail Display on Edit Page
description: 
published: true
date: 2026-03-06T08:26:22.621Z
tags: 
editor: markdown
dateCreated: 2026-03-06T08:26:19.862Z
---

# Master Detail Display on Edit Page

![rs-crud-editpage-masterdetaildisplay.webp](/assets/add-edit-properties/rs-crud-editpage-masterdetaildisplay.webp)

In RadSystems Studio, you can enhance the data management experience by displaying related child records directly on the **Edit Page** of a master record. This feature allows users to view contextually relevant details, such as a list of invoice items, while they are updating the primary invoice record.

The **Master Detail Display** property enables a read-only list of records from a related child table to appear within the edit form. It is important to note that this functionality relies entirely on the **Master Detail Relation** being correctly configured in the relations panel.

> [!NOTE]
> 
> Currently, RadSystems Studio supports displaying these detail records as a list for reference; however, it does not support bulk editing of child records directly on the master record's edit page at this time.

### Configuration Settings

The **Master Detail Display Setting** dialog provides several options to control the layout and visibility of the nested detail list:

**IncludeDetailPage**: The primary toggle to enable or disable the display of the details list on the edit page.

**MasterColumnSize**: Defines the grid width allocated to the master form section using standard framework layout classes (e.g., `col`).

**DetailColumnSize**: Sets the width of the details list section, typically set to `col-12` to span the full width of the container below the master form.

**WrapInCard**: When set to **True**, the detail list will be enclosed within a visual card component to match the styling of the main form.

**WrapperClass**: Allows you to apply custom CSS or framework-specific utility classes (e.g., `q-my-md` for vertical margins) to the container holding the details list.
