---
title: Action Buttons Property
description: 
published: true
date: 2026-03-05T06:28:37.410Z
tags: 
editor: markdown
dateCreated: 2026-03-05T06:28:34.512Z
---

# Page Action Buttons

![rs-crud-listpage-actionbuttons.webp](/assets/list-view-properties/rs-crud-listpage-actionbuttons.webp)

In RadSystems Studio, **Action Buttons** are the interactive elements provided for each record in a list, allowing users to perform specific operations like viewing, editing, or deleting data. These buttons are automatically generated for each row in a table or as part of the individual cards in other display templates.

The **Page Action Buttons** configuration window allows you to manage the specific actions available for your records and customize their visual presentation.

## Button Management

The left-most panel displays a list of the currently configured buttons for the page (e.g., **invoices/view**, **invoices/edit**). You can manage this list using the sidebar toolbar:

![rs-crud-listpage-actionbuttons-toolbar.webp](/assets/list-view-properties/rs-crud-listpage-actionbuttons-toolbar.webp)

- **Add New Button (Green Plus)**: Click this to initialize a new custom action button for your record rows.
    
- **Remove Button (Red Cross)**: Select an existing action and click this to permanently delete it from the page.
    
- **Reorder Buttons (Up/Down Arrows)**: Use these to change the physical sequence of the buttons as they appear in the application UI.
    

## Component Properties

![rs-crud-listpage-actionbuttons-properties.webp](/assets/list-view-properties/rs-crud-listpage-actionbuttons-properties.webp)

This section defines the functional behavior of the selected action button.

**Include**: A toggle to determine if the selected button should be rendered on the page.

**PageLink**: Defines the destination or action triggered by the button. This can be a defined route to an application page (e.g., `invoices/view`) or a custom **JavaScript function**.

- **JS Function Syntax**: To trigger a JavaScript function, wrap the function call inside double dashes. For example: `--MyFunction--` or `--MyFunction()--` or `--MyFunction(param1, param2)--`.
    

**PageDisplaySettings**: Controls how the linked page or content is revealed to the user. Options include:

- **InPage / InLine**: Navigates to the page or expands content directly.
    
- **Modal**: Opens the content in a centered popup window.
    
- **Drawer**: Slides the content out from the side of the screen.
    

**ButtonText**: The label displayed on the button.

**ButtonTitle**: The tooltip text that appears when a user hovers over the button.

## Button Design

These properties control the visual styling of the button. Note that the specific rendering of these classes depends on the **Frontend Framework** (Bootstrap or Quasar) selected for your project.

**Icon**: Sets the visual symbol for the button (e.g., `icon[visibility]icon`).

**Back Color**: Defines the theme-based background color (e.g., `primary`).

**TextColor**: Sets the color for the icon or label text.

**Outline / Glossy / Unelevated / Push / Flat**: Various toggles to adjust the button's physical appearance, shadow, and interaction feedback.

## Template Attribute

**TagAttributes**: A collection where you can inject custom HTML attributes or framework-specific CSS classes directly into the button component.

---

### Apply to other pages

**Apply Button Design to Other Pages**: Checking this box at the bottom allows you to synchronize the visual style (colors, icons, and shapes) of your action buttons across all other pages in the project.