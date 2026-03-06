---
title: Global Settings
description: 
published: true
date: 2026-02-16T10:37:29.281Z
tags: 
editor: markdown
dateCreated: 2026-02-16T10:37:26.265Z
---

# Global Settings

![rs-globalsettings.png](/assets/settings/rs-globalsettings.png)

**Global Settings** serves as your master template. By configuring these options, you establish a standard for every new project you create. This eliminates the need to manually repeat setup tasks and ensures that all your applications maintain a consistent look, feel, and functional behavior from the moment they are scaffolded.

While RadSystems Studio provides sensible defaults, you should adjust these to match your preferred development environment and project requirements.

## Default Database Settings

Use this section to pre-configure your local development environment. By setting these, the "Create New Project" screen will automatically be filled with your credentials.

* **Database**: Choose your preferred default engine. Default is set to **MYSQL**.
* **DatabaseHost**: Enter the address where your database resides. The default is **localhost**.
* **DatabaseUsername**: Provide the administrative username for your database. The default is **root**.
* **DatabasePassword**: Enter the password for the database user. Leave this blank if your local root user has no password.
* **DatabasePort**: Specify the port your database server listens on (e.g., 3306 for MySQL).

---

## General Settings

These instructions control the core behavior and initial appearance of your generated web application.

* **SaveProjectFilesRevisions**: Set this to **True** to ensure the Studio saves previous versions of your project files. This allows you to roll back changes if something goes wrong during development.
* **HideLaravelDatabaseTables**: Toggle this to **True** to keep your interface clean. It hides internal Laravel system tables so you only see the tables you created.
* **PHPDateDefaultTimeZone**: Define your preferred time zone (e.g., **UTC**). This ensures all time-stamps in your application are consistent.
* **EnableAppDebug**: Turn this to **True** during development. It allows the application to show detailed error reports, which are essential for troubleshooting your logic.
* **EnableRecordNavigation**: Set this to **True** if you want "Previous" and "Next" buttons to appear when a user is viewing an individual record.
* **ShowPagePreloader**: If your pages contain a lot of data, set this to **True** to show a loading animation while the content is being prepared.
* **DefaultAppTheme**: Choose the base visual style for your apps. The current default is **bootswatches/zephyr.css**.
* **FormFieldValidationRequired**: Set this to **True** to automatically force users to fill in fields that are marked as "Not Null" in your database.
* **ListPageFieldsSortable**: Enable this to allow your end-users to click on table headers to sort the data (A-Z or Z-A).
* **IncludePageFooter**: Toggle this to **True** to automatically include a standard footer area at the bottom of every page in your app.
* **PageSectionContainerClass**: Define the layout width. Use **container-fluid** for a full-width look or **container** for a centered, fixed-width look.
* **QueryLimit**: Set the default number of rows displayed per page. The default is **10**.
* **AddPageSubmitButtonText**: Change this text to customize the button used for creating new records (e.g., **Submit** or **Save**).
* **EnableCaptchaValidation**: If you are worried about spam, set this to **True** to add a Captcha check to your public forms.
* **EditPageSubmitButtonText**: Customize the button label used when a user is saving changes to an existing record (e.g., **Update**).

---

## Page Inline Edit Settings

* **InlineEdit**: If you want to allow users to edit data directly inside the table without opening a new page, set this to **True**.

---

## Page Report

In this section, you decide which export options should be available to your users.

* **WORD, EXCEL, IMAGE, CSV, PDF**: Set any of these to **True** to provide the user with a download button for that specific format on every data list.

---

## Page Settings

These settings dictate how the interactive elements of your pages function.

* **AjaxPage**: Set to **True** if you want your application to load data in the background without refreshing the whole browser page.
* **ListPageDisplayType**: Choose how data is listed. **TabularList** (the default) shows a standard grid.
* **ActionButtonDisplayStyle**: Choose how actions like Edit and Delete appear. **DropDownButtons** keep the interface clean by hiding actions under a single button.
* **ActionButtonInFront**: Toggle this to **True** if you prefer the Edit/Delete/View buttons to appear at the very beginning of the row.
* **ExportButton**: Enable this to show the main data export menu on your pages.
* **CSVDataImport**: Set this to **True** to allow users to upload their own CSV files to populate your database tables.
* **ListCheckBox**: Enable this to add a checkbox to every row, allowing users to select multiple records for bulk actions.
* **EmptyRecordMessage**: Type the message you want users to see when there is no data to show (e.g., **No record found**).
* **PromptMessageBeforeDelete**: Customize the warning message shown before a user deletes a record.
* **MessageAfterDelete / Update / Add**: Use these fields to customize the success notifications the user receives after a successful database operation.

---

## Table Settings

Use these to fine-tune the visual look of your data grids.

* **TableStriped / TableHoverable**: Set these to **True** to add alternating row colors and highlight rows when the mouse moves over them.
* **TableResponsive**: Always keep this as **True** to ensure your tables look good on mobile devices and small screens.
* **TableDark**: Set this to **True** if you want all your data tables to have a dark-themed background.

---

## Pagination Settings

* **PaginationStyle**: Choose how users move between pages. **NumericPrevNext** shows page numbers alongside "Back" and "Next" buttons.
* **LoadIndicatorType**: Choose the style of the loading spinner (e.g., **q-spinner**) that appears when data is being fetched.

---

## Misc

* **FormAutoComplete**: Set to **True** to allow the browser to suggest previously typed information in form fields.
* **PRINT**: 
