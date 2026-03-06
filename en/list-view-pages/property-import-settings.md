---
title: Import Settings
description: 
published: true
date: 2026-03-05T06:23:09.480Z
tags: 
editor: markdown
dateCreated: 2026-03-05T06:23:07.025Z
---

# Import Data Settings

![rs-crud-listpage-importsettings.webp](/assets/list-view-properties/rs-crud-listpage-importsettings.webp)

RadSystems Studio provides a streamlined way to enable bulk data entry through its **Import Data** feature. This tool allows your end-users to upload records directly into a database table using a structured CSV file, significantly reducing manual data entry time.

To function correctly, the data to be imported must strictly adhere to specific formatting rules. The CSV file must contain columns in the exact same sequence as they appear in the destination database table. Additionally, the first row of the file must be a header row, where each column header matches the database field name precisely.

When activated, an **Import** button appears at the bottom of the page records. Clicking this button triggers a standard file selection dialog, allowing the user to choose their CSV file. It is important to note that the total processing time for an import request varies based on the number of rows being uploaded and the computing resources available on your hosting environment.

---

## 01. Page

**EnableCSVImport**: This property acts as the master switch to activate or deactivate the import functionality for the current page.

**ButtonText**: Use this field to define the label shown on the import button, such as **Import Data** or **Upload CSV**.

## 02. Button Design

**Icon**: This allows you to select a visual icon to represent the import action, typically a folder or upload icon like `icon[folder]icon`.

**Back Color**: This sets the background color of the button, which will pull from the theme colors of your selected **Frontend Framework**, such as **primary**.

**TextColor**: This property defines the color of the text or icon within the button.

**Outline**: When enabled, the button will have a transparent background with a colored border.

**Glossy**: This applies a subtle gradient effect to the button, giving it a polished, reflective appearance.

**Unelevated**: If set to **True**, the button will appear flat without any drop-shadow effects.

**Push**: This adds a "depressed" visual effect when the user clicks the button, simulating a physical push.

**Flat**: This removes all borders and background colors, leaving only the text and icon.

## 10. Template Attribute

**TagAttributes**: This property allows you to inject custom HTML attributes or CSS classes directly into the button tag. The options available here are highly specific to the **Frontend Framework** (Bootstrap or Quasar) used for your project.
