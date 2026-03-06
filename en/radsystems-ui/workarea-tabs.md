---
title: Workarea Tabs
description: 
published: true
date: 2026-02-16T10:31:28.254Z
tags: 
editor: markdown
dateCreated: 2026-02-16T10:31:25.621Z
---

# RadSystems Studio Workarea Tabs

The central part of the screen is the **Work Area**, and it’s divided into three main tabs: **Pages**, **Page Design**, and **Publish**.

## Pages Tab

![rs-tab-pages.webp](/assets/radsystems-ui/rs-tab-pages.webp)

This is where most of your database-driven logic lives. The interface is split into **four columns**, each offering increasing levels of detail:

- **First Column – Database Tables and Views**  
    This column displays a tree structure of all your tables and database views. You can quickly navigate and manage CRUD operations for any table here.
    
- **Second Column – CRUD Pages**  
    For every selected table, RadSystems generates pages such as List, View, Add, Edit, and Delete. You can enable or disable any of these and even design each one separately.
    
- **Third Column – Page Fields**  
    Once you select a specific page (like Add or Edit), you’ll see all the fields available for that page. You can include or exclude fields and control how they behave during data entry or display.
    
- **Fourth Column – Field Properties**  
    When you select a field, this panel shows its detailed properties. For List or View pages, this includes display settings. For Add/Edit pages, you can configure how the field looks (textbox, select, checkbox, etc.), set data sources, placeholders, validation rules, and even add client-side events.

---
## Page Design Tab

![rs-tab-pagedesign.webp](/assets/radsystems-ui/rs-tab-pagedesign.webp)

One of the most powerful features of RadSystems Studio is its **visual drag-and-drop page builder**, which allows you to build rich user interfaces without writing code manually. When you switch to the **Page Design** tab, you’re presented with a clean and structured workspace divided into three main columns:
### 1. Page Components

- Located on the left, this panel contains all the UI components and widgets you can use in your page layout.
- These include headers, text blocks, charts, filters, accordions, tabbed pages, form wizards, buttons, modal windows, date and range pickers, and many more.
- There are also page/filter components and multi-choice lists that allow for advanced interactions.
- If you're building a data-driven app, you’ll appreciate the ability to use subpage components to nest one CRUD interface inside another—great for dashboards and relational interfaces.
### 2. Page Design Structure

- This is your central canvas where you actually build the page. You start by creating **sections**, then add **columns** within those sections, and finally drop components into those columns.
- This nested structure gives you full control over your layout, spacing, and responsiveness.
- Each element is clearly labeled, and you can drag-and-drop to reorder, duplicate, or delete components with ease.
### 3. Component Properties

- After placing a component in your layout, the right-hand panel updates to show all available configuration options for the selected component.
- Whether you’re working with a chart, a form field, or a custom text block, you can customize labels, assign data sources, bind to specific fields, define style classes, and apply conditional visibility rules. For charts, you can set data fields, axis labels, chart types (like bar, line, pie), and more.

### Custom JS and Custom CSS Buttons  
Just above the properties panel, you’ll find two incredibly useful options—**Page Custom JS** and **Page CSS Code**. These buttons allow you to inject JavaScript and CSS code specific to the page you are working on. This is not application-wide—your scripts and styles will apply only to the current page. It’s perfect for fine-tuning UI behavior, adding interactions, or overriding default styles without affecting the rest of the app.

With this intuitive design environment, RadSystems empowers users of all skill levels to create sophisticated, responsive, and data-rich user interfaces—visually and efficiently.

---

## Publish Tab

![rs-tab-publish.webp](/assets/radsystems-ui/rs-tab-publish.webp)

Once your application setup and data connections are complete, the **Publish** feature compiles and prepares your project for testing or deployment. After publishing, a confirmation screen appears showing a success message and a local URL for previewing the application.

**Preview in Browser**  
Opens the generated application in your selected browser for immediate testing. This allows you to quickly verify functionality and UI changes.

**Re-Publish Project**  
Regenerates the entire application build. Useful after major updates or if build issues occur, ensuring a clean output.

**Browse Project Folder**  
Opens the project directory, giving direct access to generated code, assets, and configuration files. Helpful for advanced customization or integration work.

**Clean Project**  
Detects and removes unused or leftover build files. This helps maintain a clean project structure and avoids unnecessary clutter.
