---
title: Export Settings
description: 
published: true
date: 2026-03-05T06:21:19.146Z
tags: 
editor: markdown
dateCreated: 2026-03-05T06:21:16.479Z
---

# Export Settings Configuration

![rs-crud-listpage-exportsettings.webp](/assets/list-view-properties/rs-crud-listpage-exportsettings.webp)

RadSystems Studio provides robust data portability options, allowing your users to generate professional reports directly from the application. The software supports a wide range of document types, including **PDF**, **Excel**, **CSV**, and **Print** formats, ensuring that your data can be shared and analyzed across different platforms.

The **Export Settings** dialog, accessed through the **ExportSetting** property in the List Page Properties, is where you define the behavior and visual style of the data export feature.

## Page

**Enable Export**: Set this to **True** to activate the export functionality for the current list page.

**ButtonText**: Define the label text for the export trigger on your page (e.g., **Export Data**).

## Export Settings

**ExportFields**: 

![rs-crud-listpage-exportsettings-exportfields.webp](/assets/list-view-properties/rs-crud-listpage-exportsettings-exportfields.webp)

This critical property allows you to select exactly which columns should be included in the exported document. Clicking the button opens a dedicated window where you can check or uncheck fields from the list. This is useful for excluding internal database IDs or action buttons from a printed report. 

For each field, you can set the "Header Label" to be used as the column header and define the template for the field to render as in the exported report.

**ReportTitle**: Enter the title that will appear at the top of your exported document (e.g., **Monthly Sales Report**).

## Export Format

**PRINT**: Enable this to allow users to send the data directly to their local printer.

**PDF**: Enable this to generate a portable document file.

**EXCEL**: Enable this to export data into a spreadsheet format compatible with Microsoft Excel.

**CSV**: Enable this for a raw comma-separated values file, ideal for data migration.

## Button Design

**Icon**: Choose a visual icon for the export button (e.g., `icon[print]icon`).

**Back Color**: Set the background color of the button based on your project's theme (e.g., **primary**).

**TextColor**: Define the color of the button text or icon.

**Outline / Glossy / Unelevated / Push / Flat**: These toggles adjust the physical appearance and interaction style of the button.

## Template Attribute

**TagAttributes**: This allows you to add custom attributes directly to the export button's HTML tag. The values and properties used here are highly dependent on the **Frontend Framework** (such as Bootstrap or Quasar) selected for your project.
